---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 03/26/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: d8307ca9797a9a780d7e08d6d21cb66446c7e289
ms.sourcegitcommit: 6d9e8ee6dd07cfd07239a2948304d7f50ef781cc
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/27/2019
ms.locfileid: "58508908"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="99f85-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="99f85-103">Azure CLI release notes</span></span>
## <a name="march-26-2019"></a><span data-ttu-id="99f85-104">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-104">March 26, 2019</span></span>

### <a name="core"></a><span data-ttu-id="99f85-105">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-105">Core</span></span>
* <span data-ttu-id="99f85-106">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="99f85-106">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="99f85-107">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="99f85-107">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="99f85-108">Облако</span><span class="sxs-lookup"><span data-stu-id="99f85-108">Cloud</span></span>
* <span data-ttu-id="99f85-109">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="99f85-109">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-110">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-110">ACR</span></span>
* <span data-ttu-id="99f85-111">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="99f85-111">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="99f85-112">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-112">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="99f85-113">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="99f85-113">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="99f85-114">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="99f85-114">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-115">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-115">AppService</span></span>
* <span data-ttu-id="99f85-116">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="99f85-116">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="99f85-117">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="99f85-117">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="99f85-118">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="99f85-118">BOT Service</span></span>
* <span data-ttu-id="99f85-119">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="99f85-119">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="99f85-120">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="99f85-120">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="99f85-121">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="99f85-121">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="99f85-122">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="99f85-122">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="99f85-123">CDN</span><span class="sxs-lookup"><span data-stu-id="99f85-123">CDN</span></span>
* <span data-ttu-id="99f85-124">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-124">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="99f85-125">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-125">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="99f85-126">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-126">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="99f85-127">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="99f85-127">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="99f85-128">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="99f85-128">Cosmosdb</span></span>
* <span data-ttu-id="99f85-129">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="99f85-129">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="99f85-130">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="99f85-130">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-131">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-131">Interactive</span></span>
* <span data-ttu-id="99f85-132">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="99f85-132">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-133">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-133">Monitor</span></span>
* <span data-ttu-id="99f85-134">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-134">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="99f85-135">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-135">Network</span></span>
* <span data-ttu-id="99f85-136">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="99f85-136">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="99f85-137">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-137">Profile</span></span>
* <span data-ttu-id="99f85-138">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="99f85-138">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="99f85-139">Postgres</span><span class="sxs-lookup"><span data-stu-id="99f85-139">Postgres</span></span> 
* <span data-ttu-id="99f85-140">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="99f85-140">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="99f85-141">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="99f85-141">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-142">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-142">Resource</span></span>
* <span data-ttu-id="99f85-143">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-143">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="99f85-144">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="99f85-144">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="99f85-145">График</span><span class="sxs-lookup"><span data-stu-id="99f85-145">Graph</span></span>
* <span data-ttu-id="99f85-146">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="99f85-146">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="99f85-147">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="99f85-147">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="99f85-148">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="99f85-148">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="99f85-149">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="99f85-149">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="99f85-150">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="99f85-150">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-151">storage</span><span class="sxs-lookup"><span data-stu-id="99f85-151">storage</span></span>
* <span data-ttu-id="99f85-152">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="99f85-152">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="99f85-153">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="99f85-153">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="99f85-154">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="99f85-154">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="99f85-155">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="99f85-155">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-156">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-156">VM</span></span>
* <span data-ttu-id="99f85-157">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-157">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="99f85-158">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-158">March 12, 2019</span></span>

<span data-ttu-id="99f85-159">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="99f85-159">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="99f85-160">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-160">Core</span></span>

* <span data-ttu-id="99f85-161">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="99f85-161">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-162">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-162">ACR</span></span>

* <span data-ttu-id="99f85-163">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="99f85-163">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-164">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-164">ACS</span></span>

* <span data-ttu-id="99f85-165">Аргумент `--listen-address` для `aks browse` игнорируется, если `kubectl` не поддерживает его.</span><span class="sxs-lookup"><span data-stu-id="99f85-165">Changed to ignore `--listen-address` argument to `aks browse` if `kubectl` doesn't support it</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-166">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-166">AppService</span></span>

* <span data-ttu-id="99f85-167">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="99f85-167">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="99f85-168">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-168">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="99f85-169">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="99f85-169">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="99f85-170">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="99f85-170">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="99f85-171">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="99f85-171">Botservice</span></span>

* <span data-ttu-id="99f85-172">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="99f85-172">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="99f85-173">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="99f85-173">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="99f85-174">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-174">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="99f85-175">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="99f85-175">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="99f85-176">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-176">Container</span></span>

* <span data-ttu-id="99f85-177">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="99f85-177">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="99f85-178">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="99f85-178">EventHub</span></span>

* <span data-ttu-id="99f85-179">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="99f85-179">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="99f85-180">Поиск</span><span class="sxs-lookup"><span data-stu-id="99f85-180">Find</span></span>

* <span data-ttu-id="99f85-181">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="99f85-181">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="99f85-182">HDInsight</span><span class="sxs-lookup"><span data-stu-id="99f85-182">HDInsight</span></span>

* <span data-ttu-id="99f85-183">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="99f85-183">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="99f85-184">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-184">Network</span></span>

* <span data-ttu-id="99f85-185">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="99f85-185">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="99f85-186">Rdbms</span><span class="sxs-lookup"><span data-stu-id="99f85-186">Rdbms</span></span>

* <span data-ttu-id="99f85-187">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="99f85-187">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="99f85-188">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-188">Role</span></span>

* <span data-ttu-id="99f85-189">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="99f85-189">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="99f85-190">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="99f85-190">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="99f85-191">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="99f85-191">Service Fabric</span></span>

* <span data-ttu-id="99f85-192">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="99f85-192">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="99f85-193">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-193">February 26, 2019</span></span>

<span data-ttu-id="99f85-194">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="99f85-194">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="99f85-195">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-195">Core</span></span>

* <span data-ttu-id="99f85-196">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="99f85-196">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-197">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-197">ACR</span></span>

* <span data-ttu-id="99f85-198">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-198">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="99f85-199">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="99f85-199">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-200">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-200">ACS</span></span>

* <span data-ttu-id="99f85-201">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="99f85-201">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-202">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-202">AppService</span></span>

* <span data-ttu-id="99f85-203">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="99f85-203">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="99f85-204">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-204">Batch</span></span>
* <span data-ttu-id="99f85-205">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="99f85-205">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="99f85-206">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="99f85-206">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="99f85-207">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="99f85-207">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="99f85-208">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="99f85-208">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="99f85-209">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="99f85-209">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="99f85-210">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="99f85-210">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="99f85-211">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="99f85-211">CosmosDB</span></span>

* <span data-ttu-id="99f85-212">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="99f85-212">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="99f85-213">Kusto</span><span class="sxs-lookup"><span data-stu-id="99f85-213">Kusto</span></span>

* <span data-ttu-id="99f85-214">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="99f85-214">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="99f85-215">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-215">Network</span></span>

* <span data-ttu-id="99f85-216">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="99f85-216">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="99f85-217">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="99f85-217">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="99f85-218">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="99f85-218">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="99f85-219">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-219">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="99f85-220">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-220">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="99f85-221">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="99f85-221">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="99f85-222">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="99f85-222">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-223">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-223">Resource</span></span>

* <span data-ttu-id="99f85-224">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="99f85-224">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="99f85-225">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-225">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="99f85-226">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-226">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="99f85-227">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-227">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="99f85-228">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="99f85-228">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="99f85-229">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-229">Role</span></span>

* <span data-ttu-id="99f85-230">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-230">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-231">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-231">VM</span></span>

* <span data-ttu-id="99f85-232">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="99f85-232">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="99f85-233">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-233">February 12, 2019</span></span>

<span data-ttu-id="99f85-234">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="99f85-234">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="99f85-235">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-235">Core</span></span>

* <span data-ttu-id="99f85-236">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="99f85-236">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="99f85-237">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="99f85-237">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-238">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-238">ACR</span></span>
* <span data-ttu-id="99f85-239">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="99f85-239">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="99f85-240">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="99f85-240">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-241">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-241">ACS</span></span>
* <span data-ttu-id="99f85-242">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="99f85-242">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="99f85-243">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="99f85-243">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="99f85-244">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="99f85-244">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="99f85-245">AMS</span><span class="sxs-lookup"><span data-stu-id="99f85-245">AMS</span></span>
* <span data-ttu-id="99f85-246">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-246">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="99f85-247">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-247">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-248">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-248">Appservice</span></span>
* <span data-ttu-id="99f85-249">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="99f85-249">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="99f85-250">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="99f85-250">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="99f85-251">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-251">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="99f85-252">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="99f85-252">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="99f85-253">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="99f85-253">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="99f85-254">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="99f85-254">Botservice</span></span>
* <span data-ttu-id="99f85-255">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="99f85-255">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="99f85-256">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="99f85-256">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="99f85-257">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-257">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="99f85-258">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="99f85-258">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="99f85-259">[УСТАРЕЛО.] Аргумент `--proj-name` не поддерживается. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="99f85-259">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="99f85-260">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="99f85-260">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="99f85-261">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="99f85-261">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="99f85-262">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="99f85-262">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="99f85-263">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="99f85-263">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="99f85-264">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="99f85-264">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="99f85-265">Key Vault</span><span class="sxs-lookup"><span data-stu-id="99f85-265">Key Vault</span></span>
* <span data-ttu-id="99f85-266">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="99f85-266">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-267">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-267">Monitor</span></span>
* <span data-ttu-id="99f85-268">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="99f85-268">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="99f85-269">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-269">Network</span></span>
* <span data-ttu-id="99f85-270">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="99f85-270">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="99f85-271">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="99f85-271">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="99f85-272">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="99f85-272">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="99f85-273">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="99f85-273">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="99f85-274">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="99f85-274">Policy Insights</span></span>
* <span data-ttu-id="99f85-275">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="99f85-275">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="99f85-276">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="99f85-276">RDBMS</span></span>
* <span data-ttu-id="99f85-277">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="99f85-277">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="99f85-278">Redis</span><span class="sxs-lookup"><span data-stu-id="99f85-278">Redis</span></span>
* <span data-ttu-id="99f85-279">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="99f85-279">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="99f85-280">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="99f85-280">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="99f85-281">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="99f85-281">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="99f85-282">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="99f85-282">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="99f85-283">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="99f85-283">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="99f85-284">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="99f85-284">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="99f85-285">[УСТРАРЕЛО.] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99f85-285">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="99f85-286">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-286">Role</span></span>
* <span data-ttu-id="99f85-287">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="99f85-287">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="99f85-288">ВМ SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-288">SQL VM</span></span>
* <span data-ttu-id="99f85-289">[УСТАРЕЛО.] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="99f85-289">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-290">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-290">VM</span></span>
* <span data-ttu-id="99f85-291">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="99f85-291">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="99f85-292">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-292">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="99f85-293">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="99f85-293">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="99f85-294">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="99f85-294">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="99f85-295">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-295">January 31, 2019</span></span>

<span data-ttu-id="99f85-296">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="99f85-296">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="99f85-297">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-297">Core</span></span>

* <span data-ttu-id="99f85-298">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="99f85-298">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="99f85-299">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-299">January 28, 2019</span></span>

<span data-ttu-id="99f85-300">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="99f85-300">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-301">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-301">ACR</span></span>
* <span data-ttu-id="99f85-302">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="99f85-302">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-303">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-303">ACS</span></span>
* <span data-ttu-id="99f85-304">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="99f85-304">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="99f85-305">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="99f85-305">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="99f85-306">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="99f85-306">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="99f85-307">AMS</span><span class="sxs-lookup"><span data-stu-id="99f85-307">AMS</span></span>
* <span data-ttu-id="99f85-308">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="99f85-308">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="99f85-309">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="99f85-309">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-310">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-310">Appservice</span></span>
* <span data-ttu-id="99f85-311">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-311">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="99f85-312">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="99f85-312">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="99f85-313">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="99f85-313">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="99f85-314">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-314">Container</span></span>
* <span data-ttu-id="99f85-315">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="99f85-315">Added `container start` command</span></span>
* <span data-ttu-id="99f85-316">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-316">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="99f85-317">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="99f85-317">EventGrid</span></span>
* <span data-ttu-id="99f85-318">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-318">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="99f85-319">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="99f85-319">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="99f85-320">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="99f85-320">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="99f85-321">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="99f85-321">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="99f85-322">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="99f85-322">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="99f85-323">HDInsight</span><span class="sxs-lookup"><span data-stu-id="99f85-323">HDInsight</span></span>
* <span data-ttu-id="99f85-324">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="99f85-324">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="99f85-325">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="99f85-325">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="99f85-326">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-326">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="99f85-327">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="99f85-327">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="99f85-328">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="99f85-328">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="99f85-329">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-329">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="99f85-330">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="99f85-330">IoT</span></span>
* <span data-ttu-id="99f85-331">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="99f85-331">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="99f85-332">Kusto</span><span class="sxs-lookup"><span data-stu-id="99f85-332">Kusto</span></span>
* <span data-ttu-id="99f85-333">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="99f85-333">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-334">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-334">Monitor</span></span>
* <span data-ttu-id="99f85-335">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="99f85-335">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="99f85-336">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-336">Profile</span></span>
* <span data-ttu-id="99f85-337">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-337">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="99f85-338">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-338">Network</span></span>
* <span data-ttu-id="99f85-339">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="99f85-339">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="99f85-340">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="99f85-340">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-341">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-341">Resource</span></span>
* <span data-ttu-id="99f85-342">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-342">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="99f85-343">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-343">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="99f85-344">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-344">SQL Virtual Machine</span></span>
* <span data-ttu-id="99f85-345">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="99f85-345">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-346">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-346">Storage</span></span>
* <span data-ttu-id="99f85-347">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="99f85-347">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="99f85-348">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="99f85-348">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-349">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-349">VM</span></span>
* <span data-ttu-id="99f85-350">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="99f85-350">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="99f85-351">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="99f85-351">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="99f85-352">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-352">January 15, 2019</span></span>

<span data-ttu-id="99f85-353">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="99f85-353">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-354">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-354">ACR</span></span>
* <span data-ttu-id="99f85-355">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="99f85-355">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="99f85-356">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="99f85-356">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="99f85-357">[УСТАРЕЛО.] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="99f85-357">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="99f85-358">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-358">ACS</span></span>
* <span data-ttu-id="99f85-359">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="99f85-359">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-360">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-360">Appservice</span></span>
* <span data-ttu-id="99f85-361">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="99f85-361">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="99f85-362">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="99f85-362">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="99f85-363">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="99f85-363">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="99f85-364">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="99f85-364">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="99f85-365">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="99f85-365">Botservice</span></span>
* <span data-ttu-id="99f85-366">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-366">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="99f85-367">Настройка</span><span class="sxs-lookup"><span data-stu-id="99f85-367">Configure</span></span>
* <span data-ttu-id="99f85-368">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="99f85-368">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="99f85-369">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="99f85-369">CosmosDB</span></span>
* <span data-ttu-id="99f85-370">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="99f85-370">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="99f85-371">HDInsight</span><span class="sxs-lookup"><span data-stu-id="99f85-371">HDInsight</span></span>
* <span data-ttu-id="99f85-372">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="99f85-372">Added commands for managing applications</span></span>
* <span data-ttu-id="99f85-373">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="99f85-373">Added commands for managing script actions</span></span>
* <span data-ttu-id="99f85-374">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="99f85-374">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="99f85-375">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="99f85-375">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="99f85-376">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-376">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="99f85-377">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-377">Network</span></span>
* <span data-ttu-id="99f85-378">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="99f85-378">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="99f85-379">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="99f85-379">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="99f85-380">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="99f85-380">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="99f85-381">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-381">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="99f85-382">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-382">Role</span></span>
* <span data-ttu-id="99f85-383">[УСТАРЕЛО.] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="99f85-383">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="99f85-384">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="99f85-384">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="99f85-385">Безопасность</span><span class="sxs-lookup"><span data-stu-id="99f85-385">Security</span></span>
* <span data-ttu-id="99f85-386">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="99f85-386">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-387">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-387">Storage</span></span>
* <span data-ttu-id="99f85-388">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="99f85-388">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="99f85-389">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="99f85-389">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="99f85-390">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="99f85-390">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="99f85-391">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="99f85-391">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="99f85-392">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="99f85-392">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-393">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-393">VM</span></span>
* <span data-ttu-id="99f85-394">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="99f85-394">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="99f85-395">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-395">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="99f85-396">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="99f85-396">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="99f85-397">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="99f85-397">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="99f85-398">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-398">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="99f85-399">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="99f85-399">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="99f85-400">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-400">December 20, 2018</span></span>

<span data-ttu-id="99f85-401">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="99f85-401">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="99f85-402">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-402">Appservice</span></span>
* <span data-ttu-id="99f85-403">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="99f85-403">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="99f85-404">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="99f85-404">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="99f85-405">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="99f85-405">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="99f85-406">IoT Central</span><span class="sxs-lookup"><span data-stu-id="99f85-406">IoTCentral</span></span>
* <span data-ttu-id="99f85-407">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="99f85-407">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="99f85-408">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-408">Role</span></span>
* <span data-ttu-id="99f85-409">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="99f85-409">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-410">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-410">SQL</span></span>
* <span data-ttu-id="99f85-411">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="99f85-411">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-412">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-412">VM</span></span>
* <span data-ttu-id="99f85-413">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-413">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="99f85-414">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-414">December 18, 2018</span></span>

<span data-ttu-id="99f85-415">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="99f85-415">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="99f85-416">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-416">ACR</span></span>
* <span data-ttu-id="99f85-417">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-417">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="99f85-418">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="99f85-418">Condensed the table layout for task list</span></span>
* <span data-ttu-id="99f85-419">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="99f85-419">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-420">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-420">ACS</span></span>
* <span data-ttu-id="99f85-421">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="99f85-421">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="99f85-422">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="99f85-422">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="99f85-423">[УСТАРЕЛО] Команды `az acs` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="99f85-423">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="99f85-424">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-424">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="99f85-425">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="99f85-425">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="99f85-426">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="99f85-426">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-427">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-427">Appservice</span></span>
* <span data-ttu-id="99f85-428">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="99f85-428">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="99f85-429">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="99f85-429">Botservice</span></span>
* <span data-ttu-id="99f85-430">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-430">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="99f85-431">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="99f85-431">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="99f85-432">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="99f85-432">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="99f85-433">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="99f85-433">Reduced Kudu network calls</span></span>
* <span data-ttu-id="99f85-434">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="99f85-434">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="99f85-435">Потребление</span><span class="sxs-lookup"><span data-stu-id="99f85-435">Consumption</span></span>
* <span data-ttu-id="99f85-436">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="99f85-436">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="99f85-437">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="99f85-437">CosmosDB</span></span>
* <span data-ttu-id="99f85-438">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="99f85-438">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="99f85-439">Карты</span><span class="sxs-lookup"><span data-stu-id="99f85-439">Maps</span></span>
* <span data-ttu-id="99f85-440">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="99f85-440">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="99f85-441">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-441">Network</span></span>
* <span data-ttu-id="99f85-442">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="99f85-442">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="99f85-443">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="99f85-443">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-444">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-444">Resource</span></span>
* <span data-ttu-id="99f85-445">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-445">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="99f85-446">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-446">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-447">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-447">Storage</span></span>
*  <span data-ttu-id="99f85-448">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="99f85-448">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-449">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-449">VM</span></span>
* <span data-ttu-id="99f85-450">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-450">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="99f85-451">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-451">December 4, 2018</span></span>

<span data-ttu-id="99f85-452">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="99f85-452">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="99f85-453">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-453">Core</span></span>
* <span data-ttu-id="99f85-454">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-454">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="99f85-455">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="99f85-455">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-456">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-456">Appservice</span></span>
* <span data-ttu-id="99f85-457">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="99f85-457">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="99f85-458">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="99f85-458">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="99f85-459">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-459">Network</span></span>
* <span data-ttu-id="99f85-460">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="99f85-460">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="99f85-461">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-461">Role</span></span>
* <span data-ttu-id="99f85-462">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="99f85-462">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="99f85-463">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-463">VM</span></span>
* <span data-ttu-id="99f85-464">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` устарел.</span><span class="sxs-lookup"><span data-stu-id="99f85-464">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="99f85-465">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="99f85-465">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="99f85-466">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="99f85-466">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="99f85-467">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="99f85-467">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="99f85-468">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-468">November 20, 2018</span></span>

<span data-ttu-id="99f85-469">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="99f85-469">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="99f85-470">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-470">Core</span></span>
* <span data-ttu-id="99f85-471">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="99f85-471">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-472">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-472">ACR</span></span>
* <span data-ttu-id="99f85-473">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="99f85-473">Added context token to task step</span></span>
* <span data-ttu-id="99f85-474">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="99f85-474">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="99f85-475">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="99f85-475">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-476">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-476">Appservice</span></span>
* <span data-ttu-id="99f85-477">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="99f85-477">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="99f85-478">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-478">Updated the default `node_version`.</span></span> <span data-ttu-id="99f85-479">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="99f85-479">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="99f85-480">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="99f85-480">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="99f85-481">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="99f85-481">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="99f85-482">IotCentral</span><span class="sxs-lookup"><span data-stu-id="99f85-482">IotCentral</span></span>
* <span data-ttu-id="99f85-483">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="99f85-483">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="99f85-484">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="99f85-484">KeyVault</span></span>
* <span data-ttu-id="99f85-485">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="99f85-485">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="99f85-486">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-486">Network</span></span>
* <span data-ttu-id="99f85-487">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="99f85-487">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="99f85-488">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="99f85-488">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="99f85-489">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="99f85-489">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="99f85-490">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="99f85-490">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="99f85-491">Rdbms</span><span class="sxs-lookup"><span data-stu-id="99f85-491">Rdbms</span></span>
* <span data-ttu-id="99f85-492">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="99f85-492">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="99f85-493">RBAC:</span><span class="sxs-lookup"><span data-stu-id="99f85-493">Rbac</span></span>
* <span data-ttu-id="99f85-494">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-494">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="99f85-495">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="99f85-495">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="99f85-496">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-496">Storage</span></span>
* <span data-ttu-id="99f85-497">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="99f85-497">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="99f85-498">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="99f85-498">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="99f85-499">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="99f85-499">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="99f85-500">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="99f85-500">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-501">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-501">VM</span></span>
* <span data-ttu-id="99f85-502">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="99f85-502">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="99f85-503">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="99f85-503">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="99f85-504">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="99f85-504">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="99f85-505">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="99f85-505">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="99f85-506">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-506">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="99f85-507">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-507">Added `snapshot wait` command</span></span>
* <span data-ttu-id="99f85-508">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="99f85-508">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="99f85-509">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-509">November 6, 2018</span></span>

<span data-ttu-id="99f85-510">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="99f85-510">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="99f85-511">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-511">Core</span></span>
* <span data-ttu-id="99f85-512">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="99f85-512">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-513">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-513">ACR</span></span>
* <span data-ttu-id="99f85-514">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="99f85-514">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="99f85-515">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="99f85-515">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-516">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-516">ACS</span></span>
* <span data-ttu-id="99f85-517">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-517">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="99f85-518">Помощник</span><span class="sxs-lookup"><span data-stu-id="99f85-518">Advisor</span></span>
* <span data-ttu-id="99f85-519">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="99f85-519">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="99f85-520">AMS</span><span class="sxs-lookup"><span data-stu-id="99f85-520">AMS</span></span>
* <span data-ttu-id="99f85-521">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="99f85-521">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="99f85-522">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="99f85-522">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="99f85-523">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-523">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="99f85-524">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="99f85-524">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="99f85-525">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="99f85-525">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="99f85-526">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="99f85-526">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="99f85-527">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="99f85-527">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="99f85-528">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="99f85-528">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="99f85-529">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="99f85-529">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="99f85-530">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="99f85-530">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="99f85-531">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="99f85-531">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="99f85-532">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="99f85-532">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="99f85-533">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="99f85-533">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="99f85-534">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="99f85-534">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="99f85-535">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="99f85-535">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="99f85-536">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="99f85-536">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="99f85-537">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="99f85-537">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-538">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-538">AppService</span></span>
* <span data-ttu-id="99f85-539">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="99f85-539">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="99f85-540">Настройка</span><span class="sxs-lookup"><span data-stu-id="99f85-540">Configure</span></span>
* <span data-ttu-id="99f85-541">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="99f85-541">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="99f85-542">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-542">Container</span></span>
* <span data-ttu-id="99f85-543">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="99f85-543">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="99f85-544">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="99f85-544">EventHub</span></span>
* <span data-ttu-id="99f85-545">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-545">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-546">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-546">Interactive</span></span>
* <span data-ttu-id="99f85-547">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="99f85-547">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-548">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-548">Monitor</span></span>
* <span data-ttu-id="99f85-549">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-549">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="99f85-550">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-550">Network</span></span>
* <span data-ttu-id="99f85-551">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="99f85-551">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="99f85-552">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="99f85-552">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="99f85-553">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-553">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="99f85-554">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-554">Profile</span></span>
* <span data-ttu-id="99f85-555">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="99f85-555">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="99f85-556">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="99f85-556">RDBMS</span></span>
* <span data-ttu-id="99f85-557">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="99f85-557">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-558">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-558">Resource</span></span>
* <span data-ttu-id="99f85-559">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="99f85-559">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="99f85-560">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-560">Role</span></span>
* <span data-ttu-id="99f85-561">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="99f85-561">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="99f85-562">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-562">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="99f85-563">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="99f85-563">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-564">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-564">Storage</span></span>
* <span data-ttu-id="99f85-565">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="99f85-565">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-566">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-566">VM</span></span>
* <span data-ttu-id="99f85-567">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="99f85-567">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="99f85-568">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="99f85-568">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="99f85-569">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="99f85-569">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="99f85-570">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="99f85-570">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="99f85-571">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="99f85-571">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="99f85-572">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="99f85-572">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="99f85-573">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-573">October 23, 2018</span></span>

<span data-ttu-id="99f85-574">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="99f85-574">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="99f85-575">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-575">Core</span></span>
* <span data-ttu-id="99f85-576">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="99f85-576">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="99f85-577">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="99f85-577">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-578">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-578">ACR</span></span>
* <span data-ttu-id="99f85-579">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="99f85-579">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="99f85-580">CDN</span><span class="sxs-lookup"><span data-stu-id="99f85-580">CDN</span></span>
* <span data-ttu-id="99f85-581">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-581">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="99f85-582">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="99f85-582">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="99f85-583">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-583">Container</span></span>
* <span data-ttu-id="99f85-584">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="99f85-584">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="99f85-585">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="99f85-585">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="99f85-586">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="99f85-586">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="99f85-587">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-587">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="99f85-588">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="99f85-588">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="99f85-589">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="99f85-589">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="99f85-590">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-590">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="99f85-591">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="99f85-591">CosmosDB</span></span>
* <span data-ttu-id="99f85-592">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="99f85-592">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-593">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-593">Interactive</span></span>
* <span data-ttu-id="99f85-594">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="99f85-594">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="99f85-595">IoT Central</span><span class="sxs-lookup"><span data-stu-id="99f85-595">IoT Central</span></span>
* <span data-ttu-id="99f85-596">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="99f85-596">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="99f85-597">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="99f85-597">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-598">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-598">Monitor</span></span>
* <span data-ttu-id="99f85-599">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="99f85-599">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="99f85-600">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="99f85-600">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="99f85-601">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="99f85-601">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="99f85-602">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="99f85-602">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="99f85-603">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="99f85-603">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="99f85-604">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="99f85-604">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="99f85-605">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="99f85-605">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="99f85-606">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="99f85-606">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="99f85-607">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="99f85-607">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="99f85-608">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-608">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="99f85-609">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-609">Network</span></span>
* <span data-ttu-id="99f85-610">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="99f85-610">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="99f85-611">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="99f85-611">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="99f85-612">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="99f85-612">ServiceBus</span></span>
* <span data-ttu-id="99f85-613">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="99f85-613">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-614">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-614">SQL</span></span>
* <span data-ttu-id="99f85-615">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="99f85-615">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-616">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-616">Storage</span></span>
* <span data-ttu-id="99f85-617">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-617">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="99f85-618">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="99f85-618">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-619">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-619">VM</span></span>
* <span data-ttu-id="99f85-620">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="99f85-620">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="99f85-621">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="99f85-621">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="99f85-622">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="99f85-622">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="99f85-623">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-623">October 16, 2018</span></span>

<span data-ttu-id="99f85-624">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="99f85-624">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-625">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-625">VM</span></span>
* <span data-ttu-id="99f85-626">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="99f85-626">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="99f85-627">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-627">October 9, 2018</span></span>

<span data-ttu-id="99f85-628">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="99f85-628">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="99f85-629">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-629">Core</span></span>
* <span data-ttu-id="99f85-630">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="99f85-630">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-631">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-631">ACR</span></span>
* <span data-ttu-id="99f85-632">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="99f85-632">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-633">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-633">ACS</span></span>
* <span data-ttu-id="99f85-634">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="99f85-634">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="99f85-635">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="99f85-635">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="99f85-636">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="99f85-636">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="99f85-637">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="99f85-637">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="99f85-638">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-638">Container</span></span>
* <span data-ttu-id="99f85-639">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="99f85-639">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="99f85-640">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="99f85-640">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="99f85-641">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="99f85-641">Event Hub</span></span>
* <span data-ttu-id="99f85-642">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-642">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="99f85-643">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="99f85-643">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="99f85-644">расширения.</span><span class="sxs-lookup"><span data-stu-id="99f85-644">Extensions</span></span>
* <span data-ttu-id="99f85-645">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="99f85-645">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="99f85-646">HDInsight</span><span class="sxs-lookup"><span data-stu-id="99f85-646">HDInsight</span></span>
* <span data-ttu-id="99f85-647">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="99f85-647">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="99f85-648">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="99f85-648">IoT</span></span>
* <span data-ttu-id="99f85-649">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="99f85-649">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="99f85-650">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="99f85-650">KeyVault</span></span>
* <span data-ttu-id="99f85-651">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="99f85-651">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="99f85-652">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-652">Network</span></span>
* <span data-ttu-id="99f85-653">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-653">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="99f85-654">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="99f85-654">See #6052</span></span>
* <span data-ttu-id="99f85-655">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-655">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="99f85-656">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="99f85-656">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="99f85-657">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="99f85-657">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="99f85-658">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="99f85-658">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="99f85-659">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="99f85-659">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="99f85-660">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-660">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="99f85-661">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-661">Role</span></span>
* <span data-ttu-id="99f85-662">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="99f85-662">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="99f85-663">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="99f85-663">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="99f85-664">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="99f85-664">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="99f85-665">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="99f85-665">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="99f85-666">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-666">Service Bus</span></span>
* <span data-ttu-id="99f85-667">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="99f85-667">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-668">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-668">VM</span></span>
* <span data-ttu-id="99f85-669">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="99f85-669">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="99f85-670">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="99f85-670">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="99f85-671">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="99f85-671">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="99f85-672">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="99f85-672">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="99f85-673">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="99f85-673">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="99f85-674">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="99f85-674">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="99f85-675">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-675">September 21, 2018</span></span>

<span data-ttu-id="99f85-676">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="99f85-676">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-677">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-677">ACR</span></span>
* <span data-ttu-id="99f85-678">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="99f85-678">Added ACR Task commands</span></span>
* <span data-ttu-id="99f85-679">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="99f85-679">Added quick run command</span></span>
* <span data-ttu-id="99f85-680">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="99f85-680">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="99f85-681">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="99f85-681">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="99f85-682">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="99f85-682">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="99f85-683">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="99f85-683">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-684">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-684">ACS</span></span>
* <span data-ttu-id="99f85-685">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="99f85-685">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="99f85-686">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="99f85-686">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-687">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-687">AppService</span></span>

* <span data-ttu-id="99f85-688">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="99f85-688">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="99f85-689">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="99f85-689">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="99f85-690">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="99f85-690">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="99f85-691">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="99f85-691">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="99f85-692">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-692">Batch</span></span>
* <span data-ttu-id="99f85-693">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="99f85-693">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="99f85-694">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="99f85-694">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="99f85-695">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-695">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="99f85-696">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="99f85-696">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="99f85-697">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="99f85-697">Batch AI</span></span> 
* <span data-ttu-id="99f85-698">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-698">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="99f85-699">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="99f85-699">Cognitive Services</span></span>
* <span data-ttu-id="99f85-700">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="99f85-700">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="99f85-701">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="99f85-701">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="99f85-702">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="99f85-702">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="99f85-703">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="99f85-703">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="99f85-704">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="99f85-704">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="99f85-705">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="99f85-705">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="99f85-706">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-706">Container</span></span>
* <span data-ttu-id="99f85-707">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-707">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="99f85-708">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="99f85-708">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="99f85-709">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="99f85-709">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="99f85-710">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-710">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="99f85-711">Data Lake</span><span class="sxs-lookup"><span data-stu-id="99f85-711">Datalake</span></span>
* <span data-ttu-id="99f85-712">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="99f85-712">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="99f85-713">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="99f85-713">Interactive Shell</span></span>
* <span data-ttu-id="99f85-714">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="99f85-714">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="99f85-715">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="99f85-715">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="99f85-716">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="99f85-716">IoT</span></span>
* <span data-ttu-id="99f85-717">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="99f85-717">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="99f85-718">Key Vault</span><span class="sxs-lookup"><span data-stu-id="99f85-718">Key Vault</span></span>
* <span data-ttu-id="99f85-719">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="99f85-719">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="99f85-720">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-720">Network</span></span>
* <span data-ttu-id="99f85-721">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="99f85-721">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="99f85-722">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-722">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="99f85-723">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="99f85-723">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="99f85-724">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="99f85-724">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="99f85-725">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-725">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="99f85-726">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-726">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="99f85-727">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="99f85-727">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="99f85-728">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="99f85-728">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="99f85-729">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="99f85-729">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="99f85-730">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="99f85-730">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="99f85-731">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="99f85-731">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="99f85-732">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="99f85-732">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="99f85-733">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="99f85-733">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="99f85-734">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="99f85-734">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="99f85-735">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="99f85-735">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="99f85-736">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="99f85-736">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="99f85-737">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="99f85-737">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="99f85-738">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="99f85-738">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="99f85-739">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="99f85-739">RDBMS</span></span>
* <span data-ttu-id="99f85-740">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="99f85-740">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="99f85-741">резервирование.</span><span class="sxs-lookup"><span data-stu-id="99f85-741">Reservation</span></span>
* <span data-ttu-id="99f85-742">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="99f85-742">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="99f85-743">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="99f85-743">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="99f85-744">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="99f85-744">Manage App</span></span>
* <span data-ttu-id="99f85-745">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="99f85-745">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="99f85-746">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="99f85-746">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="99f85-747">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-747">Role</span></span>
* <span data-ttu-id="99f85-748">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="99f85-748">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="99f85-749">SignalR</span><span class="sxs-lookup"><span data-stu-id="99f85-749">SignalR</span></span>
* <span data-ttu-id="99f85-750">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="99f85-750">First release</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-751">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-751">Storage</span></span>
* <span data-ttu-id="99f85-752">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="99f85-752">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="99f85-753">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="99f85-753">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-754">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-754">VM</span></span>
* <span data-ttu-id="99f85-755">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="99f85-755">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="99f85-756">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="99f85-756">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="99f85-757">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-757">August 28, 2018</span></span>

<span data-ttu-id="99f85-758">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="99f85-758">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="99f85-759">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-759">Core</span></span>

* <span data-ttu-id="99f85-760">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="99f85-760">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="99f85-761">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="99f85-761">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-762">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-762">ACR</span></span>

* <span data-ttu-id="99f85-763">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="99f85-763">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="99f85-764">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="99f85-764">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-765">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-765">ACS</span></span>

* <span data-ttu-id="99f85-766">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="99f85-766">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="99f85-767">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="99f85-767">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-768">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-768">AppService</span></span>

* <span data-ttu-id="99f85-769">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="99f85-769">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="99f85-770">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="99f85-770">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="99f85-771">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="99f85-771">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="99f85-772">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="99f85-772">Backup</span></span>

* <span data-ttu-id="99f85-773">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="99f85-773">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="99f85-774">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="99f85-774">Bot Service</span></span>

* <span data-ttu-id="99f85-775">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="99f85-775">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="99f85-776">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="99f85-776">Cognitive Services</span></span>

* <span data-ttu-id="99f85-777">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="99f85-777">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="99f85-778">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="99f85-778">IoT</span></span>

* <span data-ttu-id="99f85-779">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="99f85-779">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-780">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-780">Monitor</span></span>

* <span data-ttu-id="99f85-781">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="99f85-781">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="99f85-782">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="99f85-782">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="99f85-783">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-783">Network</span></span>

* <span data-ttu-id="99f85-784">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="99f85-784">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-785">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-785">Resource</span></span>

* <span data-ttu-id="99f85-786">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="99f85-786">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-787">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-787">Storage</span></span>

* <span data-ttu-id="99f85-788">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="99f85-788">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-789">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-789">VM</span></span>

* <span data-ttu-id="99f85-790">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="99f85-790">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="99f85-791">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-791">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="99f85-792">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-792">Auguest 14, 2018</span></span>

<span data-ttu-id="99f85-793">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="99f85-793">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="99f85-794">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-794">Core</span></span>

* <span data-ttu-id="99f85-795">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="99f85-795">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="99f85-796">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="99f85-796">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="99f85-797">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="99f85-797">Telemetry</span></span>

* <span data-ttu-id="99f85-798">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="99f85-798">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-799">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-799">ACR</span></span>

* <span data-ttu-id="99f85-800">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="99f85-800">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="99f85-801">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="99f85-801">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-802">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-802">ACS</span></span>

* <span data-ttu-id="99f85-803">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="99f85-803">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="99f85-804">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="99f85-804">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="99f85-805">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="99f85-805">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="99f85-806">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="99f85-806">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="99f85-807">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="99f85-807">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="99f85-808">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-808">AppService</span></span>

* <span data-ttu-id="99f85-809">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="99f85-809">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="99f85-810">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="99f85-810">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="99f85-811">Batch AI</span><span class="sxs-lookup"><span data-stu-id="99f85-811">BatchAI</span></span>

* <span data-ttu-id="99f85-812">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="99f85-812">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="99f85-813">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-813">Container</span></span>

* <span data-ttu-id="99f85-814">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="99f85-814">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="99f85-815">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="99f85-815">IoT</span></span>

* <span data-ttu-id="99f85-816">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="99f85-816">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="99f85-817">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="99f85-817">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="99f85-818">IoT Central</span><span class="sxs-lookup"><span data-stu-id="99f85-818">Iot Central</span></span>

* <span data-ttu-id="99f85-819">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="99f85-819">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="99f85-820">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="99f85-820">KeyVault</span></span>


* <span data-ttu-id="99f85-821">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="99f85-821">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="99f85-822">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="99f85-822">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="99f85-823">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="99f85-823">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="99f85-824">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="99f85-824">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="99f85-825">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="99f85-825">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="99f85-826">Передача</span><span class="sxs-lookup"><span data-stu-id="99f85-826">Relay</span></span>

* <span data-ttu-id="99f85-827">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="99f85-827">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-828">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-828">Sql</span></span>

* <span data-ttu-id="99f85-829">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="99f85-829">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-830">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-830">Storage</span></span>

* <span data-ttu-id="99f85-831">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="99f85-831">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="99f85-832">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="99f85-832">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="99f85-833">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="99f85-833">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="99f85-834">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="99f85-834">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="99f85-835">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="99f85-835">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-836">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-836">VM</span></span>

* <span data-ttu-id="99f85-837">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="99f85-837">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="99f85-838">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-838">July 31, 2018</span></span>

<span data-ttu-id="99f85-839">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="99f85-839">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-840">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-840">ACR</span></span>

* <span data-ttu-id="99f85-841">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="99f85-841">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="99f85-842">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="99f85-842">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-843">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-843">ACS</span></span>

* <span data-ttu-id="99f85-844">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="99f85-844">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="99f85-845">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-845">Batch</span></span>

* <span data-ttu-id="99f85-846">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="99f85-846">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="99f85-847">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-847">Container</span></span>

* <span data-ttu-id="99f85-848">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="99f85-848">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="99f85-849">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-849">Network</span></span>

* <span data-ttu-id="99f85-850">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="99f85-850">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="99f85-851">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-851">Resource</span></span>

* <span data-ttu-id="99f85-852">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="99f85-852">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="99f85-853">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="99f85-853">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="99f85-854">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-854">Role</span></span>

* <span data-ttu-id="99f85-855">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="99f85-855">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="99f85-856">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="99f85-856">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="99f85-857">поиска</span><span class="sxs-lookup"><span data-stu-id="99f85-857">Search</span></span>

* <span data-ttu-id="99f85-858">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="99f85-858">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="99f85-859">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-859">Service Bus</span></span>

* <span data-ttu-id="99f85-860">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="99f85-860">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="99f85-861">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="99f85-861">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="99f85-862">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="99f85-862">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="99f85-863">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="99f85-863">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-864">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-864">Storage</span></span>

* <span data-ttu-id="99f85-865">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="99f85-865">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="99f85-866">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="99f85-866">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-867">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-867">VM</span></span>

* <span data-ttu-id="99f85-868">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="99f85-868">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="99f85-869">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="99f85-869">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="99f85-870">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="99f85-870">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="99f85-871">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="99f85-871">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="99f85-872">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-872">July 18, 2018</span></span>

<span data-ttu-id="99f85-873">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="99f85-873">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="99f85-874">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-874">Core</span></span>

* <span data-ttu-id="99f85-875">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="99f85-875">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="99f85-876">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="99f85-876">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="99f85-877">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="99f85-877">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-878">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-878">ACR</span></span>

* <span data-ttu-id="99f85-879">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="99f85-879">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="99f85-880">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-880">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="99f85-881">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="99f85-881">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="99f85-882">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="99f85-882">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-883">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-883">ACS</span></span>

* <span data-ttu-id="99f85-884">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="99f85-884">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-885">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-885">AppService</span></span>

* <span data-ttu-id="99f85-886">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="99f85-886">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="99f85-887">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-887">Batch</span></span>

* <span data-ttu-id="99f85-888">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="99f85-888">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="99f85-889">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="99f85-889">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="99f85-890">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="99f85-890">Batch AI</span></span>

* <span data-ttu-id="99f85-891">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="99f85-891">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="99f85-892">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-892">Container</span></span>

* <span data-ttu-id="99f85-893">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="99f85-893">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="99f85-894">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="99f85-894">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="99f85-895">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-895">Network</span></span>

* <span data-ttu-id="99f85-896">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-896">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="99f85-897">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-897">Added `network nic wait`</span></span>
* <span data-ttu-id="99f85-898">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="99f85-898">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="99f85-899">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="99f85-899">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="99f85-900">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-900">Resource</span></span>

* <span data-ttu-id="99f85-901">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-901">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="99f85-902">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-902">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="99f85-903">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-903">Added `deployment wait` command</span></span>
* <span data-ttu-id="99f85-904">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="99f85-904">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-905">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-905">SQL</span></span>

* <span data-ttu-id="99f85-906">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-906">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="99f85-907">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="99f85-907">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="99f85-908">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="99f85-908">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-909">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-909">Storage</span></span>

* <span data-ttu-id="99f85-910">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="99f85-910">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-911">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-911">VM</span></span>

* <span data-ttu-id="99f85-912">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-912">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="99f85-913">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-913">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="99f85-914">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-914">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="99f85-915">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-915">July 3, 2018</span></span>

<span data-ttu-id="99f85-916">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="99f85-916">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="99f85-917">AKS</span><span class="sxs-lookup"><span data-stu-id="99f85-917">AKS</span></span>

* <span data-ttu-id="99f85-918">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="99f85-918">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="99f85-919">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-919">July 3, 2018</span></span>

<span data-ttu-id="99f85-920">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="99f85-920">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="99f85-921">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-921">Core</span></span>

* <span data-ttu-id="99f85-922">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="99f85-922">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-923">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-923">ACR</span></span>

* <span data-ttu-id="99f85-924">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="99f85-924">Added polling build status</span></span>
* <span data-ttu-id="99f85-925">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="99f85-925">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="99f85-926">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="99f85-926">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-927">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-927">ACS</span></span>

* <span data-ttu-id="99f85-928">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-928">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="99f85-929">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-929">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="99f85-930">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="99f85-930">Updated options for `aks browse` command.</span></span> <span data-ttu-id="99f85-931">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="99f85-931">Added `--listen-port` support</span></span>
* <span data-ttu-id="99f85-932">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="99f85-932">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="99f85-933">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="99f85-933">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="99f85-934">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="99f85-934">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-935">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-935">AppService</span></span>

* <span data-ttu-id="99f85-936">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="99f85-936">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="99f85-937">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="99f85-937">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="99f85-938">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="99f85-938">Backup</span></span>

* <span data-ttu-id="99f85-939">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="99f85-939">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="99f85-940">Batch AI</span><span class="sxs-lookup"><span data-stu-id="99f85-940">BatchAI</span></span>

* <span data-ttu-id="99f85-941">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="99f85-941">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="99f85-942">Облако</span><span class="sxs-lookup"><span data-stu-id="99f85-942">Cloud</span></span>

* <span data-ttu-id="99f85-943">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="99f85-943">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="99f85-944">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-944">Container</span></span>

* <span data-ttu-id="99f85-945">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="99f85-945">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="99f85-946">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="99f85-946">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="99f85-947">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="99f85-947">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="99f85-948">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="99f85-948">Extension</span></span>

* <span data-ttu-id="99f85-949">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="99f85-949">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="99f85-950">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-950">Network</span></span>

* <span data-ttu-id="99f85-951">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="99f85-951">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="99f85-952">Rdbms</span><span class="sxs-lookup"><span data-stu-id="99f85-952">Rdbms</span></span>

* <span data-ttu-id="99f85-953">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="99f85-953">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-954">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-954">Resource</span></span>

* <span data-ttu-id="99f85-955">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="99f85-955">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-956">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-956">VM</span></span>

* <span data-ttu-id="99f85-957">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="99f85-957">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="99f85-958">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-958">June 25, 2018</span></span>

<span data-ttu-id="99f85-959">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="99f85-959">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="99f85-960">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="99f85-960">CLI</span></span>

* <span data-ttu-id="99f85-961">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="99f85-961">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="99f85-962">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-962">June 19, 2018</span></span>

<span data-ttu-id="99f85-963">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="99f85-963">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="99f85-964">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-964">Core</span></span>

* <span data-ttu-id="99f85-965">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="99f85-965">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-966">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-966">ACR</span></span>

* <span data-ttu-id="99f85-967">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="99f85-967">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="99f85-968">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="99f85-968">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-969">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-969">ACS</span></span>

* <span data-ttu-id="99f85-970">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="99f85-970">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="99f85-971">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-971">Added `--update` support</span></span>
* <span data-ttu-id="99f85-972">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="99f85-972">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="99f85-973">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="99f85-973">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="99f85-974">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="99f85-974">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="99f85-975">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="99f85-975">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="99f85-976">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="99f85-976">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="99f85-977">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="99f85-977">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-978">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-978">AppService</span></span>

* <span data-ttu-id="99f85-979">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="99f85-979">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="99f85-980">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="99f85-980">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="99f85-981">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-981">Batch</span></span>

* <span data-ttu-id="99f85-982">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="99f85-982">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="99f85-983">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="99f85-983">Batch AI</span></span>

* <span data-ttu-id="99f85-984">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="99f85-984">Added support for workspaces.</span></span> <span data-ttu-id="99f85-985">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="99f85-985">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="99f85-986">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="99f85-986">Added support for experiments.</span></span> <span data-ttu-id="99f85-987">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="99f85-987">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="99f85-988">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="99f85-988">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="99f85-989">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="99f85-989">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="99f85-990">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="99f85-990">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="99f85-991">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="99f85-991">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="99f85-992">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="99f85-992">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="99f85-993">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="99f85-993">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="99f85-994">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-994">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="99f85-995">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="99f85-995">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="99f85-996">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-996">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="99f85-997">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="99f85-997">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="99f85-998">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="99f85-998">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="99f85-999">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="99f85-999">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="99f85-1000">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1000">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="99f85-1001">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="99f85-1001">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="99f85-1002">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="99f85-1002">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="99f85-1003">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="99f85-1003">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="99f85-1004">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="99f85-1004">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="99f85-1005">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="99f85-1005">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="99f85-1006">Карты</span><span class="sxs-lookup"><span data-stu-id="99f85-1006">Maps</span></span>

* <span data-ttu-id="99f85-1007">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1007">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1008">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1008">Network</span></span>

* <span data-ttu-id="99f85-1009">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="99f85-1009">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="99f85-1010">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="99f85-1010">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="99f85-1011">#6502</span><span class="sxs-lookup"><span data-stu-id="99f85-1011">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="99f85-1012">Резервирование</span><span class="sxs-lookup"><span data-stu-id="99f85-1012">Reservations</span></span>

* <span data-ttu-id="99f85-1013">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1013">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="99f85-1014">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1014">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="99f85-1015">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1015">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="99f85-1016">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1016">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="99f85-1017">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1017">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="99f85-1018">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1018">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="99f85-1019">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-1019">Role</span></span>

* <span data-ttu-id="99f85-1020">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="99f85-1020">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-1021">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-1021">SQL</span></span>

* <span data-ttu-id="99f85-1022">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="99f85-1022">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1023">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1023">Storage</span></span>

* <span data-ttu-id="99f85-1024">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="99f85-1024">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1025">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1025">VM</span></span>

* <span data-ttu-id="99f85-1026">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1026">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="99f85-1027">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1027">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="99f85-1028">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="99f85-1028">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="99f85-1029">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1029">June 13, 2018</span></span>

<span data-ttu-id="99f85-1030">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="99f85-1030">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1031">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1031">Core</span></span>

* <span data-ttu-id="99f85-1032">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="99f85-1032">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="99f85-1033">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1033">June 13, 2018</span></span>

<span data-ttu-id="99f85-1034">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="99f85-1034">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="99f85-1035">AKS</span><span class="sxs-lookup"><span data-stu-id="99f85-1035">AKS</span></span>

* <span data-ttu-id="99f85-1036">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="99f85-1036">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="99f85-1037">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="99f85-1037">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="99f85-1038">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="99f85-1038">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="99f85-1039">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="99f85-1039">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="99f85-1040">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="99f85-1040">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1041">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-1041">AppService</span></span>

* <span data-ttu-id="99f85-1042">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="99f85-1042">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="99f85-1043">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1043">June 5, 2018</span></span>

<span data-ttu-id="99f85-1044">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="99f85-1044">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-1045">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-1045">Interactive</span></span>

* <span data-ttu-id="99f85-1046">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="99f85-1046">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="99f85-1047">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1047">June 5, 2018</span></span>

<span data-ttu-id="99f85-1048">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="99f85-1048">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1049">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1049">Core</span></span>

* <span data-ttu-id="99f85-1050">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="99f85-1050">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="99f85-1051">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="99f85-1051">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-1052">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-1052">ACR</span></span>

* <span data-ttu-id="99f85-1053">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="99f85-1053">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="99f85-1054">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1054">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="99f85-1055">AKS</span><span class="sxs-lookup"><span data-stu-id="99f85-1055">AKS</span></span>

* <span data-ttu-id="99f85-1056">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="99f85-1056">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="99f85-1057">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-1057">Batch</span></span>

* <span data-ttu-id="99f85-1058">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="99f85-1058">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="99f85-1059">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="99f85-1059">IOT</span></span>

* <span data-ttu-id="99f85-1060">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="99f85-1060">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1061">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1061">Network</span></span>

* <span data-ttu-id="99f85-1062">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1062">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="99f85-1063">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="99f85-1063">Policy Insights</span></span>

* <span data-ttu-id="99f85-1064">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="99f85-1064">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="99f85-1065">ARM</span><span class="sxs-lookup"><span data-stu-id="99f85-1065">ARM</span></span>

* <span data-ttu-id="99f85-1066">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1066">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-1067">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-1067">SQL</span></span>

* <span data-ttu-id="99f85-1068">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="99f85-1068">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="99f85-1069">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="99f85-1069">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="99f85-1070">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1070">Storage</span></span>

* <span data-ttu-id="99f85-1071">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1071">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1072">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1072">VM</span></span>

* <span data-ttu-id="99f85-1073">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1073">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="99f85-1074">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1074">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="99f85-1075">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1075">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="99f85-1076">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1076">May 22, 2018</span></span>

<span data-ttu-id="99f85-1077">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="99f85-1077">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1078">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1078">Core</span></span>

* <span data-ttu-id="99f85-1079">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1079">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1080">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1080">ACS</span></span>

* <span data-ttu-id="99f85-1081">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1081">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="99f85-1082">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="99f85-1082">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1083">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-1083">AppService</span></span>

* <span data-ttu-id="99f85-1084">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="99f85-1084">Improved generic update commands</span></span>
* <span data-ttu-id="99f85-1085">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1085">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="99f85-1086">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-1086">Container</span></span>

* <span data-ttu-id="99f85-1087">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="99f85-1087">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="99f85-1088">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1088">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="99f85-1089">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="99f85-1089">Extension</span></span>

* <span data-ttu-id="99f85-1090">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="99f85-1090">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-1091">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-1091">Interactive</span></span>

* <span data-ttu-id="99f85-1092">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="99f85-1092">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="99f85-1093">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="99f85-1093">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="99f85-1094">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="99f85-1094">KeyVault</span></span>

* <span data-ttu-id="99f85-1095">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="99f85-1095">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1096">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1096">Network</span></span>

* <span data-ttu-id="99f85-1097">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="99f85-1097">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="99f85-1098">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="99f85-1098">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-1099">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-1099">SQL</span></span>

* <span data-ttu-id="99f85-1100">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="99f85-1100">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="99f85-1101">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1101">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="99f85-1102">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1102">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="99f85-1103">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="99f85-1103">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="99f85-1104">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="99f85-1104">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="99f85-1105">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1105">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="99f85-1106">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1106">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="99f85-1107">`edition`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1107">`edition`.</span></span> <span data-ttu-id="99f85-1108">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1108">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="99f85-1109">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1109">`elasticPoolName`.</span></span> <span data-ttu-id="99f85-1110">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1110">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="99f85-1111">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="99f85-1111">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="99f85-1112">`edition`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1112">`edition`.</span></span> <span data-ttu-id="99f85-1113">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1113">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="99f85-1114">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1114">`dtu`.</span></span> <span data-ttu-id="99f85-1115">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1115">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="99f85-1116">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1116">`databaseDtuMin`.</span></span> <span data-ttu-id="99f85-1117">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1117">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="99f85-1118">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1118">`databaseDtuMax`.</span></span> <span data-ttu-id="99f85-1119">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1119">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="99f85-1120">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1120">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="99f85-1121">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1121">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1122">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1122">Storage</span></span>

* <span data-ttu-id="99f85-1123">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1123">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="99f85-1124">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1124">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1125">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1125">VM</span></span>

* <span data-ttu-id="99f85-1126">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1126">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="99f85-1127">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1127">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="99f85-1128">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1128">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="99f85-1129">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="99f85-1129">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="99f85-1130">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1130">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="99f85-1131">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1131">May 7, 2018</span></span>

<span data-ttu-id="99f85-1132">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="99f85-1132">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1133">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1133">Core</span></span>

* <span data-ttu-id="99f85-1134">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="99f85-1134">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="99f85-1135">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1135">Added limited support for positional arguments</span></span>
* <span data-ttu-id="99f85-1136">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1136">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="99f85-1137">#5591</span><span class="sxs-lookup"><span data-stu-id="99f85-1137">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="99f85-1138">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1138">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="99f85-1139">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="99f85-1139">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="99f85-1140">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="99f85-1140">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="99f85-1141">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1141">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="99f85-1142">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="99f85-1142">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-1143">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-1143">ACR</span></span>

* <span data-ttu-id="99f85-1144">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="99f85-1144">Added ACR Build commands</span></span>
* <span data-ttu-id="99f85-1145">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="99f85-1145">Improved resource not found error messages</span></span>
* <span data-ttu-id="99f85-1146">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="99f85-1146">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="99f85-1147">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="99f85-1147">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="99f85-1148">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="99f85-1148">Improved repository commands error messages</span></span>
* <span data-ttu-id="99f85-1149">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="99f85-1149">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1150">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1150">ACS</span></span>

* <span data-ttu-id="99f85-1151">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-1151">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="99f85-1152">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="99f85-1152">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="99f85-1153">AMS</span><span class="sxs-lookup"><span data-stu-id="99f85-1153">AMS</span></span>

* <span data-ttu-id="99f85-1154">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="99f85-1154">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1155">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1155">Appservice</span></span>

* <span data-ttu-id="99f85-1156">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="99f85-1156">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="99f85-1157">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1157">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="99f85-1158">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="99f85-1158">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="99f85-1159">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1159">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="99f85-1160">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="99f85-1160">Batch AI</span></span>

* <span data-ttu-id="99f85-1161">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="99f85-1161">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="99f85-1162">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="99f85-1162">Cognitive Services</span></span>

* <span data-ttu-id="99f85-1163">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="99f85-1163">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="99f85-1164">Потребление</span><span class="sxs-lookup"><span data-stu-id="99f85-1164">Consumption</span></span>

* <span data-ttu-id="99f85-1165">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="99f85-1165">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="99f85-1166">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-1166">Container</span></span>

* <span data-ttu-id="99f85-1167">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="99f85-1167">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="99f85-1168">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="99f85-1168">Cosmos DB</span></span>

* <span data-ttu-id="99f85-1169">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="99f85-1169">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="99f85-1170">DMS</span><span class="sxs-lookup"><span data-stu-id="99f85-1170">DMS</span></span>

* <span data-ttu-id="99f85-1171">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="99f85-1171">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="99f85-1172">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="99f85-1172">Extension</span></span>

* <span data-ttu-id="99f85-1173">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="99f85-1173">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-1174">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-1174">Interactive</span></span>

* <span data-ttu-id="99f85-1175">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="99f85-1175">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="99f85-1176">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="99f85-1176">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="99f85-1177">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="99f85-1177">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="99f85-1178">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="99f85-1178">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="99f85-1179">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="99f85-1179">Lab</span></span>

* <span data-ttu-id="99f85-1180">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="99f85-1180">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1181">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1181">Network</span></span>

* <span data-ttu-id="99f85-1182">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="99f85-1182">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="99f85-1183">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-1183">Profile</span></span>

* <span data-ttu-id="99f85-1184">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1184">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="99f85-1185">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="99f85-1185">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="99f85-1186">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1186">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="99f85-1187">Redis</span><span class="sxs-lookup"><span data-stu-id="99f85-1187">Redis</span></span>

* <span data-ttu-id="99f85-1188">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1188">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="99f85-1189">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="99f85-1189">Deprecated `redis list-all`.</span></span> <span data-ttu-id="99f85-1190">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1190">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="99f85-1191">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1191">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="99f85-1192">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="99f85-1192">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="99f85-1193">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-1193">Role</span></span>

* <span data-ttu-id="99f85-1194">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="99f85-1194">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1195">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1195">Storage</span></span>

* <span data-ttu-id="99f85-1196">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="99f85-1196">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="99f85-1197">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="99f85-1197">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="99f85-1198">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="99f85-1198">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="99f85-1199">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="99f85-1199">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="99f85-1200">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="99f85-1200">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1201">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1201">VM</span></span>

* <span data-ttu-id="99f85-1202">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="99f85-1202">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="99f85-1203">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="99f85-1203">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="99f85-1204">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="99f85-1204">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="99f85-1205">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1205">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="99f85-1206">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="99f85-1206">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="99f85-1207">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="99f85-1207">Added write accelerator support</span></span>
* <span data-ttu-id="99f85-1208">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1208">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="99f85-1209">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="99f85-1209">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="99f85-1210">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="99f85-1210">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="99f85-1211">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1211">April 10, 2018</span></span>

<span data-ttu-id="99f85-1212">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="99f85-1212">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-1213">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-1213">ACR</span></span>

* <span data-ttu-id="99f85-1214">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="99f85-1214">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1215">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1215">ACS</span></span>

* <span data-ttu-id="99f85-1216">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="99f85-1216">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1217">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1217">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="99f85-1219">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="99f85-1219">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="99f85-1220">Batch AI</span><span class="sxs-lookup"><span data-stu-id="99f85-1220">BatchAI</span></span>

* <span data-ttu-id="99f85-1221">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="99f85-1221">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="99f85-1222">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="99f85-1222">Job level mounting</span></span>
  - <span data-ttu-id="99f85-1223">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1223">Environment variables with secret values</span></span>
  - <span data-ttu-id="99f85-1224">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="99f85-1224">Performance counters settings</span></span>
  - <span data-ttu-id="99f85-1225">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="99f85-1225">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="99f85-1226">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1226">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="99f85-1227">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="99f85-1227">Usage and limits reporting</span></span>
  - <span data-ttu-id="99f85-1228">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1228">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="99f85-1229">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1229">Support for custom images</span></span>
  - <span data-ttu-id="99f85-1230">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="99f85-1230">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="99f85-1231">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="99f85-1231">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="99f85-1232">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1232">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="99f85-1233">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="99f85-1233">National clouds are supported</span></span>
* <span data-ttu-id="99f85-1234">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="99f85-1234">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="99f85-1235">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="99f85-1235">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="99f85-1236">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="99f85-1236">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="99f85-1237">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="99f85-1237">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="99f85-1238">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="99f85-1238">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="99f85-1239">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="99f85-1239">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="99f85-1240">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1240">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="99f85-1241">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="99f85-1241">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="99f85-1242">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="99f85-1242">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="99f85-1243">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1243">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="99f85-1244">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="99f85-1244">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="99f85-1245">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1245">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="99f85-1246">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1246">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="99f85-1247">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="99f85-1247">Billing</span></span>

* <span data-ttu-id="99f85-1248">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="99f85-1248">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="99f85-1249">Потребление</span><span class="sxs-lookup"><span data-stu-id="99f85-1249">Consumption</span></span>

* <span data-ttu-id="99f85-1250">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1250">Added `marketplace` commands</span></span>
* <span data-ttu-id="99f85-1251">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1251">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="99f85-1252">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1252">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="99f85-1253">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1253">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="99f85-1254">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1254">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="99f85-1255">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1255">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="99f85-1256">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-1256">Container</span></span>

* <span data-ttu-id="99f85-1257">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1257">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="99f85-1258">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="99f85-1258">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="99f85-1259">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="99f85-1259">Extension</span></span>

* <span data-ttu-id="99f85-1260">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="99f85-1260">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-1261">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-1261">Interactive</span></span>

* <span data-ttu-id="99f85-1262">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="99f85-1262">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="99f85-1263">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="99f85-1263">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="99f85-1264">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1264">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1265">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1265">Network</span></span>

* <span data-ttu-id="99f85-1266">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1266">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="99f85-1267">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1267">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="99f85-1268">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="99f85-1268">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="99f85-1269">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="99f85-1269">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="99f85-1270">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="99f85-1270">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="99f85-1271">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1271">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="99f85-1272">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1272">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="99f85-1273">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="99f85-1273">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="99f85-1274">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-1274">Profile</span></span>

* <span data-ttu-id="99f85-1275">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1275">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="99f85-1276">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1276">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="99f85-1277">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="99f85-1277">RDBMS</span></span>

* <span data-ttu-id="99f85-1278">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1278">Added `georestore` command</span></span>
* <span data-ttu-id="99f85-1279">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="99f85-1279">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-1280">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-1280">Resource</span></span>

* <span data-ttu-id="99f85-1281">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1281">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="99f85-1282">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1282">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-1283">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-1283">SQL</span></span>

* <span data-ttu-id="99f85-1284">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1284">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1285">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1285">Storage</span></span>

* <span data-ttu-id="99f85-1286">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="99f85-1286">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1287">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1287">VM</span></span>

* <span data-ttu-id="99f85-1288">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="99f85-1288">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="99f85-1289">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="99f85-1289">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="99f85-1291">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1291">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="99f85-1292">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="99f85-1292">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="99f85-1293">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="99f85-1293">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="99f85-1294">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="99f85-1294">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="99f85-1295">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1295">March 27, 2018</span></span>

<span data-ttu-id="99f85-1296">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="99f85-1296">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1297">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1297">Core</span></span>

* <span data-ttu-id="99f85-1298">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="99f85-1298">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1299">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1299">ACS</span></span>

* <span data-ttu-id="99f85-1300">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="99f85-1300">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1301">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1301">Appservice</span></span>

* <span data-ttu-id="99f85-1302">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1302">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="99f85-1303">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1303">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="99f85-1304">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="99f85-1304">Backup</span></span>

* <span data-ttu-id="99f85-1305">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1305">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="99f85-1306">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="99f85-1306">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="99f85-1307">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="99f85-1307">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="99f85-1308">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1308">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="99f85-1309">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-1309">Container</span></span>

* <span data-ttu-id="99f85-1310">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1310">Added `container exec` command.</span></span> <span data-ttu-id="99f85-1311">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1311">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="99f85-1312">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1312">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="99f85-1313">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="99f85-1313">Extension</span></span>

* <span data-ttu-id="99f85-1314">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="99f85-1314">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="99f85-1315">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1315">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="99f85-1316">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-1316">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-1317">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-1317">Interactive</span></span>

* <span data-ttu-id="99f85-1318">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="99f85-1318">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="99f85-1319">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1319">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="99f85-1320">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="99f85-1320">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="99f85-1321">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="99f85-1321">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="99f85-1322">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="99f85-1322">Lab</span></span>

* <span data-ttu-id="99f85-1323">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1323">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-1324">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-1324">Monitor</span></span>

* <span data-ttu-id="99f85-1325">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="99f85-1325">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="99f85-1326">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="99f85-1326">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="99f85-1327">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="99f85-1327">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1328">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1328">Network</span></span>

* <span data-ttu-id="99f85-1329">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="99f85-1329">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="99f85-1330">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-1330">Profile</span></span>

* <span data-ttu-id="99f85-1331">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1331">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="99f85-1332">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="99f85-1332">RDBMS</span></span>

* <span data-ttu-id="99f85-1333">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="99f85-1333">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-1334">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-1334">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="99f85-1336">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-1336">Role</span></span>

* <span data-ttu-id="99f85-1337">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1337">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="99f85-1338">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="99f85-1338">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="99f85-1339">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="99f85-1339">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="99f85-1340">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1340">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="99f85-1341">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1341">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1342">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1342">Storage</span></span>

* <span data-ttu-id="99f85-1343">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="99f85-1343">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="99f85-1344">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="99f85-1344">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1345">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1345">VM</span></span>

* <span data-ttu-id="99f85-1346">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1346">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="99f85-1347">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1347">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="99f85-1348">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="99f85-1348">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="99f85-1349">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="99f85-1349">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="99f85-1350">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1350">March 13, 2018</span></span>

<span data-ttu-id="99f85-1351">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="99f85-1351">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-1352">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-1352">ACR</span></span>

* <span data-ttu-id="99f85-1353">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1353">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="99f85-1354">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="99f85-1354">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="99f85-1355">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="99f85-1355">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1356">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1356">ACS</span></span>

* <span data-ttu-id="99f85-1357">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="99f85-1357">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="99f85-1358">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="99f85-1358">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="99f85-1359">Помощник</span><span class="sxs-lookup"><span data-stu-id="99f85-1359">Advisor</span></span>

* <span data-ttu-id="99f85-1360">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1360">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="99f85-1361">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1361">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="99f85-1362">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1362">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="99f85-1363">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1363">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="99f85-1364">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1364">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1365">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1365">Appservice</span></span>

* <span data-ttu-id="99f85-1366">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="99f85-1366">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="99f85-1367">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1367">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="99f85-1368">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="99f85-1368">Eventhubs</span></span>

* <span data-ttu-id="99f85-1369">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="99f85-1369">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="99f85-1370">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="99f85-1370">Extension</span></span>

* <span data-ttu-id="99f85-1371">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="99f85-1371">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-1372">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-1372">Interactive</span></span>

* <span data-ttu-id="99f85-1373">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="99f85-1373">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="99f85-1374">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="99f85-1374">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="99f85-1375">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="99f85-1375">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="99f85-1376">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="99f85-1376">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-1377">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-1377">Monitor</span></span>

* <span data-ttu-id="99f85-1378">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="99f85-1378">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="99f85-1379">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1379">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="99f85-1380">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1380">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="99f85-1381">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1381">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1382">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1382">Network</span></span>

* <span data-ttu-id="99f85-1383">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1383">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="99f85-1384">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="99f85-1384">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="99f85-1385">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1385">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="99f85-1386">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1386">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="99f85-1387">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-1387">Profile</span></span>

* <span data-ttu-id="99f85-1388">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="99f85-1388">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="99f85-1389">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1389">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="99f85-1390">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="99f85-1390">RDBMS</span></span>

* <span data-ttu-id="99f85-1391">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="99f85-1391">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="99f85-1392">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-1392">Service Bus</span></span>

* <span data-ttu-id="99f85-1393">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="99f85-1393">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1394">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1394">Storage</span></span>

* <span data-ttu-id="99f85-1395">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="99f85-1395">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="99f85-1396">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="99f85-1396">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1397">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1397">VM</span></span>

* <span data-ttu-id="99f85-1398">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="99f85-1398">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="99f85-1399">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="99f85-1399">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="99f85-1400">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1400">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="99f85-1401">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="99f85-1401">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="99f85-1402">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="99f85-1402">February 27, 2018</span></span>

<span data-ttu-id="99f85-1403">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="99f85-1403">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1404">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1404">Core</span></span>

* <span data-ttu-id="99f85-1405">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="99f85-1405">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="99f85-1406">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="99f85-1406">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="99f85-1407">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1407">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1408">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1408">ACS</span></span>

* <span data-ttu-id="99f85-1409">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-1409">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="99f85-1410">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="99f85-1410">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="99f85-1411">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1411">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="99f85-1412">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1412">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1413">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1413">Appservice</span></span>

* <span data-ttu-id="99f85-1414">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="99f85-1414">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="99f85-1415">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="99f85-1415">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="99f85-1416">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="99f85-1416">Cognitive Services</span></span>

* <span data-ttu-id="99f85-1417">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="99f85-1417">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="99f85-1418">Потребление</span><span class="sxs-lookup"><span data-stu-id="99f85-1418">Consumption</span></span>

* <span data-ttu-id="99f85-1419">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="99f85-1419">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="99f85-1420">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="99f85-1420">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="99f85-1421">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-1421">Container</span></span>

* <span data-ttu-id="99f85-1422">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="99f85-1422">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1423">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1423">Network</span></span>

* <span data-ttu-id="99f85-1424">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1424">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-1425">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-1425">Resource</span></span>

* <span data-ttu-id="99f85-1426">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="99f85-1426">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="99f85-1427">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-1427">Role</span></span>

* <span data-ttu-id="99f85-1428">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-1428">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-1429">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-1429">SQL</span></span>

* <span data-ttu-id="99f85-1430">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1430">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1431">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1431">Storage</span></span>

* <span data-ttu-id="99f85-1432">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1432">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1433">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1433">VM</span></span>

* <span data-ttu-id="99f85-1434">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="99f85-1434">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="99f85-1435">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1435">February 13, 2018</span></span>

<span data-ttu-id="99f85-1436">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="99f85-1436">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1437">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1437">Core</span></span>

* <span data-ttu-id="99f85-1438">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="99f85-1438">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1439">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1439">ACS</span></span>

* <span data-ttu-id="99f85-1440">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="99f85-1440">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="99f85-1441">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1441">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="99f85-1442">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="99f85-1442">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="99f85-1443">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="99f85-1443">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="99f85-1444">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="99f85-1444">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="99f85-1445">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1445">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="99f85-1446">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="99f85-1446">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="99f85-1447">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1447">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1448">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1448">Appservice</span></span>

* <span data-ttu-id="99f85-1449">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="99f85-1449">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="99f85-1450">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1450">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="99f85-1451">CDN</span><span class="sxs-lookup"><span data-stu-id="99f85-1451">CDN</span></span>

* <span data-ttu-id="99f85-1452">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1452">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="99f85-1453">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-1453">Container</span></span>

* <span data-ttu-id="99f85-1454">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="99f85-1454">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="99f85-1455">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1455">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="99f85-1456">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="99f85-1456">CosmosDB</span></span>

* <span data-ttu-id="99f85-1457">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1457">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="99f85-1458">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="99f85-1458">Extension</span></span>

* <span data-ttu-id="99f85-1459">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1459">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="99f85-1460">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1460">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="99f85-1461">Отзыв</span><span class="sxs-lookup"><span data-stu-id="99f85-1461">Feedback</span></span>

* <span data-ttu-id="99f85-1462">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="99f85-1462">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-1463">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-1463">Interactive</span></span>

* <span data-ttu-id="99f85-1464">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="99f85-1464">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="99f85-1465">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1465">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="99f85-1466">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="99f85-1466">IoT</span></span>

* <span data-ttu-id="99f85-1467">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="99f85-1467">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="99f85-1468">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="99f85-1468">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="99f85-1469">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1469">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="99f85-1470">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="99f85-1470">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-1471">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-1471">Monitor</span></span>

* <span data-ttu-id="99f85-1472">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1472">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1473">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1473">Network</span></span>

* <span data-ttu-id="99f85-1474">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="99f85-1474">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="99f85-1475">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-1475">Profile</span></span>

* <span data-ttu-id="99f85-1476">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="99f85-1476">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-1477">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-1477">Resource</span></span>

* <span data-ttu-id="99f85-1478">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1478">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="99f85-1479">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-1479">Role</span></span>

* <span data-ttu-id="99f85-1480">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="99f85-1480">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-1481">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-1481">SQL</span></span>

* <span data-ttu-id="99f85-1482">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1482">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="99f85-1483">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1483">Added `sql db rename`</span></span>
* <span data-ttu-id="99f85-1484">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="99f85-1484">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1485">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1485">Storage</span></span>

* <span data-ttu-id="99f85-1486">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="99f85-1486">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1487">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1487">VM</span></span>

* <span data-ttu-id="99f85-1488">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="99f85-1488">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="99f85-1489">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="99f85-1489">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="99f85-1490">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="99f85-1490">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="99f85-1491">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1491">January 31, 2018</span></span>

<span data-ttu-id="99f85-1492">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="99f85-1492">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1493">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1493">Core</span></span>

* <span data-ttu-id="99f85-1494">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="99f85-1494">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="99f85-1495">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="99f85-1495">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="99f85-1496">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="99f85-1496">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="99f85-1497">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="99f85-1497">Use `--verbose` to see</span></span>
* <span data-ttu-id="99f85-1498">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="99f85-1498">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1499">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1499">ACS</span></span>

* <span data-ttu-id="99f85-1500">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1500">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="99f85-1501">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1501">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1502">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1502">Appservice</span></span>

* <span data-ttu-id="99f85-1503">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="99f85-1503">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="99f85-1504">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="99f85-1504">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="99f85-1505">CDN</span><span class="sxs-lookup"><span data-stu-id="99f85-1505">CDN</span></span>

* <span data-ttu-id="99f85-1506">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1506">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="99f85-1507">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="99f85-1507">CosmosDB</span></span>

* <span data-ttu-id="99f85-1508">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="99f85-1508">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-1509">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-1509">Interactive</span></span>

* <span data-ttu-id="99f85-1510">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="99f85-1510">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1511">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1511">Network</span></span>

* <span data-ttu-id="99f85-1512">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1512">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="99f85-1513">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-1513">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="99f85-1514">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1514">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="99f85-1515">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1515">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="99f85-1516">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1516">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="99f85-1517">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="99f85-1517">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="99f85-1518">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="99f85-1518">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="99f85-1519">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="99f85-1519">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="99f85-1520">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1520">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="99f85-1521">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1521">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="99f85-1522">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-1522">Profile</span></span>

* <span data-ttu-id="99f85-1523">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="99f85-1523">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-1524">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-1524">Resource</span></span>

* <span data-ttu-id="99f85-1525">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="99f85-1525">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1526">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1526">Storage</span></span>

* <span data-ttu-id="99f85-1527">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="99f85-1527">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="99f85-1528">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="99f85-1528">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="99f85-1529">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1529">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="99f85-1530">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1530">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="99f85-1531">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="99f85-1531">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1532">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1532">VM</span></span>

* <span data-ttu-id="99f85-1533">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="99f85-1533">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="99f85-1534">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1534">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="99f85-1535">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="99f85-1535">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="99f85-1536">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1536">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="99f85-1537">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1537">January 17, 2018</span></span>

<span data-ttu-id="99f85-1538">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="99f85-1538">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-1539">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-1539">ACR</span></span>

* <span data-ttu-id="99f85-1540">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="99f85-1540">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="99f85-1541">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="99f85-1541">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1542">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1542">ACS</span></span>

* <span data-ttu-id="99f85-1543">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1543">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="99f85-1544">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-1544">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1545">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1545">Appservice</span></span>

* <span data-ttu-id="99f85-1546">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="99f85-1546">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="99f85-1547">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1547">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="99f85-1548">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1548">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="99f85-1549">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="99f85-1549">Backup</span></span>

* <span data-ttu-id="99f85-1550">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="99f85-1550">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="99f85-1551">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="99f85-1551">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="99f85-1552">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="99f85-1552">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="99f85-1553">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="99f85-1553">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="99f85-1554">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="99f85-1554">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="99f85-1555">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-1555">Batch</span></span>

* <span data-ttu-id="99f85-1556">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="99f85-1556">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="99f85-1557">Облако</span><span class="sxs-lookup"><span data-stu-id="99f85-1557">Cloud</span></span>

* <span data-ttu-id="99f85-1558">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="99f85-1558">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="99f85-1559">Потребление</span><span class="sxs-lookup"><span data-stu-id="99f85-1559">Consumption</span></span>

* <span data-ttu-id="99f85-1560">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1560">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="99f85-1561">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-1561">Event Grid</span></span>

* <span data-ttu-id="99f85-1562">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1562">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="99f85-1563">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1563">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="99f85-1564">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1564">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="99f85-1565">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1565">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="99f85-1566">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1566">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="99f85-1567">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1567">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="99f85-1568">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1568">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="99f85-1569">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1569">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-1570">Interactive</span><span class="sxs-lookup"><span data-stu-id="99f85-1570">Interactive</span></span>

* <span data-ttu-id="99f85-1571">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="99f85-1571">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="99f85-1572">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="99f85-1572">Fixed errors on startup</span></span>
* <span data-ttu-id="99f85-1573">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="99f85-1573">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="99f85-1574">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="99f85-1574">IoT</span></span>

* <span data-ttu-id="99f85-1575">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="99f85-1575">Added support for device provisioning service</span></span>
* <span data-ttu-id="99f85-1576">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="99f85-1576">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="99f85-1577">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="99f85-1577">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-1578">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-1578">Monitor</span></span>

* <span data-ttu-id="99f85-1579">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="99f85-1579">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="99f85-1580">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1580">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="99f85-1581">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="99f85-1581">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1582">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1582">Network</span></span>

* <span data-ttu-id="99f85-1583">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="99f85-1583">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="99f85-1584">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="99f85-1584">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="99f85-1585">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-1585">Profile</span></span>

* <span data-ttu-id="99f85-1586">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="99f85-1586">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="99f85-1587">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-1587">Role</span></span>

* <span data-ttu-id="99f85-1588">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1588">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="99f85-1589">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="99f85-1589">Service Fabric</span></span>

* <span data-ttu-id="99f85-1590">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="99f85-1590">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="99f85-1591">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="99f85-1591">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1592">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1592">VM</span></span>

* <span data-ttu-id="99f85-1593">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1593">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="99f85-1594">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="99f85-1594">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="99f85-1595">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1595">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="99f85-1596">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="99f85-1596">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="99f85-1597">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="99f85-1597">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="99f85-1598">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1598">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="99f85-1599">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1599">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="99f85-1600">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1600">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="99f85-1601">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1601">December 19, 2017</span></span>

<span data-ttu-id="99f85-1602">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="99f85-1602">Version 2.0.23</span></span>

* <span data-ttu-id="99f85-1603">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="99f85-1603">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="99f85-1604">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-1604">Container</span></span>

* <span data-ttu-id="99f85-1605">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1605">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1606">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1606">Network</span></span>

* <span data-ttu-id="99f85-1607">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="99f85-1607">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="99f85-1608">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="99f85-1608">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1609">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1609">Storage</span></span>

* <span data-ttu-id="99f85-1610">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="99f85-1610">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1611">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1611">VM</span></span>

* <span data-ttu-id="99f85-1612">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="99f85-1612">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="99f85-1613">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1613">December 5, 2017</span></span>

<span data-ttu-id="99f85-1614">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="99f85-1614">Version 2.0.22</span></span>

* <span data-ttu-id="99f85-1615">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1615">Removed `az component` commands.</span></span> <span data-ttu-id="99f85-1616">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1616">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1617">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1617">Core</span></span>
* <span data-ttu-id="99f85-1618">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="99f85-1618">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="99f85-1619">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="99f85-1619">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1620">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1620">ACS</span></span>

* <span data-ttu-id="99f85-1621">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1621">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="99f85-1622">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1622">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="99f85-1623">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="99f85-1623">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="99f85-1624">Помощник</span><span class="sxs-lookup"><span data-stu-id="99f85-1624">Advisor</span></span>

* <span data-ttu-id="99f85-1625">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="99f85-1625">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1626">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1626">Appservice</span></span>

* <span data-ttu-id="99f85-1627">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1627">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="99f85-1628">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="99f85-1628">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="99f85-1629">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1629">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="99f85-1630">Потребление</span><span class="sxs-lookup"><span data-stu-id="99f85-1630">Consumption</span></span>

* <span data-ttu-id="99f85-1631">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="99f85-1631">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="99f85-1632">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-1632">Container</span></span>

* <span data-ttu-id="99f85-1633">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="99f85-1633">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-1634">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-1634">Monitor</span></span>

* <span data-ttu-id="99f85-1635">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="99f85-1635">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-1636">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-1636">Resource</span></span>

* <span data-ttu-id="99f85-1637">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="99f85-1637">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="99f85-1638">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-1638">Role</span></span>

* <span data-ttu-id="99f85-1639">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1639">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="99f85-1640">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="99f85-1640">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="99f85-1641">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1641">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-1642">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-1642">SQL</span></span>

* <span data-ttu-id="99f85-1643">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1643">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="99f85-1644">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1644">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1645">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1645">VM</span></span>

* <span data-ttu-id="99f85-1646">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1646">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="99f85-1647">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1647">November 14, 2017</span></span>

<span data-ttu-id="99f85-1648">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="99f85-1648">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-1649">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-1649">ACR</span></span>

* <span data-ttu-id="99f85-1650">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="99f85-1650">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="99f85-1651">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1651">ACS</span></span>

* <span data-ttu-id="99f85-1652">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="99f85-1652">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="99f85-1653">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="99f85-1653">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="99f85-1654">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1654">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="99f85-1655">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="99f85-1655">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="99f85-1656">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="99f85-1656">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1657">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1657">Appservice</span></span>

* <span data-ttu-id="99f85-1658">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="99f85-1658">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="99f85-1659">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1659">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="99f85-1660">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1660">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="99f85-1661">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1661">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="99f85-1662">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="99f85-1662">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="99f85-1663">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="99f85-1663">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="99f85-1664">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-1664">Batch</span></span>

* <span data-ttu-id="99f85-1665">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1665">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="99f85-1666">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="99f85-1666">Batchai</span></span>

* <span data-ttu-id="99f85-1667">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1667">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="99f85-1668">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1668">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="99f85-1669">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1669">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="99f85-1670">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1670">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="99f85-1671">Облако</span><span class="sxs-lookup"><span data-stu-id="99f85-1671">Cloud</span></span>

* <span data-ttu-id="99f85-1672">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="99f85-1672">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="99f85-1673">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-1673">Container</span></span>

* <span data-ttu-id="99f85-1674">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1674">Added support to open multiple ports</span></span>
* <span data-ttu-id="99f85-1675">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1675">Added container group restart policy</span></span>
* <span data-ttu-id="99f85-1676">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="99f85-1676">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="99f85-1677">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="99f85-1677">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="99f85-1678">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="99f85-1678">Data Lake Analytics</span></span>

* <span data-ttu-id="99f85-1679">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="99f85-1679">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="99f85-1680">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="99f85-1680">Data Lake Store</span></span>

* <span data-ttu-id="99f85-1681">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="99f85-1681">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="99f85-1682">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="99f85-1682">Extension</span></span>

* <span data-ttu-id="99f85-1683">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="99f85-1683">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="99f85-1684">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="99f85-1684">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="99f85-1685">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="99f85-1685">IoT</span></span>

* <span data-ttu-id="99f85-1686">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1686">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-1687">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-1687">Monitor</span></span>

* <span data-ttu-id="99f85-1688">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1688">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1689">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1689">Network</span></span>

* <span data-ttu-id="99f85-1690">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="99f85-1690">Added support for CAA DNS records</span></span>
* <span data-ttu-id="99f85-1691">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1691">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="99f85-1692">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="99f85-1692">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="99f85-1693">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1693">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="99f85-1694">Резервирование</span><span class="sxs-lookup"><span data-stu-id="99f85-1694">Reservations</span></span>

* <span data-ttu-id="99f85-1695">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="99f85-1695">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-1696">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-1696">Resource</span></span>

* <span data-ttu-id="99f85-1697">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1697">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-1698">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-1698">SQL</span></span>

* <span data-ttu-id="99f85-1699">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1699">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1700">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1700">Storage</span></span>

* <span data-ttu-id="99f85-1701">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-1701">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="99f85-1702">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="99f85-1702">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="99f85-1703">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1703">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="99f85-1704">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1704">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="99f85-1705">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1705">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="99f85-1706">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1706">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="99f85-1707">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1707">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1708">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1708">VM</span></span>

* <span data-ttu-id="99f85-1709">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1709">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="99f85-1710">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1710">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="99f85-1711">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1711">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="99f85-1712">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1712">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="99f85-1713">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="99f85-1713">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="99f85-1714">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1714">October 24, 2017</span></span>

<span data-ttu-id="99f85-1715">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="99f85-1715">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1716">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1716">Core</span></span>

* <span data-ttu-id="99f85-1717">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="99f85-1717">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-1718">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-1718">ACR</span></span>

* <span data-ttu-id="99f85-1719">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="99f85-1719">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="99f85-1720">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="99f85-1720">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="99f85-1721">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="99f85-1721">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1722">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1722">ACS</span></span>

* <span data-ttu-id="99f85-1723">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="99f85-1723">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="99f85-1724">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="99f85-1724">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1725">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1725">Appservice</span></span>

* <span data-ttu-id="99f85-1726">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="99f85-1726">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="99f85-1727">Компонент</span><span class="sxs-lookup"><span data-stu-id="99f85-1727">Component</span></span>

* <span data-ttu-id="99f85-1728">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="99f85-1728">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-1729">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-1729">Monitor</span></span>

* <span data-ttu-id="99f85-1730">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1730">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-1731">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-1731">Resource</span></span>

* <span data-ttu-id="99f85-1732">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="99f85-1732">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="99f85-1733">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="99f85-1733">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1734">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1734">VM</span></span>

* <span data-ttu-id="99f85-1735">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="99f85-1735">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="99f85-1736">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1736">October 9, 2017</span></span>

<span data-ttu-id="99f85-1737">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="99f85-1737">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1738">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1738">Core</span></span>

* <span data-ttu-id="99f85-1739">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="99f85-1739">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1740">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1740">Appservice</span></span>

* <span data-ttu-id="99f85-1741">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1741">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="99f85-1742">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-1742">Batch</span></span>

* <span data-ttu-id="99f85-1743">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="99f85-1743">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="99f85-1744">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="99f85-1744">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="99f85-1745">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-1745">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="99f85-1746">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1746">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="99f85-1747">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="99f85-1747">Batchai</span></span>

* <span data-ttu-id="99f85-1748">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="99f85-1748">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="99f85-1749">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="99f85-1749">Keyvault</span></span>

* <span data-ttu-id="99f85-1750">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="99f85-1750">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="99f85-1751">(#4448)</span><span class="sxs-lookup"><span data-stu-id="99f85-1751">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="99f85-1752">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1752">Network</span></span>

* <span data-ttu-id="99f85-1753">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="99f85-1753">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="99f85-1754">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="99f85-1754">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-1755">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-1755">Resource</span></span>

* <span data-ttu-id="99f85-1756">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1756">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="99f85-1757">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="99f85-1757">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="99f85-1758">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="99f85-1758">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="99f85-1759">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="99f85-1759">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-1760">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-1760">Sql</span></span>

* <span data-ttu-id="99f85-1761">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="99f85-1761">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="99f85-1762">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="99f85-1762">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="99f85-1763">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="99f85-1763">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1764">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1764">Storage</span></span>

* <span data-ttu-id="99f85-1765">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1765">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1766">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="99f85-1766">Vm</span></span>

* <span data-ttu-id="99f85-1767">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1767">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="99f85-1768">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1768">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="99f85-1769">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1769">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="99f85-1770">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1770">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="99f85-1771">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="99f85-1771">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="99f85-1772">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1772">September 22, 2017</span></span>

<span data-ttu-id="99f85-1773">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="99f85-1773">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-1774">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-1774">Resource</span></span>

* <span data-ttu-id="99f85-1775">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="99f85-1775">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="99f85-1776">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="99f85-1776">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="99f85-1777">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="99f85-1777">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="99f85-1778">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1778">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1779">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1779">Network</span></span>

* <span data-ttu-id="99f85-1780">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="99f85-1780">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="99f85-1781">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="99f85-1781">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="99f85-1782">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="99f85-1782">Added `asg` application security group commands</span></span>
* <span data-ttu-id="99f85-1783">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="99f85-1783">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="99f85-1784">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="99f85-1784">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="99f85-1785">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="99f85-1785">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="99f85-1786">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1786">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1787">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1787">Storage</span></span>

* <span data-ttu-id="99f85-1788">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="99f85-1788">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="99f85-1789">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="99f85-1789">Eventgrid</span></span>

* <span data-ttu-id="99f85-1790">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="99f85-1790">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-1791">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-1791">SQL</span></span>

* <span data-ttu-id="99f85-1792">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="99f85-1792">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="99f85-1793">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="99f85-1793">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="99f85-1794">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="99f85-1794">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="99f85-1795">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="99f85-1795">Keyvault</span></span>

* <span data-ttu-id="99f85-1796">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="99f85-1796">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1797">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1797">VM</span></span>

* <span data-ttu-id="99f85-1798">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="99f85-1798">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="99f85-1799">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="99f85-1799">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="99f85-1800">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="99f85-1800">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="99f85-1801">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="99f85-1801">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="99f85-1802">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="99f85-1802">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="99f85-1803">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="99f85-1803">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1804">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1804">ACS</span></span>

* <span data-ttu-id="99f85-1805">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="99f85-1805">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1806">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1806">Appservice</span></span>

* <span data-ttu-id="99f85-1807">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="99f85-1807">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="99f85-1808">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="99f85-1808">Backup</span></span>

* <span data-ttu-id="99f85-1809">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="99f85-1809">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="99f85-1810">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1810">September 11, 2017</span></span>

<span data-ttu-id="99f85-1811">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="99f85-1811">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="99f85-1812">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1812">Core</span></span>

* <span data-ttu-id="99f85-1813">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="99f85-1813">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="99f85-1814">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="99f85-1814">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1815">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1815">Acs</span></span>

* <span data-ttu-id="99f85-1816">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1816">Added `acs list-locations` command</span></span>
* <span data-ttu-id="99f85-1817">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-1817">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1818">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1818">Appservice</span></span>

* <span data-ttu-id="99f85-1819">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="99f85-1819">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="99f85-1820">CDN</span><span class="sxs-lookup"><span data-stu-id="99f85-1820">CDN</span></span>

* <span data-ttu-id="99f85-1821">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1821">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="99f85-1822">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="99f85-1822">Extension</span></span>

* <span data-ttu-id="99f85-1823">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="99f85-1823">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="99f85-1824">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="99f85-1824">Keyvault</span></span>

* <span data-ttu-id="99f85-1825">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1825">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1826">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1826">Network</span></span>

* <span data-ttu-id="99f85-1827">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1827">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="99f85-1828">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1828">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="99f85-1829">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1829">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="99f85-1830">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1830">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="99f85-1831">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1831">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-1832">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-1832">Resource</span></span>

* <span data-ttu-id="99f85-1833">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1833">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="99f85-1834">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1834">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="99f85-1835">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1835">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="99f85-1836">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="99f85-1836">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-1837">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-1837">SQL</span></span>

* <span data-ttu-id="99f85-1838">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1838">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1839">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1839">VM</span></span>

* <span data-ttu-id="99f85-1840">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="99f85-1840">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="99f85-1841">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="99f85-1841">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="99f85-1842">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1842">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="99f85-1843">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="99f85-1843">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="99f85-1844">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="99f85-1844">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="99f85-1845">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1845">August 31, 2017</span></span>

<span data-ttu-id="99f85-1846">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="99f85-1846">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="99f85-1847">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="99f85-1847">Keyvault</span></span>

* <span data-ttu-id="99f85-1848">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1848">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="99f85-1849">Sf</span><span class="sxs-lookup"><span data-stu-id="99f85-1849">Sf</span></span>

* <span data-ttu-id="99f85-1850">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="99f85-1850">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1851">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1851">Storage</span></span>

* <span data-ttu-id="99f85-1852">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="99f85-1852">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="99f85-1853">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="99f85-1853">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="99f85-1854">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1854">August 28, 2017</span></span>

<span data-ttu-id="99f85-1855">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="99f85-1855">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="99f85-1856">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="99f85-1856">CLI</span></span>

* <span data-ttu-id="99f85-1857">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="99f85-1857">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1858">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1858">ACS</span></span>

* <span data-ttu-id="99f85-1859">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="99f85-1859">Corrected preview regions</span></span>
* <span data-ttu-id="99f85-1860">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1860">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="99f85-1861">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="99f85-1861">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1862">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1862">Appservice</span></span>

* <span data-ttu-id="99f85-1863">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1863">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="99f85-1864">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1864">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="99f85-1865">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1865">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="99f85-1866">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="99f85-1866">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="99f85-1867">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="99f85-1867">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="99f85-1868">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="99f85-1868">IoT</span></span>

* <span data-ttu-id="99f85-1869">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="99f85-1869">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1870">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1870">Network</span></span>

* <span data-ttu-id="99f85-1871">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1871">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="99f85-1872">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1872">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="99f85-1873">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1873">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="99f85-1874">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1874">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="99f85-1875">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1875">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="99f85-1876">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-1876">Profile</span></span>

* <span data-ttu-id="99f85-1877">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="99f85-1877">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="99f85-1878">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="99f85-1878">Service Fabric</span></span>

* <span data-ttu-id="99f85-1879">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="99f85-1879">Preview release</span></span>
* <span data-ttu-id="99f85-1880">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="99f85-1880">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="99f85-1881">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="99f85-1881">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="99f85-1882">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1882">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1883">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1883">Storage</span></span>

* <span data-ttu-id="99f85-1884">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="99f85-1884">Enabled setting blob tier</span></span>
* <span data-ttu-id="99f85-1885">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-1885">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="99f85-1886">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1886">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="99f85-1887">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="99f85-1887">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="99f85-1888">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1888">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="99f85-1889">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1889">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1890">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1890">VM</span></span>

* <span data-ttu-id="99f85-1891">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1891">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="99f85-1892">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1892">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="99f85-1893">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="99f85-1893">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="99f85-1894">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="99f85-1894">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="99f85-1895">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="99f85-1895">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="99f85-1896">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1896">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="99f85-1897">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1897">August 15, 2017</span></span>

<span data-ttu-id="99f85-1898">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="99f85-1898">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1899">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1899">ACS</span></span>

* <span data-ttu-id="99f85-1900">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="99f85-1900">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1901">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1901">Appservice</span></span>

* <span data-ttu-id="99f85-1902">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="99f85-1902">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="99f85-1903">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-1903">Event Grid</span></span>

* <span data-ttu-id="99f85-1904">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="99f85-1904">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="99f85-1905">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1905">August 11, 2017</span></span>

<span data-ttu-id="99f85-1906">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="99f85-1906">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1907">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1907">ACS</span></span>

* <span data-ttu-id="99f85-1908">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="99f85-1908">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="99f85-1909">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-1909">Batch</span></span>

* <span data-ttu-id="99f85-1910">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="99f85-1910">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="99f85-1911">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="99f85-1911">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="99f85-1912">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1912">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="99f85-1913">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="99f85-1913">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="99f85-1914">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="99f85-1914">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="99f85-1915">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="99f85-1915">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="99f85-1916">Компонент</span><span class="sxs-lookup"><span data-stu-id="99f85-1916">Component</span></span>

* <span data-ttu-id="99f85-1917">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="99f85-1917">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="99f85-1918">Контейнер</span><span class="sxs-lookup"><span data-stu-id="99f85-1918">Container</span></span>

* <span data-ttu-id="99f85-1919">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="99f85-1919">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="99f85-1920">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="99f85-1920">Data Lake Store</span></span>

* <span data-ttu-id="99f85-1921">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="99f85-1921">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="99f85-1922">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-1922">Event Grid</span></span>

* <span data-ttu-id="99f85-1923">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="99f85-1923">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="99f85-1924">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-1924">Network</span></span>

* <span data-ttu-id="99f85-1925">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="99f85-1925">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="99f85-1926">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1926">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="99f85-1927">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1927">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="99f85-1928">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1928">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="99f85-1929">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-1929">Profile</span></span>

* <span data-ttu-id="99f85-1930">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="99f85-1930">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-1931">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-1931">Storage</span></span>

* <span data-ttu-id="99f85-1932">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="99f85-1932">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-1933">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-1933">VM</span></span>

* <span data-ttu-id="99f85-1934">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="99f85-1934">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="99f85-1935">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1935">Exposed `list-skus` command</span></span>
* <span data-ttu-id="99f85-1936">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="99f85-1936">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="99f85-1937">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="99f85-1937">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="99f85-1938">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="99f85-1938">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="99f85-1939">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-1939">July 28, 2017</span></span>

<span data-ttu-id="99f85-1940">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="99f85-1940">Version 2.0.12</span></span>

* <span data-ttu-id="99f85-1941">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1941">Added container commands</span></span>
* <span data-ttu-id="99f85-1942">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1942">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="99f85-1943">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-1943">Core</span></span>

* <span data-ttu-id="99f85-1944">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="99f85-1944">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="99f85-1945">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="99f85-1945">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="99f85-1946">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="99f85-1946">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="99f85-1947">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="99f85-1947">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="99f85-1948">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="99f85-1948">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="99f85-1949">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="99f85-1949">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="99f85-1950">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="99f85-1950">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="99f85-1951">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="99f85-1951">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="99f85-1952">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="99f85-1952">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="99f85-1953">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="99f85-1953">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="99f85-1954">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="99f85-1954">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="99f85-1955">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="99f85-1955">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="99f85-1956">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="99f85-1956">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="99f85-1957">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="99f85-1957">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="99f85-1958">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="99f85-1958">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="99f85-1959">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="99f85-1959">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="99f85-1960">ACR</span><span class="sxs-lookup"><span data-stu-id="99f85-1960">ACR</span></span>

* <span data-ttu-id="99f85-1961">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1961">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="99f85-1962">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="99f85-1962">Support SKU update for managed registries</span></span>
* <span data-ttu-id="99f85-1963">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="99f85-1963">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="99f85-1964">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="99f85-1964">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="99f85-1965">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="99f85-1965">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="99f85-1966">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="99f85-1966">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-1967">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-1967">ACS</span></span>

* <span data-ttu-id="99f85-1968">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="99f85-1968">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-1969">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="99f85-1969">Appservice</span></span>

* <span data-ttu-id="99f85-1970">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="99f85-1970">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="99f85-1971">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="99f85-1971">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="99f85-1972">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1972">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="99f85-1973">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="99f85-1973">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="99f85-1974">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="99f85-1974">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="99f85-1975">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="99f85-1975">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="99f85-1976">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="99f85-1976">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="99f85-1977">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="99f85-1977">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="99f85-1978">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="99f85-1978">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="99f85-1979">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1979">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="99f85-1980">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="99f85-1980">Batch</span></span>

* <span data-ttu-id="99f85-1981">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="99f85-1981">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="99f85-1982">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1982">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="99f85-1983">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1983">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="99f85-1984">CDN</span><span class="sxs-lookup"><span data-stu-id="99f85-1984">CDN</span></span>

* <span data-ttu-id="99f85-1985">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="99f85-1985">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="99f85-1986">Облако</span><span class="sxs-lookup"><span data-stu-id="99f85-1986">Cloud</span></span>

* <span data-ttu-id="99f85-1987">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="99f85-1987">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="99f85-1988">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="99f85-1988">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="99f85-1989">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="99f85-1989">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="99f85-1990">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="99f85-1990">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="99f85-1991">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1991">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="99f85-1992">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="99f85-1992">CosmosDB</span></span>

* <span data-ttu-id="99f85-1993">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="99f85-1993">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="99f85-1994">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="99f85-1994">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="99f85-1995">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="99f85-1995">Data Lake Analytics</span></span>

* <span data-ttu-id="99f85-1996">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1996">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="99f85-1997">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1997">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="99f85-1998">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="99f85-1998">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="99f85-1999">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="99f85-1999">Data Lake Store</span></span>

* <span data-ttu-id="99f85-2000">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2000">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="99f85-2001">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="99f85-2001">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="99f85-2002">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2002">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="99f85-2003">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="99f85-2003">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="99f85-2004">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="99f85-2004">Interactive</span></span>

* <span data-ttu-id="99f85-2005">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="99f85-2005">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="99f85-2006">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="99f85-2006">Increased test coverage</span></span>
* <span data-ttu-id="99f85-2007">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="99f85-2007">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="99f85-2008">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="99f85-2008">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="99f85-2009">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="99f85-2009">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="99f85-2010">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="99f85-2010">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="99f85-2011">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="99f85-2011">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="99f85-2012">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2012">Added `--progress` flag</span></span>
* <span data-ttu-id="99f85-2013">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2013">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="99f85-2014">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="99f85-2014">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="99f85-2015">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="99f85-2015">IoT</span></span>

* <span data-ttu-id="99f85-2016">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="99f85-2016">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="99f85-2017">(3934).</span><span class="sxs-lookup"><span data-stu-id="99f85-2017">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="99f85-2018">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="99f85-2018">Key vault</span></span>

* <span data-ttu-id="99f85-2019">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="99f85-2019">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="99f85-2020">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2020">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="99f85-2021">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="99f85-2021">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="99f85-2022">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="99f85-2022">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="99f85-2023">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2023">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="99f85-2024">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="99f85-2024">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="99f85-2025">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="99f85-2025">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="99f85-2026">(3307).</span><span class="sxs-lookup"><span data-stu-id="99f85-2026">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="99f85-2027">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="99f85-2027">Lab</span></span>

* <span data-ttu-id="99f85-2028">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2028">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="99f85-2029">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2029">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-2030">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-2030">Monitor</span></span>

* <span data-ttu-id="99f85-2031">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="99f85-2031">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="99f85-2032">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2032">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="99f85-2033">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2033">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="99f85-2034">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2034">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="99f85-2035">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2035">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="99f85-2036">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="99f85-2036">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="99f85-2037">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="99f85-2037">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="99f85-2038">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="99f85-2038">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="99f85-2039">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="99f85-2039">`location` no longer required</span></span>
  * <span data-ttu-id="99f85-2040">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="99f85-2040">Add name and ID support for target</span></span>
  * <span data-ttu-id="99f85-2041">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="99f85-2041">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="99f85-2042">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="99f85-2042">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="99f85-2043">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="99f85-2043">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="99f85-2044">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="99f85-2044">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="99f85-2045">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2045">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="99f85-2046">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2046">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="99f85-2047">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-2047">Network</span></span>

* <span data-ttu-id="99f85-2048">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2048">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="99f85-2049">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2049">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="99f85-2050">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="99f85-2050">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="99f85-2051">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2051">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="99f85-2052">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2052">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="99f85-2053">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2053">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="99f85-2054">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2054">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="99f85-2055">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2055">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="99f85-2056">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2056">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="99f85-2057">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2057">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="99f85-2058">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2058">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="99f85-2059">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2059">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="99f85-2060">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2060">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="99f85-2061">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2061">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="99f85-2062">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2062">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="99f85-2063">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2063">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="99f85-2064">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="99f85-2064">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="99f85-2065">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2065">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="99f85-2066">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2066">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="99f85-2067">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2067">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="99f85-2068">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2068">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="99f85-2069">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2069">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="99f85-2070">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2070">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="99f85-2071">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="99f85-2071">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="99f85-2072">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="99f85-2072">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="99f85-2073">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="99f85-2073">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="99f85-2074">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="99f85-2074">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="99f85-2075">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-2075">Profile</span></span>

* <span data-ttu-id="99f85-2076">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="99f85-2076">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="99f85-2077">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="99f85-2077">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="99f85-2078">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="99f85-2078">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="99f85-2079">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="99f85-2079">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="99f85-2080">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="99f85-2080">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="99f85-2081">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="99f85-2081">RDBMS</span></span>

* <span data-ttu-id="99f85-2082">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="99f85-2082">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="99f85-2083">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="99f85-2083">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="99f85-2084">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="99f85-2084">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="99f85-2085">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="99f85-2085">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-2086">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-2086">Resource</span></span>

* <span data-ttu-id="99f85-2087">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2087">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="99f85-2088">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2088">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="99f85-2089">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2089">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="99f85-2090">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2090">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="99f85-2091">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="99f85-2091">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="99f85-2092">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2092">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="99f85-2093">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="99f85-2093">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="99f85-2094">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2094">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="99f85-2095">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-2095">Role</span></span>

* <span data-ttu-id="99f85-2096">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="99f85-2096">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="99f85-2097">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="99f85-2097">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="99f85-2098">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="99f85-2098">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="99f85-2099">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="99f85-2099">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="99f85-2100">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2100">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="99f85-2101">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="99f85-2101">Service Fabric</span></span>
* <span data-ttu-id="99f85-2102">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="99f85-2102">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="99f85-2103">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="99f85-2103">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="99f85-2104">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="99f85-2104">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-2105">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-2105">SQL</span></span>

* <span data-ttu-id="99f85-2106">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2106">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="99f85-2107">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2107">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="99f85-2108">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2108">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-2109">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-2109">Storage</span></span>

* <span data-ttu-id="99f85-2110">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="99f85-2110">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="99f85-2111">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="99f85-2111">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="99f85-2112">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="99f85-2112">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="99f85-2113">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="99f85-2113">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="99f85-2114">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="99f85-2114">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="99f85-2115">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="99f85-2115">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-2116">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-2116">VM</span></span>

* <span data-ttu-id="99f85-2117">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="99f85-2117">Support configuring nsg</span></span>
* <span data-ttu-id="99f85-2118">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="99f85-2118">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="99f85-2119">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="99f85-2119">Support managed service identities</span></span>
* <span data-ttu-id="99f85-2120">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2120">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="99f85-2121">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="99f85-2121">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="99f85-2122">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-2122">May 10, 2017</span></span>

<span data-ttu-id="99f85-2123">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="99f85-2123">Version 2.0.6</span></span>

* <span data-ttu-id="99f85-2124">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="99f85-2124">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="99f85-2125">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="99f85-2125">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="99f85-2126">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="99f85-2126">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="99f85-2127">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="99f85-2127">Include Cognitive Services module</span></span>
* <span data-ttu-id="99f85-2128">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="99f85-2128">Include Service Fabric module</span></span>
* <span data-ttu-id="99f85-2129">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="99f85-2129">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="99f85-2130">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="99f85-2130">Add support for CDN commands</span></span>
* <span data-ttu-id="99f85-2131">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="99f85-2131">Remove Container module</span></span>
* <span data-ttu-id="99f85-2132">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2132">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="99f85-2133">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2133">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="99f85-2134">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-2134">Core</span></span>

* <span data-ttu-id="99f85-2135">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="99f85-2135">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="99f85-2136">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2136">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="99f85-2137">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2137">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="99f85-2138">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2138">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="99f85-2139">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2139">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="99f85-2140">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2140">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="99f85-2141">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2141">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="99f85-2142">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2142">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="99f85-2143">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2143">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="99f85-2144">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="99f85-2144">core: Improved performance</span></span>
* <span data-ttu-id="99f85-2145">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="99f85-2145">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="99f85-2146">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="99f85-2146">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-2147">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-2147">ACS</span></span>

* <span data-ttu-id="99f85-2148">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="99f85-2148">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="99f85-2149">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="99f85-2149">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="99f85-2150">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="99f85-2150">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="99f85-2151">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2151">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-2152">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-2152">AppService</span></span>

* <span data-ttu-id="99f85-2153">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="99f85-2153">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="99f85-2154">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="99f85-2154">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="99f85-2155">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="99f85-2155">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="99f85-2156">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="99f85-2156">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="99f85-2157">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="99f85-2157">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="99f85-2158">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2158">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="99f85-2159">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="99f85-2159">support slot swap with preview</span></span>
* <span data-ttu-id="99f85-2160">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2160">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="99f85-2161">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2161">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="99f85-2162">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="99f85-2162">CosmosDB</span></span>

* <span data-ttu-id="99f85-2163">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="99f85-2163">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="99f85-2164">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="99f85-2164">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="99f85-2165">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="99f85-2165">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="99f85-2166">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="99f85-2166">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="99f85-2167">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="99f85-2167">Data Lake Analytics</span></span>

* <span data-ttu-id="99f85-2168">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="99f85-2168">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="99f85-2169">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="99f85-2169">Add support for new catalog item type: package.</span></span> <span data-ttu-id="99f85-2170">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2170">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="99f85-2171">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="99f85-2171">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="99f85-2172">Таблица</span><span class="sxs-lookup"><span data-stu-id="99f85-2172">Table</span></span>
  * <span data-ttu-id="99f85-2173">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="99f85-2173">Table valued function</span></span>
  * <span data-ttu-id="99f85-2174">Просмотр</span><span class="sxs-lookup"><span data-stu-id="99f85-2174">View</span></span>
  * <span data-ttu-id="99f85-2175">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="99f85-2175">Table Statistics.</span></span> <span data-ttu-id="99f85-2176">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="99f85-2176">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="99f85-2177">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="99f85-2177">Data Lake Store</span></span>

* <span data-ttu-id="99f85-2178">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="99f85-2178">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="99f85-2179">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2179">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="99f85-2180">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="99f85-2180">missed help for access show.</span></span> <span data-ttu-id="99f85-2181">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="99f85-2181">adding it.</span></span> <span data-ttu-id="99f85-2182">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="99f85-2182">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="99f85-2183">Поиск</span><span class="sxs-lookup"><span data-stu-id="99f85-2183">Find</span></span>

* <span data-ttu-id="99f85-2184">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="99f85-2184">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="99f85-2185">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="99f85-2185">KeyVault</span></span>

* <span data-ttu-id="99f85-2186">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="99f85-2186">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="99f85-2187">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="99f85-2187">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="99f85-2188">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="99f85-2188">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="99f85-2189">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="99f85-2189">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="99f85-2190">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2190">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="99f85-2191">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="99f85-2191">Lab</span></span>

* <span data-ttu-id="99f85-2192">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="99f85-2192">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="99f85-2193">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="99f85-2193">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="99f85-2194">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="99f85-2194">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="99f85-2195">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="99f85-2195">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="99f85-2196">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="99f85-2196">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="99f85-2197">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="99f85-2197">Monitor</span></span>

* <span data-ttu-id="99f85-2198">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2198">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="99f85-2199">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2199">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="99f85-2200">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-2200">Network</span></span>

* <span data-ttu-id="99f85-2201">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2201">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="99f85-2202">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2202">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="99f85-2203">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="99f85-2203">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="99f85-2204">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="99f85-2204">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="99f85-2205">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="99f85-2205">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="99f85-2206">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="99f85-2206">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="99f85-2207">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="99f85-2207">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="99f85-2208">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="99f85-2208">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="99f85-2209">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2209">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="99f85-2210">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="99f85-2210">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="99f85-2211">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2211">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="99f85-2212">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2212">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="99f85-2213">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="99f85-2213">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="99f85-2214">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="99f85-2214">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="99f85-2215">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="99f85-2215">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="99f85-2216">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="99f85-2216">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="99f85-2217">Профиль</span><span class="sxs-lookup"><span data-stu-id="99f85-2217">Profile</span></span>

* <span data-ttu-id="99f85-2218">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2218">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="99f85-2219">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2219">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="99f85-2220">Redis</span><span class="sxs-lookup"><span data-stu-id="99f85-2220">Redis</span></span>

* <span data-ttu-id="99f85-2221">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="99f85-2221">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="99f85-2222">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="99f85-2222">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="99f85-2223">Ресурс</span><span class="sxs-lookup"><span data-stu-id="99f85-2223">Resource</span></span>

* <span data-ttu-id="99f85-2224">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2224">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="99f85-2225">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2225">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="99f85-2226">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2226">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="99f85-2227">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="99f85-2227">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="99f85-2228">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="99f85-2228">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="99f85-2229">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="99f85-2229">Add docs for az lock update.</span></span> <span data-ttu-id="99f85-2230">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="99f85-2230">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="99f85-2231">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="99f85-2231">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="99f85-2232">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="99f85-2232">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="99f85-2233">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="99f85-2233">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="99f85-2234">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="99f85-2234">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="99f85-2235">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2235">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="99f85-2236">Роль</span><span class="sxs-lookup"><span data-stu-id="99f85-2236">Role</span></span>

* <span data-ttu-id="99f85-2237">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2237">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="99f85-2238">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2238">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="99f85-2239">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2239">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="99f85-2240">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="99f85-2240">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="99f85-2241">SQL</span><span class="sxs-lookup"><span data-stu-id="99f85-2241">SQL</span></span>

* <span data-ttu-id="99f85-2242">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="99f85-2242">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="99f85-2243">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2243">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="99f85-2244">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-2244">Storage</span></span>

* <span data-ttu-id="99f85-2245">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2245">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="99f85-2246">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="99f85-2246">Add support for incremental blob copy</span></span>
* <span data-ttu-id="99f85-2247">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="99f85-2247">Add support for large block blob upload</span></span>
* <span data-ttu-id="99f85-2248">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="99f85-2248">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-2249">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-2249">VM</span></span>

* <span data-ttu-id="99f85-2250">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="99f85-2250">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="99f85-2251">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="99f85-2251">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="99f85-2252">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="99f85-2252">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="99f85-2253">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="99f85-2253">az vm/vmss disk</span></span>
  3. <span data-ttu-id="99f85-2254">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="99f85-2254">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="99f85-2255">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="99f85-2255">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="99f85-2256">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2256">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="99f85-2257">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-2257">April 3, 2017</span></span>

<span data-ttu-id="99f85-2258">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="99f85-2258">Version 2.0.2</span></span>

<span data-ttu-id="99f85-2259">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="99f85-2259">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="99f85-2260">Core</span><span class="sxs-lookup"><span data-stu-id="99f85-2260">Core</span></span>

* <span data-ttu-id="99f85-2261">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-2261">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="99f85-2262">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2262">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="99f85-2263">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2263">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="99f85-2264">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2264">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="99f85-2265">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2265">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="99f85-2266">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="99f85-2266">Add prompting for missing template parameters.</span></span> <span data-ttu-id="99f85-2267">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2267">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="99f85-2268">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="99f85-2268">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="99f85-2269">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="99f85-2269">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="99f85-2270">ACS</span><span class="sxs-lookup"><span data-stu-id="99f85-2270">ACS</span></span>

* <span data-ttu-id="99f85-2271">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2271">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="99f85-2272">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="99f85-2272">Add support for ssh key password prompting.</span></span> <span data-ttu-id="99f85-2273">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2273">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="99f85-2274">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="99f85-2274">Add support for windows clusters.</span></span> <span data-ttu-id="99f85-2275">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2275">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="99f85-2276">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="99f85-2276">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="99f85-2277">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2277">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="99f85-2278">AppService</span><span class="sxs-lookup"><span data-stu-id="99f85-2278">AppService</span></span>

* <span data-ttu-id="99f85-2279">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2279">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="99f85-2280">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2280">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="99f85-2281">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2281">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="99f85-2282">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2282">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="99f85-2283">Data Lake</span><span class="sxs-lookup"><span data-stu-id="99f85-2283">DataLake</span></span>

* <span data-ttu-id="99f85-2284">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="99f85-2284">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="99f85-2285">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="99f85-2285">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="99f85-2286">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="99f85-2286">DocuemntDB</span></span>

* <span data-ttu-id="99f85-2287">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2287">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="99f85-2288">ВМ</span><span class="sxs-lookup"><span data-stu-id="99f85-2288">VM</span></span>

* <span data-ttu-id="99f85-2289">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2289">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="99f85-2290">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2290">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="99f85-2291">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2291">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="99f85-2292">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2292">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="99f85-2293">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2293">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="99f85-2294">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2294">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="99f85-2295">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="99f85-2295">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="99f85-2296">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="99f85-2296">February 27, 2017</span></span>

<span data-ttu-id="99f85-2297">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="99f85-2297">Version 2.0.0</span></span>

<span data-ttu-id="99f85-2298">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="99f85-2298">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="99f85-2299">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="99f85-2299">Container Service (acs)</span></span>
- <span data-ttu-id="99f85-2300">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="99f85-2300">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="99f85-2301">Сеть</span><span class="sxs-lookup"><span data-stu-id="99f85-2301">Networking</span></span>
- <span data-ttu-id="99f85-2302">Хранилище</span><span class="sxs-lookup"><span data-stu-id="99f85-2302">Storage</span></span>

<span data-ttu-id="99f85-2303">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2303">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="99f85-2304">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="99f85-2304">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="99f85-2305">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="99f85-2305">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="99f85-2306">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="99f85-2306">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="99f85-2307">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="99f85-2307">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="99f85-2308">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="99f85-2308">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="99f85-2309">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="99f85-2309">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="99f85-2310">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="99f85-2310">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="99f85-2311">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="99f85-2311">Provide feedback from the command line with the `az feedback` command</span></span>

