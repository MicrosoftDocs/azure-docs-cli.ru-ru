---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/15/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 4337f2203841d6247e4b487d245138424c63e448
ms.sourcegitcommit: 71c0ccd475524cf4d6db45bba8139fef3262d764
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/19/2019
ms.locfileid: "58175139"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="fc024-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="fc024-103">Azure CLI release notes</span></span>
## <a name="march-12-2019"></a><span data-ttu-id="fc024-104">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-104">March 12, 2019</span></span>

<span data-ttu-id="fc024-105">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="fc024-105">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="fc024-106">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-106">Core</span></span>

* <span data-ttu-id="fc024-107">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="fc024-107">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-108">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-108">ACR</span></span>

* <span data-ttu-id="fc024-109">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="fc024-109">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-110">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-110">ACS</span></span>

* <span data-ttu-id="fc024-111">Аргумент `--listen-address` для `aks browse` игнорируется, если `kubectl` не поддерживает его.</span><span class="sxs-lookup"><span data-stu-id="fc024-111">Changed to ignore `--listen-address` argument to `aks browse` if `kubectl` doesn't support it</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-112">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-112">AppService</span></span>

* <span data-ttu-id="fc024-113">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="fc024-113">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="fc024-114">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-114">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="fc024-115">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="fc024-115">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="fc024-116">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="fc024-116">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="fc024-117">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="fc024-117">Botservice</span></span>

* <span data-ttu-id="fc024-118">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="fc024-118">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="fc024-119">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="fc024-119">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="fc024-120">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-120">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="fc024-121">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="fc024-121">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="fc024-122">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-122">Container</span></span>

* <span data-ttu-id="fc024-123">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="fc024-123">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="fc024-124">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="fc024-124">EventHub</span></span>

* <span data-ttu-id="fc024-125">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="fc024-125">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="fc024-126">Поиск</span><span class="sxs-lookup"><span data-stu-id="fc024-126">Find</span></span>

* <span data-ttu-id="fc024-127">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="fc024-127">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc024-128">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc024-128">HDInsight</span></span>

* <span data-ttu-id="fc024-129">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="fc024-129">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="fc024-130">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-130">Network</span></span>

* <span data-ttu-id="fc024-131">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="fc024-131">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc024-132">Rdbms</span><span class="sxs-lookup"><span data-stu-id="fc024-132">Rdbms</span></span>

* <span data-ttu-id="fc024-133">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="fc024-133">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="fc024-134">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-134">Role</span></span>

* <span data-ttu-id="fc024-135">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="fc024-135">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="fc024-136">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="fc024-136">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fc024-137">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fc024-137">Service Fabric</span></span>

* <span data-ttu-id="fc024-138">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="fc024-138">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="fc024-139">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-139">February 26, 2019</span></span>

<span data-ttu-id="fc024-140">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="fc024-140">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="fc024-141">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-141">Core</span></span>

* <span data-ttu-id="fc024-142">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="fc024-142">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-143">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-143">ACR</span></span>

* <span data-ttu-id="fc024-144">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-144">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="fc024-145">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="fc024-145">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-146">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-146">ACS</span></span>

* <span data-ttu-id="fc024-147">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="fc024-147">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-148">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-148">AppService</span></span>

* <span data-ttu-id="fc024-149">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="fc024-149">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="fc024-150">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-150">Batch</span></span>
* <span data-ttu-id="fc024-151">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="fc024-151">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="fc024-152">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="fc024-152">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="fc024-153">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="fc024-153">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="fc024-154">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="fc024-154">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="fc024-155">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="fc024-155">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="fc024-156">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fc024-156">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc024-157">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc024-157">CosmosDB</span></span>

* <span data-ttu-id="fc024-158">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="fc024-158">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="fc024-159">Kusto</span><span class="sxs-lookup"><span data-stu-id="fc024-159">Kusto</span></span>

* <span data-ttu-id="fc024-160">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="fc024-160">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="fc024-161">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-161">Network</span></span>

* <span data-ttu-id="fc024-162">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fc024-162">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="fc024-163">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="fc024-163">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="fc024-164">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="fc024-164">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="fc024-165">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-165">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="fc024-166">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-166">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="fc024-167">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fc024-167">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="fc024-168">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="fc024-168">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-169">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-169">Resource</span></span>

* <span data-ttu-id="fc024-170">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="fc024-170">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="fc024-171">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-171">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="fc024-172">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-172">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="fc024-173">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-173">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="fc024-174">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="fc024-174">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="fc024-175">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-175">Role</span></span>

* <span data-ttu-id="fc024-176">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-176">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-177">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-177">VM</span></span>

* <span data-ttu-id="fc024-178">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="fc024-178">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="fc024-179">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-179">February 12, 2019</span></span>

<span data-ttu-id="fc024-180">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="fc024-180">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="fc024-181">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-181">Core</span></span>

* <span data-ttu-id="fc024-182">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="fc024-182">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="fc024-183">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="fc024-183">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-184">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-184">ACR</span></span>
* <span data-ttu-id="fc024-185">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="fc024-185">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="fc024-186">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="fc024-186">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-187">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-187">ACS</span></span>
* <span data-ttu-id="fc024-188">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="fc024-188">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="fc024-189">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="fc024-189">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="fc024-190">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="fc024-190">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="fc024-191">AMS</span><span class="sxs-lookup"><span data-stu-id="fc024-191">AMS</span></span>
* <span data-ttu-id="fc024-192">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-192">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="fc024-193">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-193">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-194">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-194">Appservice</span></span>
* <span data-ttu-id="fc024-195">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="fc024-195">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="fc024-196">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="fc024-196">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="fc024-197">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-197">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="fc024-198">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="fc024-198">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="fc024-199">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="fc024-199">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="fc024-200">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="fc024-200">Botservice</span></span>
* <span data-ttu-id="fc024-201">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="fc024-201">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="fc024-202">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="fc024-202">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="fc024-203">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-203">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="fc024-204">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="fc024-204">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="fc024-205">[УСТАРЕЛО.] Аргумент `--proj-name` не поддерживается. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="fc024-205">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="fc024-206">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="fc024-206">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="fc024-207">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="fc024-207">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="fc024-208">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="fc024-208">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="fc024-209">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="fc024-209">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="fc024-210">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="fc024-210">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc024-211">Key Vault</span><span class="sxs-lookup"><span data-stu-id="fc024-211">Key Vault</span></span>
* <span data-ttu-id="fc024-212">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="fc024-212">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-213">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-213">Monitor</span></span>
* <span data-ttu-id="fc024-214">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="fc024-214">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="fc024-215">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-215">Network</span></span>
* <span data-ttu-id="fc024-216">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="fc024-216">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="fc024-217">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="fc024-217">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="fc024-218">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="fc024-218">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="fc024-219">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="fc024-219">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="fc024-220">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="fc024-220">Policy Insights</span></span>
* <span data-ttu-id="fc024-221">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fc024-221">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc024-222">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="fc024-222">RDBMS</span></span>
* <span data-ttu-id="fc024-223">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="fc024-223">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="fc024-224">Redis</span><span class="sxs-lookup"><span data-stu-id="fc024-224">Redis</span></span>
* <span data-ttu-id="fc024-225">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="fc024-225">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="fc024-226">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="fc024-226">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="fc024-227">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="fc024-227">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="fc024-228">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="fc024-228">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="fc024-229">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="fc024-229">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="fc024-230">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="fc024-230">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="fc024-231">[УСТРАРЕЛО.] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc024-231">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="fc024-232">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-232">Role</span></span>
* <span data-ttu-id="fc024-233">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="fc024-233">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="fc024-234">ВМ SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-234">SQL VM</span></span>
* <span data-ttu-id="fc024-235">[УСТАРЕЛО.] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="fc024-235">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-236">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-236">VM</span></span>
* <span data-ttu-id="fc024-237">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="fc024-237">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="fc024-238">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-238">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="fc024-239">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="fc024-239">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="fc024-240">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="fc024-240">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="fc024-241">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-241">January 31, 2019</span></span>

<span data-ttu-id="fc024-242">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="fc024-242">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="fc024-243">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-243">Core</span></span>

* <span data-ttu-id="fc024-244">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="fc024-244">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="fc024-245">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-245">January 28, 2019</span></span>

<span data-ttu-id="fc024-246">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="fc024-246">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-247">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-247">ACR</span></span>
* <span data-ttu-id="fc024-248">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="fc024-248">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-249">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-249">ACS</span></span>
* <span data-ttu-id="fc024-250">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="fc024-250">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="fc024-251">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="fc024-251">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="fc024-252">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="fc024-252">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="fc024-253">AMS</span><span class="sxs-lookup"><span data-stu-id="fc024-253">AMS</span></span>
* <span data-ttu-id="fc024-254">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="fc024-254">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="fc024-255">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="fc024-255">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-256">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-256">Appservice</span></span>
* <span data-ttu-id="fc024-257">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-257">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="fc024-258">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="fc024-258">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="fc024-259">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="fc024-259">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="fc024-260">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-260">Container</span></span>
* <span data-ttu-id="fc024-261">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="fc024-261">Added `container start` command</span></span>
* <span data-ttu-id="fc024-262">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-262">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="fc024-263">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="fc024-263">EventGrid</span></span>
* <span data-ttu-id="fc024-264">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-264">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="fc024-265">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="fc024-265">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="fc024-266">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="fc024-266">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="fc024-267">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="fc024-267">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="fc024-268">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="fc024-268">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc024-269">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc024-269">HDInsight</span></span>
* <span data-ttu-id="fc024-270">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="fc024-270">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="fc024-271">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="fc024-271">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="fc024-272">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-272">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="fc024-273">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="fc024-273">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="fc024-274">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="fc024-274">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="fc024-275">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-275">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="fc024-276">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="fc024-276">IoT</span></span>
* <span data-ttu-id="fc024-277">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="fc024-277">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="fc024-278">Kusto</span><span class="sxs-lookup"><span data-stu-id="fc024-278">Kusto</span></span>
* <span data-ttu-id="fc024-279">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="fc024-279">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-280">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-280">Monitor</span></span>
* <span data-ttu-id="fc024-281">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="fc024-281">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="fc024-282">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-282">Profile</span></span>
* <span data-ttu-id="fc024-283">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-283">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="fc024-284">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-284">Network</span></span>
* <span data-ttu-id="fc024-285">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="fc024-285">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="fc024-286">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="fc024-286">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-287">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-287">Resource</span></span>
* <span data-ttu-id="fc024-288">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-288">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="fc024-289">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-289">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="fc024-290">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-290">SQL Virtual Machine</span></span>
* <span data-ttu-id="fc024-291">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="fc024-291">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-292">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-292">Storage</span></span>
* <span data-ttu-id="fc024-293">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="fc024-293">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="fc024-294">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="fc024-294">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-295">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-295">VM</span></span>
* <span data-ttu-id="fc024-296">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="fc024-296">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="fc024-297">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="fc024-297">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="fc024-298">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-298">January 15, 2019</span></span>

<span data-ttu-id="fc024-299">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="fc024-299">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-300">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-300">ACR</span></span>
* <span data-ttu-id="fc024-301">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="fc024-301">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="fc024-302">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="fc024-302">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="fc024-303">[УСТАРЕЛО.] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="fc024-303">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="fc024-304">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-304">ACS</span></span>
* <span data-ttu-id="fc024-305">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="fc024-305">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-306">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-306">Appservice</span></span>
* <span data-ttu-id="fc024-307">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="fc024-307">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="fc024-308">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="fc024-308">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="fc024-309">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="fc024-309">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="fc024-310">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="fc024-310">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="fc024-311">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="fc024-311">Botservice</span></span>
* <span data-ttu-id="fc024-312">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-312">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="fc024-313">Настройка</span><span class="sxs-lookup"><span data-stu-id="fc024-313">Configure</span></span>
* <span data-ttu-id="fc024-314">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="fc024-314">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc024-315">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc024-315">CosmosDB</span></span>
* <span data-ttu-id="fc024-316">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="fc024-316">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc024-317">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc024-317">HDInsight</span></span>
* <span data-ttu-id="fc024-318">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="fc024-318">Added commands for managing applications</span></span>
* <span data-ttu-id="fc024-319">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="fc024-319">Added commands for managing script actions</span></span>
* <span data-ttu-id="fc024-320">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="fc024-320">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="fc024-321">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="fc024-321">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="fc024-322">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-322">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="fc024-323">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-323">Network</span></span>
* <span data-ttu-id="fc024-324">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fc024-324">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="fc024-325">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="fc024-325">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="fc024-326">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fc024-326">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="fc024-327">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-327">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="fc024-328">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-328">Role</span></span>
* <span data-ttu-id="fc024-329">[УСТАРЕЛО.] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc024-329">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="fc024-330">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="fc024-330">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="fc024-331">Безопасность</span><span class="sxs-lookup"><span data-stu-id="fc024-331">Security</span></span>
* <span data-ttu-id="fc024-332">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="fc024-332">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-333">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-333">Storage</span></span>
* <span data-ttu-id="fc024-334">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="fc024-334">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="fc024-335">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="fc024-335">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="fc024-336">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="fc024-336">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="fc024-337">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="fc024-337">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="fc024-338">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="fc024-338">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-339">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-339">VM</span></span>
* <span data-ttu-id="fc024-340">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="fc024-340">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="fc024-341">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-341">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="fc024-342">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="fc024-342">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="fc024-343">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="fc024-343">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="fc024-344">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-344">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="fc024-345">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="fc024-345">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="fc024-346">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-346">December 20, 2018</span></span>

<span data-ttu-id="fc024-347">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="fc024-347">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="fc024-348">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-348">Appservice</span></span>
* <span data-ttu-id="fc024-349">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="fc024-349">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="fc024-350">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="fc024-350">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="fc024-351">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="fc024-351">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="fc024-352">IoT Central</span><span class="sxs-lookup"><span data-stu-id="fc024-352">IoTCentral</span></span>
* <span data-ttu-id="fc024-353">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="fc024-353">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="fc024-354">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-354">Role</span></span>
* <span data-ttu-id="fc024-355">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="fc024-355">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-356">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-356">SQL</span></span>
* <span data-ttu-id="fc024-357">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="fc024-357">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-358">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-358">VM</span></span>
* <span data-ttu-id="fc024-359">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-359">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="fc024-360">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-360">December 18, 2018</span></span>

<span data-ttu-id="fc024-361">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="fc024-361">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="fc024-362">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-362">ACR</span></span>
* <span data-ttu-id="fc024-363">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-363">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="fc024-364">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="fc024-364">Condensed the table layout for task list</span></span>
* <span data-ttu-id="fc024-365">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="fc024-365">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-366">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-366">ACS</span></span>
* <span data-ttu-id="fc024-367">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="fc024-367">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="fc024-368">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="fc024-368">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="fc024-369">[УСТАРЕЛО] Команды `az acs` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="fc024-369">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="fc024-370">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-370">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="fc024-371">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="fc024-371">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="fc024-372">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="fc024-372">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-373">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-373">Appservice</span></span>
* <span data-ttu-id="fc024-374">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="fc024-374">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="fc024-375">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="fc024-375">Botservice</span></span>
* <span data-ttu-id="fc024-376">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-376">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="fc024-377">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="fc024-377">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="fc024-378">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="fc024-378">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="fc024-379">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="fc024-379">Reduced Kudu network calls</span></span>
* <span data-ttu-id="fc024-380">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="fc024-380">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="fc024-381">Потребление</span><span class="sxs-lookup"><span data-stu-id="fc024-381">Consumption</span></span>
* <span data-ttu-id="fc024-382">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="fc024-382">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc024-383">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc024-383">CosmosDB</span></span>
* <span data-ttu-id="fc024-384">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="fc024-384">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="fc024-385">Карты</span><span class="sxs-lookup"><span data-stu-id="fc024-385">Maps</span></span>
* <span data-ttu-id="fc024-386">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="fc024-386">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="fc024-387">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-387">Network</span></span>
* <span data-ttu-id="fc024-388">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="fc024-388">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="fc024-389">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="fc024-389">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-390">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-390">Resource</span></span>
* <span data-ttu-id="fc024-391">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-391">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="fc024-392">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-392">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-393">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-393">Storage</span></span>
*  <span data-ttu-id="fc024-394">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="fc024-394">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-395">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-395">VM</span></span>
* <span data-ttu-id="fc024-396">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-396">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="fc024-397">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-397">December 4, 2018</span></span>

<span data-ttu-id="fc024-398">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="fc024-398">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="fc024-399">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-399">Core</span></span>
* <span data-ttu-id="fc024-400">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-400">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="fc024-401">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="fc024-401">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-402">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-402">Appservice</span></span>
* <span data-ttu-id="fc024-403">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="fc024-403">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="fc024-404">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="fc024-404">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="fc024-405">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-405">Network</span></span>
* <span data-ttu-id="fc024-406">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="fc024-406">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="fc024-407">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-407">Role</span></span>
* <span data-ttu-id="fc024-408">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="fc024-408">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="fc024-409">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-409">VM</span></span>
* <span data-ttu-id="fc024-410">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` устарел.</span><span class="sxs-lookup"><span data-stu-id="fc024-410">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="fc024-411">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="fc024-411">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="fc024-412">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="fc024-412">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="fc024-413">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="fc024-413">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="fc024-414">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-414">November 20, 2018</span></span>

<span data-ttu-id="fc024-415">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="fc024-415">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="fc024-416">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-416">Core</span></span>
* <span data-ttu-id="fc024-417">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="fc024-417">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-418">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-418">ACR</span></span>
* <span data-ttu-id="fc024-419">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="fc024-419">Added context token to task step</span></span>
* <span data-ttu-id="fc024-420">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="fc024-420">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="fc024-421">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="fc024-421">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-422">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-422">Appservice</span></span>
* <span data-ttu-id="fc024-423">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="fc024-423">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="fc024-424">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-424">Updated the default `node_version`.</span></span> <span data-ttu-id="fc024-425">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="fc024-425">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="fc024-426">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="fc024-426">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="fc024-427">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="fc024-427">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="fc024-428">IotCentral</span><span class="sxs-lookup"><span data-stu-id="fc024-428">IotCentral</span></span>
* <span data-ttu-id="fc024-429">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="fc024-429">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc024-430">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="fc024-430">KeyVault</span></span>
* <span data-ttu-id="fc024-431">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="fc024-431">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="fc024-432">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-432">Network</span></span>
* <span data-ttu-id="fc024-433">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="fc024-433">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="fc024-434">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="fc024-434">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="fc024-435">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="fc024-435">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="fc024-436">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="fc024-436">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc024-437">Rdbms</span><span class="sxs-lookup"><span data-stu-id="fc024-437">Rdbms</span></span>
* <span data-ttu-id="fc024-438">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="fc024-438">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="fc024-439">RBAC:</span><span class="sxs-lookup"><span data-stu-id="fc024-439">Rbac</span></span>
* <span data-ttu-id="fc024-440">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-440">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="fc024-441">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="fc024-441">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="fc024-442">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-442">Storage</span></span>
* <span data-ttu-id="fc024-443">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="fc024-443">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="fc024-444">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="fc024-444">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="fc024-445">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="fc024-445">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="fc024-446">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="fc024-446">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-447">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-447">VM</span></span>
* <span data-ttu-id="fc024-448">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="fc024-448">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="fc024-449">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="fc024-449">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="fc024-450">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="fc024-450">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="fc024-451">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="fc024-451">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="fc024-452">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-452">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="fc024-453">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-453">Added `snapshot wait` command</span></span>
* <span data-ttu-id="fc024-454">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="fc024-454">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="fc024-455">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-455">November 6, 2018</span></span>

<span data-ttu-id="fc024-456">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="fc024-456">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="fc024-457">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-457">Core</span></span>
* <span data-ttu-id="fc024-458">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="fc024-458">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-459">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-459">ACR</span></span>
* <span data-ttu-id="fc024-460">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="fc024-460">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="fc024-461">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="fc024-461">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-462">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-462">ACS</span></span>
* <span data-ttu-id="fc024-463">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-463">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="fc024-464">Помощник</span><span class="sxs-lookup"><span data-stu-id="fc024-464">Advisor</span></span>
* <span data-ttu-id="fc024-465">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="fc024-465">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="fc024-466">AMS</span><span class="sxs-lookup"><span data-stu-id="fc024-466">AMS</span></span>
* <span data-ttu-id="fc024-467">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="fc024-467">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="fc024-468">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="fc024-468">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="fc024-469">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-469">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="fc024-470">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="fc024-470">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="fc024-471">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="fc024-471">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="fc024-472">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="fc024-472">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="fc024-473">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="fc024-473">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="fc024-474">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="fc024-474">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="fc024-475">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="fc024-475">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="fc024-476">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="fc024-476">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="fc024-477">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="fc024-477">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="fc024-478">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="fc024-478">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="fc024-479">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="fc024-479">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="fc024-480">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="fc024-480">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="fc024-481">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="fc024-481">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="fc024-482">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="fc024-482">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="fc024-483">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="fc024-483">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-484">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-484">AppService</span></span>
* <span data-ttu-id="fc024-485">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="fc024-485">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="fc024-486">Настройка</span><span class="sxs-lookup"><span data-stu-id="fc024-486">Configure</span></span>
* <span data-ttu-id="fc024-487">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="fc024-487">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="fc024-488">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-488">Container</span></span>
* <span data-ttu-id="fc024-489">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="fc024-489">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="fc024-490">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="fc024-490">EventHub</span></span>
* <span data-ttu-id="fc024-491">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-491">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-492">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc024-492">Interactive</span></span>
* <span data-ttu-id="fc024-493">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="fc024-493">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-494">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-494">Monitor</span></span>
* <span data-ttu-id="fc024-495">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-495">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="fc024-496">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-496">Network</span></span>
* <span data-ttu-id="fc024-497">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="fc024-497">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="fc024-498">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="fc024-498">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="fc024-499">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-499">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="fc024-500">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-500">Profile</span></span>
* <span data-ttu-id="fc024-501">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="fc024-501">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc024-502">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="fc024-502">RDBMS</span></span>
* <span data-ttu-id="fc024-503">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="fc024-503">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-504">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-504">Resource</span></span>
* <span data-ttu-id="fc024-505">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="fc024-505">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="fc024-506">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-506">Role</span></span>
* <span data-ttu-id="fc024-507">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="fc024-507">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="fc024-508">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-508">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="fc024-509">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="fc024-509">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-510">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-510">Storage</span></span>
* <span data-ttu-id="fc024-511">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="fc024-511">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-512">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-512">VM</span></span>
* <span data-ttu-id="fc024-513">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="fc024-513">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="fc024-514">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="fc024-514">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="fc024-515">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="fc024-515">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="fc024-516">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="fc024-516">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="fc024-517">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="fc024-517">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="fc024-518">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="fc024-518">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="fc024-519">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-519">October 23, 2018</span></span>

<span data-ttu-id="fc024-520">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="fc024-520">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="fc024-521">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-521">Core</span></span>
* <span data-ttu-id="fc024-522">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="fc024-522">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="fc024-523">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="fc024-523">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-524">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-524">ACR</span></span>
* <span data-ttu-id="fc024-525">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="fc024-525">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="fc024-526">CDN</span><span class="sxs-lookup"><span data-stu-id="fc024-526">CDN</span></span>
* <span data-ttu-id="fc024-527">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-527">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="fc024-528">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="fc024-528">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="fc024-529">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-529">Container</span></span>
* <span data-ttu-id="fc024-530">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="fc024-530">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="fc024-531">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="fc024-531">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="fc024-532">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fc024-532">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="fc024-533">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-533">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="fc024-534">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="fc024-534">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="fc024-535">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="fc024-535">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="fc024-536">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-536">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc024-537">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc024-537">CosmosDB</span></span>
* <span data-ttu-id="fc024-538">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="fc024-538">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-539">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc024-539">Interactive</span></span>
* <span data-ttu-id="fc024-540">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="fc024-540">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="fc024-541">IoT Central</span><span class="sxs-lookup"><span data-stu-id="fc024-541">IoT Central</span></span>
* <span data-ttu-id="fc024-542">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="fc024-542">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="fc024-543">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="fc024-543">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-544">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-544">Monitor</span></span>
* <span data-ttu-id="fc024-545">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="fc024-545">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="fc024-546">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="fc024-546">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="fc024-547">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="fc024-547">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="fc024-548">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="fc024-548">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="fc024-549">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="fc024-549">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="fc024-550">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="fc024-550">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="fc024-551">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="fc024-551">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="fc024-552">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="fc024-552">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="fc024-553">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="fc024-553">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="fc024-554">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-554">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="fc024-555">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-555">Network</span></span>
* <span data-ttu-id="fc024-556">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="fc024-556">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="fc024-557">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="fc024-557">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="fc024-558">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="fc024-558">ServiceBus</span></span>
* <span data-ttu-id="fc024-559">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="fc024-559">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-560">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-560">SQL</span></span>
* <span data-ttu-id="fc024-561">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="fc024-561">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-562">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-562">Storage</span></span>
* <span data-ttu-id="fc024-563">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-563">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="fc024-564">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="fc024-564">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-565">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-565">VM</span></span>
* <span data-ttu-id="fc024-566">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="fc024-566">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="fc024-567">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="fc024-567">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="fc024-568">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="fc024-568">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="fc024-569">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-569">October 16, 2018</span></span>

<span data-ttu-id="fc024-570">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="fc024-570">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-571">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-571">VM</span></span>
* <span data-ttu-id="fc024-572">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="fc024-572">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="fc024-573">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-573">October 9, 2018</span></span>

<span data-ttu-id="fc024-574">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="fc024-574">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="fc024-575">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-575">Core</span></span>
* <span data-ttu-id="fc024-576">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="fc024-576">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-577">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-577">ACR</span></span>
* <span data-ttu-id="fc024-578">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="fc024-578">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-579">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-579">ACS</span></span>
* <span data-ttu-id="fc024-580">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="fc024-580">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="fc024-581">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="fc024-581">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="fc024-582">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="fc024-582">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="fc024-583">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="fc024-583">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="fc024-584">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-584">Container</span></span>
* <span data-ttu-id="fc024-585">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="fc024-585">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="fc024-586">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="fc024-586">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="fc024-587">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="fc024-587">Event Hub</span></span>
* <span data-ttu-id="fc024-588">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-588">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="fc024-589">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="fc024-589">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="fc024-590">расширения.</span><span class="sxs-lookup"><span data-stu-id="fc024-590">Extensions</span></span>
* <span data-ttu-id="fc024-591">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="fc024-591">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="fc024-592">HDInsight</span><span class="sxs-lookup"><span data-stu-id="fc024-592">HDInsight</span></span>
* <span data-ttu-id="fc024-593">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="fc024-593">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="fc024-594">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="fc024-594">IoT</span></span>
* <span data-ttu-id="fc024-595">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="fc024-595">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc024-596">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="fc024-596">KeyVault</span></span>
* <span data-ttu-id="fc024-597">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="fc024-597">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="fc024-598">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-598">Network</span></span>
* <span data-ttu-id="fc024-599">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-599">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="fc024-600">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="fc024-600">See #6052</span></span>
* <span data-ttu-id="fc024-601">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-601">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="fc024-602">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="fc024-602">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="fc024-603">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="fc024-603">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="fc024-604">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="fc024-604">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="fc024-605">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="fc024-605">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="fc024-606">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-606">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="fc024-607">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-607">Role</span></span>
* <span data-ttu-id="fc024-608">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="fc024-608">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="fc024-609">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="fc024-609">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="fc024-610">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="fc024-610">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="fc024-611">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="fc024-611">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="fc024-612">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-612">Service Bus</span></span>
* <span data-ttu-id="fc024-613">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="fc024-613">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-614">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-614">VM</span></span>
* <span data-ttu-id="fc024-615">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="fc024-615">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="fc024-616">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="fc024-616">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="fc024-617">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="fc024-617">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="fc024-618">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="fc024-618">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="fc024-619">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="fc024-619">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="fc024-620">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="fc024-620">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="fc024-621">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-621">September 21, 2018</span></span>

<span data-ttu-id="fc024-622">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="fc024-622">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-623">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-623">ACR</span></span>
* <span data-ttu-id="fc024-624">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="fc024-624">Added ACR Task commands</span></span>
* <span data-ttu-id="fc024-625">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="fc024-625">Added quick run command</span></span>
* <span data-ttu-id="fc024-626">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="fc024-626">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="fc024-627">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="fc024-627">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="fc024-628">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="fc024-628">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="fc024-629">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="fc024-629">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-630">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-630">ACS</span></span>
* <span data-ttu-id="fc024-631">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="fc024-631">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="fc024-632">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="fc024-632">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-633">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-633">AppService</span></span>

* <span data-ttu-id="fc024-634">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="fc024-634">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="fc024-635">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="fc024-635">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="fc024-636">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="fc024-636">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="fc024-637">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="fc024-637">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="fc024-638">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-638">Batch</span></span>
* <span data-ttu-id="fc024-639">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="fc024-639">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="fc024-640">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="fc024-640">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="fc024-641">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-641">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="fc024-642">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="fc024-642">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="fc024-643">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="fc024-643">Batch AI</span></span> 
* <span data-ttu-id="fc024-644">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-644">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="fc024-645">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="fc024-645">Cognitive Services</span></span>
* <span data-ttu-id="fc024-646">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="fc024-646">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="fc024-647">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="fc024-647">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="fc024-648">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="fc024-648">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="fc024-649">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="fc024-649">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="fc024-650">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="fc024-650">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="fc024-651">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="fc024-651">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="fc024-652">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-652">Container</span></span>
* <span data-ttu-id="fc024-653">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-653">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="fc024-654">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="fc024-654">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="fc024-655">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="fc024-655">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="fc024-656">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-656">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="fc024-657">Data Lake</span><span class="sxs-lookup"><span data-stu-id="fc024-657">Datalake</span></span>
* <span data-ttu-id="fc024-658">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="fc024-658">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="fc024-659">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="fc024-659">Interactive Shell</span></span>
* <span data-ttu-id="fc024-660">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="fc024-660">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="fc024-661">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="fc024-661">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="fc024-662">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="fc024-662">IoT</span></span>
* <span data-ttu-id="fc024-663">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="fc024-663">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc024-664">Key Vault</span><span class="sxs-lookup"><span data-stu-id="fc024-664">Key Vault</span></span>
* <span data-ttu-id="fc024-665">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="fc024-665">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="fc024-666">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-666">Network</span></span>
* <span data-ttu-id="fc024-667">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="fc024-667">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="fc024-668">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-668">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="fc024-669">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="fc024-669">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="fc024-670">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="fc024-670">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="fc024-671">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-671">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="fc024-672">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-672">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="fc024-673">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="fc024-673">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="fc024-674">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="fc024-674">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="fc024-675">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="fc024-675">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="fc024-676">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="fc024-676">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="fc024-677">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="fc024-677">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="fc024-678">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="fc024-678">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="fc024-679">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="fc024-679">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="fc024-680">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="fc024-680">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="fc024-681">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="fc024-681">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="fc024-682">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="fc024-682">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="fc024-683">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="fc024-683">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="fc024-684">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="fc024-684">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc024-685">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="fc024-685">RDBMS</span></span>
* <span data-ttu-id="fc024-686">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="fc024-686">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="fc024-687">резервирование.</span><span class="sxs-lookup"><span data-stu-id="fc024-687">Reservation</span></span>
* <span data-ttu-id="fc024-688">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fc024-688">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="fc024-689">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="fc024-689">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="fc024-690">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="fc024-690">Manage App</span></span>
* <span data-ttu-id="fc024-691">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="fc024-691">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="fc024-692">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="fc024-692">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="fc024-693">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-693">Role</span></span>
* <span data-ttu-id="fc024-694">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="fc024-694">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="fc024-695">SignalR</span><span class="sxs-lookup"><span data-stu-id="fc024-695">SignalR</span></span>
* <span data-ttu-id="fc024-696">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="fc024-696">First release</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-697">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-697">Storage</span></span>
* <span data-ttu-id="fc024-698">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="fc024-698">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="fc024-699">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="fc024-699">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-700">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-700">VM</span></span>
* <span data-ttu-id="fc024-701">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="fc024-701">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="fc024-702">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="fc024-702">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="fc024-703">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-703">August 28, 2018</span></span>

<span data-ttu-id="fc024-704">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="fc024-704">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="fc024-705">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-705">Core</span></span>

* <span data-ttu-id="fc024-706">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="fc024-706">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="fc024-707">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="fc024-707">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-708">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-708">ACR</span></span>

* <span data-ttu-id="fc024-709">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="fc024-709">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="fc024-710">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="fc024-710">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-711">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-711">ACS</span></span>

* <span data-ttu-id="fc024-712">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="fc024-712">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="fc024-713">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="fc024-713">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-714">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-714">AppService</span></span>

* <span data-ttu-id="fc024-715">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="fc024-715">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="fc024-716">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="fc024-716">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="fc024-717">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fc024-717">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="fc024-718">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="fc024-718">Backup</span></span>

* <span data-ttu-id="fc024-719">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fc024-719">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="fc024-720">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="fc024-720">Bot Service</span></span>

* <span data-ttu-id="fc024-721">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="fc024-721">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="fc024-722">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="fc024-722">Cognitive Services</span></span>

* <span data-ttu-id="fc024-723">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="fc024-723">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="fc024-724">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="fc024-724">IoT</span></span>

* <span data-ttu-id="fc024-725">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="fc024-725">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-726">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-726">Monitor</span></span>

* <span data-ttu-id="fc024-727">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="fc024-727">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="fc024-728">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="fc024-728">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="fc024-729">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-729">Network</span></span>

* <span data-ttu-id="fc024-730">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fc024-730">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-731">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-731">Resource</span></span>

* <span data-ttu-id="fc024-732">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fc024-732">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-733">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-733">Storage</span></span>

* <span data-ttu-id="fc024-734">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fc024-734">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-735">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-735">VM</span></span>

* <span data-ttu-id="fc024-736">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="fc024-736">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="fc024-737">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-737">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="fc024-738">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-738">Auguest 14, 2018</span></span>

<span data-ttu-id="fc024-739">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="fc024-739">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="fc024-740">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-740">Core</span></span>

* <span data-ttu-id="fc024-741">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="fc024-741">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="fc024-742">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="fc024-742">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="fc024-743">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="fc024-743">Telemetry</span></span>

* <span data-ttu-id="fc024-744">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="fc024-744">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-745">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-745">ACR</span></span>

* <span data-ttu-id="fc024-746">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="fc024-746">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="fc024-747">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="fc024-747">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-748">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-748">ACS</span></span>

* <span data-ttu-id="fc024-749">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="fc024-749">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="fc024-750">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="fc024-750">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="fc024-751">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="fc024-751">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="fc024-752">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="fc024-752">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="fc024-753">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="fc024-753">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="fc024-754">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-754">AppService</span></span>

* <span data-ttu-id="fc024-755">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fc024-755">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="fc024-756">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="fc024-756">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="fc024-757">Batch AI</span><span class="sxs-lookup"><span data-stu-id="fc024-757">BatchAI</span></span>

* <span data-ttu-id="fc024-758">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="fc024-758">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="fc024-759">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-759">Container</span></span>

* <span data-ttu-id="fc024-760">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="fc024-760">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="fc024-761">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="fc024-761">IoT</span></span>

* <span data-ttu-id="fc024-762">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="fc024-762">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="fc024-763">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="fc024-763">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="fc024-764">IoT Central</span><span class="sxs-lookup"><span data-stu-id="fc024-764">Iot Central</span></span>

* <span data-ttu-id="fc024-765">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="fc024-765">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc024-766">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="fc024-766">KeyVault</span></span>


* <span data-ttu-id="fc024-767">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="fc024-767">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="fc024-768">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="fc024-768">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="fc024-769">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="fc024-769">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="fc024-770">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="fc024-770">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="fc024-771">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="fc024-771">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="fc024-772">Передача</span><span class="sxs-lookup"><span data-stu-id="fc024-772">Relay</span></span>

* <span data-ttu-id="fc024-773">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="fc024-773">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-774">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-774">Sql</span></span>

* <span data-ttu-id="fc024-775">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="fc024-775">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-776">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-776">Storage</span></span>

* <span data-ttu-id="fc024-777">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="fc024-777">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="fc024-778">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="fc024-778">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="fc024-779">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="fc024-779">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="fc024-780">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="fc024-780">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="fc024-781">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="fc024-781">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-782">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-782">VM</span></span>

* <span data-ttu-id="fc024-783">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="fc024-783">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="fc024-784">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-784">July 31, 2018</span></span>

<span data-ttu-id="fc024-785">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="fc024-785">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-786">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-786">ACR</span></span>

* <span data-ttu-id="fc024-787">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="fc024-787">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="fc024-788">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="fc024-788">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-789">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-789">ACS</span></span>

* <span data-ttu-id="fc024-790">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="fc024-790">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="fc024-791">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-791">Batch</span></span>

* <span data-ttu-id="fc024-792">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="fc024-792">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="fc024-793">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-793">Container</span></span>

* <span data-ttu-id="fc024-794">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="fc024-794">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="fc024-795">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-795">Network</span></span>

* <span data-ttu-id="fc024-796">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="fc024-796">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="fc024-797">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-797">Resource</span></span>

* <span data-ttu-id="fc024-798">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="fc024-798">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="fc024-799">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="fc024-799">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="fc024-800">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-800">Role</span></span>

* <span data-ttu-id="fc024-801">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="fc024-801">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="fc024-802">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="fc024-802">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="fc024-803">поиска</span><span class="sxs-lookup"><span data-stu-id="fc024-803">Search</span></span>

* <span data-ttu-id="fc024-804">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="fc024-804">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="fc024-805">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-805">Service Bus</span></span>

* <span data-ttu-id="fc024-806">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="fc024-806">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="fc024-807">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="fc024-807">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="fc024-808">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="fc024-808">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="fc024-809">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="fc024-809">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-810">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-810">Storage</span></span>

* <span data-ttu-id="fc024-811">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="fc024-811">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="fc024-812">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="fc024-812">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-813">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-813">VM</span></span>

* <span data-ttu-id="fc024-814">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="fc024-814">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="fc024-815">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="fc024-815">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="fc024-816">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="fc024-816">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="fc024-817">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="fc024-817">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="fc024-818">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-818">July 18, 2018</span></span>

<span data-ttu-id="fc024-819">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="fc024-819">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="fc024-820">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-820">Core</span></span>

* <span data-ttu-id="fc024-821">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="fc024-821">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="fc024-822">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="fc024-822">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="fc024-823">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="fc024-823">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-824">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-824">ACR</span></span>

* <span data-ttu-id="fc024-825">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="fc024-825">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="fc024-826">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-826">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="fc024-827">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="fc024-827">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="fc024-828">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="fc024-828">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-829">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-829">ACS</span></span>

* <span data-ttu-id="fc024-830">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="fc024-830">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-831">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-831">AppService</span></span>

* <span data-ttu-id="fc024-832">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="fc024-832">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="fc024-833">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-833">Batch</span></span>

* <span data-ttu-id="fc024-834">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="fc024-834">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="fc024-835">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="fc024-835">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="fc024-836">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="fc024-836">Batch AI</span></span>

* <span data-ttu-id="fc024-837">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="fc024-837">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="fc024-838">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-838">Container</span></span>

* <span data-ttu-id="fc024-839">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="fc024-839">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="fc024-840">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="fc024-840">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="fc024-841">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-841">Network</span></span>

* <span data-ttu-id="fc024-842">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-842">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="fc024-843">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-843">Added `network nic wait`</span></span>
* <span data-ttu-id="fc024-844">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="fc024-844">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="fc024-845">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="fc024-845">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="fc024-846">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-846">Resource</span></span>

* <span data-ttu-id="fc024-847">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-847">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="fc024-848">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-848">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="fc024-849">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-849">Added `deployment wait` command</span></span>
* <span data-ttu-id="fc024-850">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="fc024-850">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-851">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-851">SQL</span></span>

* <span data-ttu-id="fc024-852">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-852">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="fc024-853">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="fc024-853">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="fc024-854">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="fc024-854">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-855">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-855">Storage</span></span>

* <span data-ttu-id="fc024-856">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="fc024-856">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-857">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-857">VM</span></span>

* <span data-ttu-id="fc024-858">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-858">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="fc024-859">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-859">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="fc024-860">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-860">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="fc024-861">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-861">July 3, 2018</span></span>

<span data-ttu-id="fc024-862">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="fc024-862">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="fc024-863">AKS</span><span class="sxs-lookup"><span data-stu-id="fc024-863">AKS</span></span>

* <span data-ttu-id="fc024-864">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="fc024-864">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="fc024-865">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-865">July 3, 2018</span></span>

<span data-ttu-id="fc024-866">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="fc024-866">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="fc024-867">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-867">Core</span></span>

* <span data-ttu-id="fc024-868">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="fc024-868">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-869">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-869">ACR</span></span>

* <span data-ttu-id="fc024-870">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="fc024-870">Added polling build status</span></span>
* <span data-ttu-id="fc024-871">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="fc024-871">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="fc024-872">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="fc024-872">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-873">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-873">ACS</span></span>

* <span data-ttu-id="fc024-874">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-874">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="fc024-875">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-875">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="fc024-876">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="fc024-876">Updated options for `aks browse` command.</span></span> <span data-ttu-id="fc024-877">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="fc024-877">Added `--listen-port` support</span></span>
* <span data-ttu-id="fc024-878">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="fc024-878">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="fc024-879">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="fc024-879">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="fc024-880">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="fc024-880">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-881">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-881">AppService</span></span>

* <span data-ttu-id="fc024-882">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="fc024-882">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="fc024-883">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="fc024-883">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="fc024-884">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="fc024-884">Backup</span></span>

* <span data-ttu-id="fc024-885">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="fc024-885">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="fc024-886">Batch AI</span><span class="sxs-lookup"><span data-stu-id="fc024-886">BatchAI</span></span>

* <span data-ttu-id="fc024-887">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="fc024-887">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="fc024-888">Облако</span><span class="sxs-lookup"><span data-stu-id="fc024-888">Cloud</span></span>

* <span data-ttu-id="fc024-889">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="fc024-889">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="fc024-890">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-890">Container</span></span>

* <span data-ttu-id="fc024-891">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="fc024-891">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="fc024-892">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="fc024-892">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="fc024-893">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="fc024-893">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="fc024-894">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="fc024-894">Extension</span></span>

* <span data-ttu-id="fc024-895">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="fc024-895">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="fc024-896">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-896">Network</span></span>

* <span data-ttu-id="fc024-897">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="fc024-897">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc024-898">Rdbms</span><span class="sxs-lookup"><span data-stu-id="fc024-898">Rdbms</span></span>

* <span data-ttu-id="fc024-899">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="fc024-899">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-900">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-900">Resource</span></span>

* <span data-ttu-id="fc024-901">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="fc024-901">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-902">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-902">VM</span></span>

* <span data-ttu-id="fc024-903">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="fc024-903">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="fc024-904">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-904">June 25, 2018</span></span>

<span data-ttu-id="fc024-905">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="fc024-905">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="fc024-906">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="fc024-906">CLI</span></span>

* <span data-ttu-id="fc024-907">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="fc024-907">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="fc024-908">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-908">June 19, 2018</span></span>

<span data-ttu-id="fc024-909">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="fc024-909">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="fc024-910">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-910">Core</span></span>

* <span data-ttu-id="fc024-911">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="fc024-911">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-912">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-912">ACR</span></span>

* <span data-ttu-id="fc024-913">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="fc024-913">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="fc024-914">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="fc024-914">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-915">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-915">ACS</span></span>

* <span data-ttu-id="fc024-916">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="fc024-916">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="fc024-917">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-917">Added `--update` support</span></span>
* <span data-ttu-id="fc024-918">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="fc024-918">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="fc024-919">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="fc024-919">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="fc024-920">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="fc024-920">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="fc024-921">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="fc024-921">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="fc024-922">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="fc024-922">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="fc024-923">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="fc024-923">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-924">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-924">AppService</span></span>

* <span data-ttu-id="fc024-925">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="fc024-925">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="fc024-926">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fc024-926">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="fc024-927">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-927">Batch</span></span>

* <span data-ttu-id="fc024-928">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="fc024-928">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="fc024-929">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="fc024-929">Batch AI</span></span>

* <span data-ttu-id="fc024-930">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="fc024-930">Added support for workspaces.</span></span> <span data-ttu-id="fc024-931">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fc024-931">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="fc024-932">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="fc024-932">Added support for experiments.</span></span> <span data-ttu-id="fc024-933">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="fc024-933">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="fc024-934">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="fc024-934">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="fc024-935">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="fc024-935">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="fc024-936">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="fc024-936">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="fc024-937">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="fc024-937">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="fc024-938">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="fc024-938">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="fc024-939">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="fc024-939">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="fc024-940">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-940">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="fc024-941">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="fc024-941">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="fc024-942">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-942">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="fc024-943">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="fc024-943">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="fc024-944">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="fc024-944">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="fc024-945">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="fc024-945">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="fc024-946">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-946">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="fc024-947">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="fc024-947">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="fc024-948">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="fc024-948">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="fc024-949">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="fc024-949">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="fc024-950">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="fc024-950">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="fc024-951">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="fc024-951">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="fc024-952">Карты</span><span class="sxs-lookup"><span data-stu-id="fc024-952">Maps</span></span>

* <span data-ttu-id="fc024-953">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="fc024-953">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="fc024-954">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-954">Network</span></span>

* <span data-ttu-id="fc024-955">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="fc024-955">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="fc024-956">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="fc024-956">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="fc024-957">#6502</span><span class="sxs-lookup"><span data-stu-id="fc024-957">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="fc024-958">Резервирование</span><span class="sxs-lookup"><span data-stu-id="fc024-958">Reservations</span></span>

* <span data-ttu-id="fc024-959">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-959">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="fc024-960">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-960">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="fc024-961">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="fc024-961">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="fc024-962">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="fc024-962">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="fc024-963">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="fc024-963">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="fc024-964">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-964">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="fc024-965">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-965">Role</span></span>

* <span data-ttu-id="fc024-966">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="fc024-966">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-967">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-967">SQL</span></span>

* <span data-ttu-id="fc024-968">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="fc024-968">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-969">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-969">Storage</span></span>

* <span data-ttu-id="fc024-970">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="fc024-970">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-971">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-971">VM</span></span>

* <span data-ttu-id="fc024-972">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-972">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="fc024-973">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="fc024-973">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="fc024-974">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="fc024-974">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="fc024-975">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-975">June 13, 2018</span></span>

<span data-ttu-id="fc024-976">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="fc024-976">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="fc024-977">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-977">Core</span></span>

* <span data-ttu-id="fc024-978">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="fc024-978">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="fc024-979">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-979">June 13, 2018</span></span>

<span data-ttu-id="fc024-980">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="fc024-980">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="fc024-981">AKS</span><span class="sxs-lookup"><span data-stu-id="fc024-981">AKS</span></span>

* <span data-ttu-id="fc024-982">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="fc024-982">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="fc024-983">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="fc024-983">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="fc024-984">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="fc024-984">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="fc024-985">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="fc024-985">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="fc024-986">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fc024-986">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-987">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-987">AppService</span></span>

* <span data-ttu-id="fc024-988">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="fc024-988">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="fc024-989">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-989">June 5, 2018</span></span>

<span data-ttu-id="fc024-990">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="fc024-990">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-991">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc024-991">Interactive</span></span>

* <span data-ttu-id="fc024-992">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="fc024-992">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="fc024-993">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-993">June 5, 2018</span></span>

<span data-ttu-id="fc024-994">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="fc024-994">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="fc024-995">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-995">Core</span></span>

* <span data-ttu-id="fc024-996">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="fc024-996">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="fc024-997">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="fc024-997">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-998">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-998">ACR</span></span>

* <span data-ttu-id="fc024-999">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="fc024-999">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="fc024-1000">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1000">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="fc024-1001">AKS</span><span class="sxs-lookup"><span data-stu-id="fc024-1001">AKS</span></span>

* <span data-ttu-id="fc024-1002">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="fc024-1002">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="fc024-1003">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-1003">Batch</span></span>

* <span data-ttu-id="fc024-1004">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="fc024-1004">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="fc024-1005">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="fc024-1005">IOT</span></span>

* <span data-ttu-id="fc024-1006">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="fc024-1006">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1007">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1007">Network</span></span>

* <span data-ttu-id="fc024-1008">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1008">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="fc024-1009">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="fc024-1009">Policy Insights</span></span>

* <span data-ttu-id="fc024-1010">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="fc024-1010">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="fc024-1011">ARM</span><span class="sxs-lookup"><span data-stu-id="fc024-1011">ARM</span></span>

* <span data-ttu-id="fc024-1012">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1012">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-1013">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-1013">SQL</span></span>

* <span data-ttu-id="fc024-1014">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="fc024-1014">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="fc024-1015">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="fc024-1015">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="fc024-1016">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1016">Storage</span></span>

* <span data-ttu-id="fc024-1017">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1017">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1018">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1018">VM</span></span>

* <span data-ttu-id="fc024-1019">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1019">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="fc024-1020">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1020">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="fc024-1021">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1021">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="fc024-1022">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1022">May 22, 2018</span></span>

<span data-ttu-id="fc024-1023">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="fc024-1023">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="fc024-1024">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-1024">Core</span></span>

* <span data-ttu-id="fc024-1025">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1025">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1026">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1026">ACS</span></span>

* <span data-ttu-id="fc024-1027">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1027">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="fc024-1028">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="fc024-1028">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1029">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-1029">AppService</span></span>

* <span data-ttu-id="fc024-1030">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="fc024-1030">Improved generic update commands</span></span>
* <span data-ttu-id="fc024-1031">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1031">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="fc024-1032">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-1032">Container</span></span>

* <span data-ttu-id="fc024-1033">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="fc024-1033">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="fc024-1034">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1034">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="fc024-1035">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="fc024-1035">Extension</span></span>

* <span data-ttu-id="fc024-1036">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="fc024-1036">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-1037">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc024-1037">Interactive</span></span>

* <span data-ttu-id="fc024-1038">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="fc024-1038">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="fc024-1039">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="fc024-1039">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc024-1040">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="fc024-1040">KeyVault</span></span>

* <span data-ttu-id="fc024-1041">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="fc024-1041">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1042">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1042">Network</span></span>

* <span data-ttu-id="fc024-1043">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="fc024-1043">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="fc024-1044">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="fc024-1044">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-1045">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-1045">SQL</span></span>

* <span data-ttu-id="fc024-1046">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="fc024-1046">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="fc024-1047">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1047">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="fc024-1048">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1048">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="fc024-1049">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="fc024-1049">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="fc024-1050">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="fc024-1050">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="fc024-1051">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1051">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="fc024-1052">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1052">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="fc024-1053">`edition`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1053">`edition`.</span></span> <span data-ttu-id="fc024-1054">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1054">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="fc024-1055">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1055">`elasticPoolName`.</span></span> <span data-ttu-id="fc024-1056">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1056">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="fc024-1057">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="fc024-1057">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="fc024-1058">`edition`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1058">`edition`.</span></span> <span data-ttu-id="fc024-1059">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1059">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="fc024-1060">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1060">`dtu`.</span></span> <span data-ttu-id="fc024-1061">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1061">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="fc024-1062">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1062">`databaseDtuMin`.</span></span> <span data-ttu-id="fc024-1063">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1063">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="fc024-1064">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1064">`databaseDtuMax`.</span></span> <span data-ttu-id="fc024-1065">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1065">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="fc024-1066">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1066">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="fc024-1067">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1067">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1068">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1068">Storage</span></span>

* <span data-ttu-id="fc024-1069">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1069">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="fc024-1070">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1070">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1071">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1071">VM</span></span>

* <span data-ttu-id="fc024-1072">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1072">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="fc024-1073">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1073">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="fc024-1074">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1074">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="fc024-1075">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="fc024-1075">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="fc024-1076">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1076">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="fc024-1077">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1077">May 7, 2018</span></span>

<span data-ttu-id="fc024-1078">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="fc024-1078">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="fc024-1079">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-1079">Core</span></span>

* <span data-ttu-id="fc024-1080">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="fc024-1080">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="fc024-1081">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1081">Added limited support for positional arguments</span></span>
* <span data-ttu-id="fc024-1082">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1082">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="fc024-1083">#5591</span><span class="sxs-lookup"><span data-stu-id="fc024-1083">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="fc024-1084">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1084">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="fc024-1085">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="fc024-1085">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="fc024-1086">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="fc024-1086">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="fc024-1087">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1087">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="fc024-1088">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="fc024-1088">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-1089">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-1089">ACR</span></span>

* <span data-ttu-id="fc024-1090">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="fc024-1090">Added ACR Build commands</span></span>
* <span data-ttu-id="fc024-1091">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="fc024-1091">Improved resource not found error messages</span></span>
* <span data-ttu-id="fc024-1092">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="fc024-1092">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="fc024-1093">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="fc024-1093">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="fc024-1094">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="fc024-1094">Improved repository commands error messages</span></span>
* <span data-ttu-id="fc024-1095">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="fc024-1095">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1096">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1096">ACS</span></span>

* <span data-ttu-id="fc024-1097">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-1097">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="fc024-1098">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="fc024-1098">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="fc024-1099">AMS</span><span class="sxs-lookup"><span data-stu-id="fc024-1099">AMS</span></span>

* <span data-ttu-id="fc024-1100">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="fc024-1100">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1101">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1101">Appservice</span></span>

* <span data-ttu-id="fc024-1102">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="fc024-1102">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="fc024-1103">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1103">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="fc024-1104">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="fc024-1104">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="fc024-1105">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1105">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="fc024-1106">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="fc024-1106">Batch AI</span></span>

* <span data-ttu-id="fc024-1107">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="fc024-1107">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="fc024-1108">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="fc024-1108">Cognitive Services</span></span>

* <span data-ttu-id="fc024-1109">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="fc024-1109">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="fc024-1110">Потребление</span><span class="sxs-lookup"><span data-stu-id="fc024-1110">Consumption</span></span>

* <span data-ttu-id="fc024-1111">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="fc024-1111">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="fc024-1112">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-1112">Container</span></span>

* <span data-ttu-id="fc024-1113">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="fc024-1113">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="fc024-1114">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="fc024-1114">Cosmos DB</span></span>

* <span data-ttu-id="fc024-1115">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc024-1115">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="fc024-1116">DMS</span><span class="sxs-lookup"><span data-stu-id="fc024-1116">DMS</span></span>

* <span data-ttu-id="fc024-1117">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="fc024-1117">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="fc024-1118">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="fc024-1118">Extension</span></span>

* <span data-ttu-id="fc024-1119">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="fc024-1119">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-1120">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc024-1120">Interactive</span></span>

* <span data-ttu-id="fc024-1121">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="fc024-1121">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="fc024-1122">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="fc024-1122">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="fc024-1123">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="fc024-1123">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="fc024-1124">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="fc024-1124">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="fc024-1125">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="fc024-1125">Lab</span></span>

* <span data-ttu-id="fc024-1126">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="fc024-1126">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1127">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1127">Network</span></span>

* <span data-ttu-id="fc024-1128">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="fc024-1128">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="fc024-1129">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-1129">Profile</span></span>

* <span data-ttu-id="fc024-1130">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1130">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="fc024-1131">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="fc024-1131">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="fc024-1132">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1132">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="fc024-1133">Redis</span><span class="sxs-lookup"><span data-stu-id="fc024-1133">Redis</span></span>

* <span data-ttu-id="fc024-1134">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1134">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="fc024-1135">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="fc024-1135">Deprecated `redis list-all`.</span></span> <span data-ttu-id="fc024-1136">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1136">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="fc024-1137">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1137">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="fc024-1138">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="fc024-1138">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="fc024-1139">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-1139">Role</span></span>

* <span data-ttu-id="fc024-1140">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="fc024-1140">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1141">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1141">Storage</span></span>

* <span data-ttu-id="fc024-1142">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="fc024-1142">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="fc024-1143">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="fc024-1143">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="fc024-1144">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="fc024-1144">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="fc024-1145">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="fc024-1145">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="fc024-1146">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="fc024-1146">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1147">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1147">VM</span></span>

* <span data-ttu-id="fc024-1148">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="fc024-1148">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="fc024-1149">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="fc024-1149">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="fc024-1150">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="fc024-1150">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="fc024-1151">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1151">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="fc024-1152">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="fc024-1152">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="fc024-1153">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="fc024-1153">Added write accelerator support</span></span>
* <span data-ttu-id="fc024-1154">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1154">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="fc024-1155">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="fc024-1155">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="fc024-1156">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="fc024-1156">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="fc024-1157">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1157">April 10, 2018</span></span>

<span data-ttu-id="fc024-1158">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="fc024-1158">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-1159">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-1159">ACR</span></span>

* <span data-ttu-id="fc024-1160">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="fc024-1160">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1161">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1161">ACS</span></span>

* <span data-ttu-id="fc024-1162">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="fc024-1162">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1163">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1163">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="fc024-1165">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="fc024-1165">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="fc024-1166">Batch AI</span><span class="sxs-lookup"><span data-stu-id="fc024-1166">BatchAI</span></span>

* <span data-ttu-id="fc024-1167">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="fc024-1167">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="fc024-1168">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="fc024-1168">Job level mounting</span></span>
  - <span data-ttu-id="fc024-1169">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1169">Environment variables with secret values</span></span>
  - <span data-ttu-id="fc024-1170">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="fc024-1170">Performance counters settings</span></span>
  - <span data-ttu-id="fc024-1171">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="fc024-1171">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="fc024-1172">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1172">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="fc024-1173">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="fc024-1173">Usage and limits reporting</span></span>
  - <span data-ttu-id="fc024-1174">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1174">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="fc024-1175">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1175">Support for custom images</span></span>
  - <span data-ttu-id="fc024-1176">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="fc024-1176">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="fc024-1177">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="fc024-1177">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="fc024-1178">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1178">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="fc024-1179">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="fc024-1179">National clouds are supported</span></span>
* <span data-ttu-id="fc024-1180">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="fc024-1180">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="fc024-1181">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="fc024-1181">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="fc024-1182">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="fc024-1182">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="fc024-1183">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="fc024-1183">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="fc024-1184">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="fc024-1184">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="fc024-1185">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="fc024-1185">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="fc024-1186">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1186">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="fc024-1187">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="fc024-1187">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="fc024-1188">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="fc024-1188">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="fc024-1189">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1189">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="fc024-1190">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="fc024-1190">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="fc024-1191">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1191">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="fc024-1192">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1192">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="fc024-1193">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="fc024-1193">Billing</span></span>

* <span data-ttu-id="fc024-1194">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="fc024-1194">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="fc024-1195">Потребление</span><span class="sxs-lookup"><span data-stu-id="fc024-1195">Consumption</span></span>

* <span data-ttu-id="fc024-1196">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1196">Added `marketplace` commands</span></span>
* <span data-ttu-id="fc024-1197">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1197">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="fc024-1198">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1198">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="fc024-1199">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1199">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="fc024-1200">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1200">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="fc024-1201">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1201">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="fc024-1202">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-1202">Container</span></span>

* <span data-ttu-id="fc024-1203">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1203">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="fc024-1204">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="fc024-1204">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="fc024-1205">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="fc024-1205">Extension</span></span>

* <span data-ttu-id="fc024-1206">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="fc024-1206">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-1207">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc024-1207">Interactive</span></span>

* <span data-ttu-id="fc024-1208">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="fc024-1208">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="fc024-1209">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="fc024-1209">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="fc024-1210">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1210">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1211">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1211">Network</span></span>

* <span data-ttu-id="fc024-1212">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1212">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="fc024-1213">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1213">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="fc024-1214">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="fc024-1214">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="fc024-1215">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="fc024-1215">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="fc024-1216">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="fc024-1216">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="fc024-1217">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1217">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="fc024-1218">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1218">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="fc024-1219">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="fc024-1219">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="fc024-1220">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-1220">Profile</span></span>

* <span data-ttu-id="fc024-1221">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1221">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="fc024-1222">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1222">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc024-1223">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="fc024-1223">RDBMS</span></span>

* <span data-ttu-id="fc024-1224">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1224">Added `georestore` command</span></span>
* <span data-ttu-id="fc024-1225">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="fc024-1225">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-1226">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-1226">Resource</span></span>

* <span data-ttu-id="fc024-1227">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1227">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="fc024-1228">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1228">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-1229">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-1229">SQL</span></span>

* <span data-ttu-id="fc024-1230">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1230">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1231">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1231">Storage</span></span>

* <span data-ttu-id="fc024-1232">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="fc024-1232">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1233">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1233">VM</span></span>

* <span data-ttu-id="fc024-1234">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="fc024-1234">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="fc024-1235">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="fc024-1235">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="fc024-1237">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1237">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="fc024-1238">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="fc024-1238">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="fc024-1239">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="fc024-1239">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="fc024-1240">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="fc024-1240">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="fc024-1241">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1241">March 27, 2018</span></span>

<span data-ttu-id="fc024-1242">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="fc024-1242">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="fc024-1243">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-1243">Core</span></span>

* <span data-ttu-id="fc024-1244">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="fc024-1244">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1245">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1245">ACS</span></span>

* <span data-ttu-id="fc024-1246">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="fc024-1246">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1247">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1247">Appservice</span></span>

* <span data-ttu-id="fc024-1248">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1248">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="fc024-1249">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1249">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="fc024-1250">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="fc024-1250">Backup</span></span>

* <span data-ttu-id="fc024-1251">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1251">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="fc024-1252">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="fc024-1252">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="fc024-1253">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="fc024-1253">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="fc024-1254">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1254">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="fc024-1255">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-1255">Container</span></span>

* <span data-ttu-id="fc024-1256">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1256">Added `container exec` command.</span></span> <span data-ttu-id="fc024-1257">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1257">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="fc024-1258">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1258">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="fc024-1259">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="fc024-1259">Extension</span></span>

* <span data-ttu-id="fc024-1260">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="fc024-1260">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="fc024-1261">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1261">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="fc024-1262">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-1262">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-1263">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc024-1263">Interactive</span></span>

* <span data-ttu-id="fc024-1264">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="fc024-1264">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="fc024-1265">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1265">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="fc024-1266">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="fc024-1266">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="fc024-1267">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="fc024-1267">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="fc024-1268">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="fc024-1268">Lab</span></span>

* <span data-ttu-id="fc024-1269">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1269">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-1270">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-1270">Monitor</span></span>

* <span data-ttu-id="fc024-1271">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="fc024-1271">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="fc024-1272">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="fc024-1272">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="fc024-1273">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="fc024-1273">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1274">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1274">Network</span></span>

* <span data-ttu-id="fc024-1275">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="fc024-1275">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="fc024-1276">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-1276">Profile</span></span>

* <span data-ttu-id="fc024-1277">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1277">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc024-1278">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="fc024-1278">RDBMS</span></span>

* <span data-ttu-id="fc024-1279">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="fc024-1279">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-1280">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-1280">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="fc024-1282">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-1282">Role</span></span>

* <span data-ttu-id="fc024-1283">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1283">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="fc024-1284">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="fc024-1284">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="fc024-1285">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="fc024-1285">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="fc024-1286">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1286">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="fc024-1287">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1287">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1288">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1288">Storage</span></span>

* <span data-ttu-id="fc024-1289">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="fc024-1289">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="fc024-1290">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="fc024-1290">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1291">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1291">VM</span></span>

* <span data-ttu-id="fc024-1292">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1292">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="fc024-1293">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1293">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="fc024-1294">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="fc024-1294">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="fc024-1295">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="fc024-1295">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="fc024-1296">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1296">March 13, 2018</span></span>

<span data-ttu-id="fc024-1297">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="fc024-1297">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-1298">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-1298">ACR</span></span>

* <span data-ttu-id="fc024-1299">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1299">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="fc024-1300">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="fc024-1300">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="fc024-1301">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="fc024-1301">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1302">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1302">ACS</span></span>

* <span data-ttu-id="fc024-1303">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="fc024-1303">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="fc024-1304">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="fc024-1304">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="fc024-1305">Помощник</span><span class="sxs-lookup"><span data-stu-id="fc024-1305">Advisor</span></span>

* <span data-ttu-id="fc024-1306">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1306">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="fc024-1307">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1307">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="fc024-1308">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1308">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="fc024-1309">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1309">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="fc024-1310">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1310">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1311">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1311">Appservice</span></span>

* <span data-ttu-id="fc024-1312">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="fc024-1312">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="fc024-1313">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1313">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="fc024-1314">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="fc024-1314">Eventhubs</span></span>

* <span data-ttu-id="fc024-1315">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="fc024-1315">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="fc024-1316">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="fc024-1316">Extension</span></span>

* <span data-ttu-id="fc024-1317">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="fc024-1317">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-1318">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc024-1318">Interactive</span></span>

* <span data-ttu-id="fc024-1319">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="fc024-1319">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="fc024-1320">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="fc024-1320">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="fc024-1321">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="fc024-1321">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="fc024-1322">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="fc024-1322">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-1323">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-1323">Monitor</span></span>

* <span data-ttu-id="fc024-1324">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="fc024-1324">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="fc024-1325">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1325">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="fc024-1326">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1326">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="fc024-1327">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1327">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1328">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1328">Network</span></span>

* <span data-ttu-id="fc024-1329">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1329">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="fc024-1330">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="fc024-1330">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="fc024-1331">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1331">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="fc024-1332">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1332">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="fc024-1333">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-1333">Profile</span></span>

* <span data-ttu-id="fc024-1334">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="fc024-1334">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="fc024-1335">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1335">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc024-1336">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="fc024-1336">RDBMS</span></span>

* <span data-ttu-id="fc024-1337">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="fc024-1337">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="fc024-1338">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-1338">Service Bus</span></span>

* <span data-ttu-id="fc024-1339">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="fc024-1339">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1340">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1340">Storage</span></span>

* <span data-ttu-id="fc024-1341">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="fc024-1341">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="fc024-1342">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="fc024-1342">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1343">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1343">VM</span></span>

* <span data-ttu-id="fc024-1344">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="fc024-1344">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="fc024-1345">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="fc024-1345">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="fc024-1346">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1346">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="fc024-1347">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="fc024-1347">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="fc024-1348">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="fc024-1348">February 27, 2018</span></span>

<span data-ttu-id="fc024-1349">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="fc024-1349">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="fc024-1350">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-1350">Core</span></span>

* <span data-ttu-id="fc024-1351">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="fc024-1351">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="fc024-1352">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="fc024-1352">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="fc024-1353">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1353">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1354">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1354">ACS</span></span>

* <span data-ttu-id="fc024-1355">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-1355">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="fc024-1356">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="fc024-1356">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="fc024-1357">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1357">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="fc024-1358">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1358">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1359">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1359">Appservice</span></span>

* <span data-ttu-id="fc024-1360">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="fc024-1360">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="fc024-1361">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="fc024-1361">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="fc024-1362">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="fc024-1362">Cognitive Services</span></span>

* <span data-ttu-id="fc024-1363">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="fc024-1363">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="fc024-1364">Потребление</span><span class="sxs-lookup"><span data-stu-id="fc024-1364">Consumption</span></span>

* <span data-ttu-id="fc024-1365">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="fc024-1365">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="fc024-1366">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="fc024-1366">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="fc024-1367">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-1367">Container</span></span>

* <span data-ttu-id="fc024-1368">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="fc024-1368">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1369">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1369">Network</span></span>

* <span data-ttu-id="fc024-1370">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1370">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-1371">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-1371">Resource</span></span>

* <span data-ttu-id="fc024-1372">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="fc024-1372">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="fc024-1373">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-1373">Role</span></span>

* <span data-ttu-id="fc024-1374">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-1374">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-1375">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-1375">SQL</span></span>

* <span data-ttu-id="fc024-1376">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1376">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1377">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1377">Storage</span></span>

* <span data-ttu-id="fc024-1378">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1378">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1379">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1379">VM</span></span>

* <span data-ttu-id="fc024-1380">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="fc024-1380">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="fc024-1381">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1381">February 13, 2018</span></span>

<span data-ttu-id="fc024-1382">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="fc024-1382">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="fc024-1383">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-1383">Core</span></span>

* <span data-ttu-id="fc024-1384">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="fc024-1384">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1385">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1385">ACS</span></span>

* <span data-ttu-id="fc024-1386">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="fc024-1386">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="fc024-1387">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1387">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="fc024-1388">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="fc024-1388">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="fc024-1389">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="fc024-1389">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="fc024-1390">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="fc024-1390">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="fc024-1391">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1391">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="fc024-1392">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="fc024-1392">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="fc024-1393">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1393">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1394">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1394">Appservice</span></span>

* <span data-ttu-id="fc024-1395">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="fc024-1395">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="fc024-1396">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1396">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="fc024-1397">CDN</span><span class="sxs-lookup"><span data-stu-id="fc024-1397">CDN</span></span>

* <span data-ttu-id="fc024-1398">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1398">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="fc024-1399">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-1399">Container</span></span>

* <span data-ttu-id="fc024-1400">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="fc024-1400">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="fc024-1401">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1401">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc024-1402">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc024-1402">CosmosDB</span></span>

* <span data-ttu-id="fc024-1403">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1403">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="fc024-1404">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="fc024-1404">Extension</span></span>

* <span data-ttu-id="fc024-1405">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1405">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="fc024-1406">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1406">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="fc024-1407">Отзыв</span><span class="sxs-lookup"><span data-stu-id="fc024-1407">Feedback</span></span>

* <span data-ttu-id="fc024-1408">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="fc024-1408">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-1409">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc024-1409">Interactive</span></span>

* <span data-ttu-id="fc024-1410">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="fc024-1410">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="fc024-1411">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1411">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="fc024-1412">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="fc024-1412">IoT</span></span>

* <span data-ttu-id="fc024-1413">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="fc024-1413">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="fc024-1414">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="fc024-1414">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="fc024-1415">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1415">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="fc024-1416">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="fc024-1416">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-1417">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-1417">Monitor</span></span>

* <span data-ttu-id="fc024-1418">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1418">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1419">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1419">Network</span></span>

* <span data-ttu-id="fc024-1420">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="fc024-1420">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="fc024-1421">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-1421">Profile</span></span>

* <span data-ttu-id="fc024-1422">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="fc024-1422">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-1423">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-1423">Resource</span></span>

* <span data-ttu-id="fc024-1424">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1424">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="fc024-1425">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-1425">Role</span></span>

* <span data-ttu-id="fc024-1426">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="fc024-1426">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-1427">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-1427">SQL</span></span>

* <span data-ttu-id="fc024-1428">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1428">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="fc024-1429">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1429">Added `sql db rename`</span></span>
* <span data-ttu-id="fc024-1430">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="fc024-1430">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1431">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1431">Storage</span></span>

* <span data-ttu-id="fc024-1432">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="fc024-1432">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1433">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1433">VM</span></span>

* <span data-ttu-id="fc024-1434">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="fc024-1434">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="fc024-1435">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="fc024-1435">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="fc024-1436">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="fc024-1436">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="fc024-1437">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1437">January 31, 2018</span></span>

<span data-ttu-id="fc024-1438">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="fc024-1438">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="fc024-1439">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-1439">Core</span></span>

* <span data-ttu-id="fc024-1440">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="fc024-1440">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="fc024-1441">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="fc024-1441">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="fc024-1442">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="fc024-1442">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="fc024-1443">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="fc024-1443">Use `--verbose` to see</span></span>
* <span data-ttu-id="fc024-1444">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="fc024-1444">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1445">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1445">ACS</span></span>

* <span data-ttu-id="fc024-1446">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1446">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="fc024-1447">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1447">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1448">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1448">Appservice</span></span>

* <span data-ttu-id="fc024-1449">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="fc024-1449">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="fc024-1450">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="fc024-1450">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="fc024-1451">CDN</span><span class="sxs-lookup"><span data-stu-id="fc024-1451">CDN</span></span>

* <span data-ttu-id="fc024-1452">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1452">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc024-1453">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc024-1453">CosmosDB</span></span>

* <span data-ttu-id="fc024-1454">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="fc024-1454">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-1455">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc024-1455">Interactive</span></span>

* <span data-ttu-id="fc024-1456">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="fc024-1456">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1457">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1457">Network</span></span>

* <span data-ttu-id="fc024-1458">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1458">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="fc024-1459">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-1459">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="fc024-1460">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1460">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="fc024-1461">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1461">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="fc024-1462">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1462">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="fc024-1463">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="fc024-1463">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="fc024-1464">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="fc024-1464">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="fc024-1465">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="fc024-1465">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="fc024-1466">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1466">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="fc024-1467">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1467">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="fc024-1468">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-1468">Profile</span></span>

* <span data-ttu-id="fc024-1469">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="fc024-1469">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-1470">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-1470">Resource</span></span>

* <span data-ttu-id="fc024-1471">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="fc024-1471">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1472">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1472">Storage</span></span>

* <span data-ttu-id="fc024-1473">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="fc024-1473">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="fc024-1474">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="fc024-1474">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="fc024-1475">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1475">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="fc024-1476">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1476">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="fc024-1477">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="fc024-1477">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1478">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1478">VM</span></span>

* <span data-ttu-id="fc024-1479">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="fc024-1479">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="fc024-1480">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1480">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="fc024-1481">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="fc024-1481">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="fc024-1482">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1482">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="fc024-1483">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1483">January 17, 2018</span></span>

<span data-ttu-id="fc024-1484">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="fc024-1484">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-1485">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-1485">ACR</span></span>

* <span data-ttu-id="fc024-1486">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="fc024-1486">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="fc024-1487">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="fc024-1487">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1488">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1488">ACS</span></span>

* <span data-ttu-id="fc024-1489">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1489">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="fc024-1490">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-1490">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1491">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1491">Appservice</span></span>

* <span data-ttu-id="fc024-1492">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="fc024-1492">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="fc024-1493">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1493">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="fc024-1494">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1494">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="fc024-1495">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="fc024-1495">Backup</span></span>

* <span data-ttu-id="fc024-1496">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="fc024-1496">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="fc024-1497">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="fc024-1497">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="fc024-1498">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="fc024-1498">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="fc024-1499">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="fc024-1499">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="fc024-1500">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="fc024-1500">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="fc024-1501">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-1501">Batch</span></span>

* <span data-ttu-id="fc024-1502">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="fc024-1502">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="fc024-1503">Облако</span><span class="sxs-lookup"><span data-stu-id="fc024-1503">Cloud</span></span>

* <span data-ttu-id="fc024-1504">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="fc024-1504">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="fc024-1505">Потребление</span><span class="sxs-lookup"><span data-stu-id="fc024-1505">Consumption</span></span>

* <span data-ttu-id="fc024-1506">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1506">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="fc024-1507">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-1507">Event Grid</span></span>

* <span data-ttu-id="fc024-1508">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1508">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="fc024-1509">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1509">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="fc024-1510">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1510">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="fc024-1511">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1511">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="fc024-1512">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1512">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="fc024-1513">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1513">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="fc024-1514">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1514">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="fc024-1515">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1515">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-1516">Interactive</span><span class="sxs-lookup"><span data-stu-id="fc024-1516">Interactive</span></span>

* <span data-ttu-id="fc024-1517">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="fc024-1517">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="fc024-1518">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="fc024-1518">Fixed errors on startup</span></span>
* <span data-ttu-id="fc024-1519">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="fc024-1519">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="fc024-1520">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="fc024-1520">IoT</span></span>

* <span data-ttu-id="fc024-1521">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="fc024-1521">Added support for device provisioning service</span></span>
* <span data-ttu-id="fc024-1522">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="fc024-1522">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="fc024-1523">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="fc024-1523">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-1524">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-1524">Monitor</span></span>

* <span data-ttu-id="fc024-1525">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="fc024-1525">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="fc024-1526">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1526">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="fc024-1527">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="fc024-1527">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1528">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1528">Network</span></span>

* <span data-ttu-id="fc024-1529">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="fc024-1529">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="fc024-1530">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="fc024-1530">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="fc024-1531">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-1531">Profile</span></span>

* <span data-ttu-id="fc024-1532">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="fc024-1532">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="fc024-1533">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-1533">Role</span></span>

* <span data-ttu-id="fc024-1534">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1534">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fc024-1535">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fc024-1535">Service Fabric</span></span>

* <span data-ttu-id="fc024-1536">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="fc024-1536">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="fc024-1537">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="fc024-1537">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1538">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1538">VM</span></span>

* <span data-ttu-id="fc024-1539">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1539">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="fc024-1540">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="fc024-1540">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="fc024-1541">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1541">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="fc024-1542">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="fc024-1542">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="fc024-1543">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="fc024-1543">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="fc024-1544">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1544">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="fc024-1545">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1545">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="fc024-1546">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1546">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="fc024-1547">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1547">December 19, 2017</span></span>

<span data-ttu-id="fc024-1548">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="fc024-1548">Version 2.0.23</span></span>

* <span data-ttu-id="fc024-1549">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="fc024-1549">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="fc024-1550">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-1550">Container</span></span>

* <span data-ttu-id="fc024-1551">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1551">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1552">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1552">Network</span></span>

* <span data-ttu-id="fc024-1553">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fc024-1553">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="fc024-1554">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fc024-1554">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1555">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1555">Storage</span></span>

* <span data-ttu-id="fc024-1556">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="fc024-1556">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1557">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1557">VM</span></span>

* <span data-ttu-id="fc024-1558">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="fc024-1558">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="fc024-1559">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1559">December 5, 2017</span></span>

<span data-ttu-id="fc024-1560">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="fc024-1560">Version 2.0.22</span></span>

* <span data-ttu-id="fc024-1561">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1561">Removed `az component` commands.</span></span> <span data-ttu-id="fc024-1562">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1562">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="fc024-1563">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-1563">Core</span></span>
* <span data-ttu-id="fc024-1564">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="fc024-1564">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="fc024-1565">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="fc024-1565">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1566">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1566">ACS</span></span>

* <span data-ttu-id="fc024-1567">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1567">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="fc024-1568">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1568">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="fc024-1569">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="fc024-1569">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="fc024-1570">Помощник</span><span class="sxs-lookup"><span data-stu-id="fc024-1570">Advisor</span></span>

* <span data-ttu-id="fc024-1571">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="fc024-1571">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1572">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1572">Appservice</span></span>

* <span data-ttu-id="fc024-1573">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1573">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="fc024-1574">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="fc024-1574">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="fc024-1575">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1575">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="fc024-1576">Потребление</span><span class="sxs-lookup"><span data-stu-id="fc024-1576">Consumption</span></span>

* <span data-ttu-id="fc024-1577">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="fc024-1577">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="fc024-1578">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-1578">Container</span></span>

* <span data-ttu-id="fc024-1579">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="fc024-1579">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-1580">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-1580">Monitor</span></span>

* <span data-ttu-id="fc024-1581">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="fc024-1581">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-1582">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-1582">Resource</span></span>

* <span data-ttu-id="fc024-1583">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="fc024-1583">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="fc024-1584">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-1584">Role</span></span>

* <span data-ttu-id="fc024-1585">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1585">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="fc024-1586">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="fc024-1586">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="fc024-1587">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1587">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-1588">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-1588">SQL</span></span>

* <span data-ttu-id="fc024-1589">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1589">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="fc024-1590">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1590">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1591">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1591">VM</span></span>

* <span data-ttu-id="fc024-1592">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1592">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="fc024-1593">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1593">November 14, 2017</span></span>

<span data-ttu-id="fc024-1594">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="fc024-1594">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-1595">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-1595">ACR</span></span>

* <span data-ttu-id="fc024-1596">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="fc024-1596">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="fc024-1597">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1597">ACS</span></span>

* <span data-ttu-id="fc024-1598">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="fc024-1598">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="fc024-1599">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="fc024-1599">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="fc024-1600">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1600">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="fc024-1601">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="fc024-1601">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="fc024-1602">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="fc024-1602">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1603">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1603">Appservice</span></span>

* <span data-ttu-id="fc024-1604">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="fc024-1604">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="fc024-1605">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1605">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="fc024-1606">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1606">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="fc024-1607">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1607">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="fc024-1608">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="fc024-1608">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="fc024-1609">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="fc024-1609">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="fc024-1610">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-1610">Batch</span></span>

* <span data-ttu-id="fc024-1611">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1611">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="fc024-1612">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="fc024-1612">Batchai</span></span>

* <span data-ttu-id="fc024-1613">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1613">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="fc024-1614">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1614">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="fc024-1615">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1615">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="fc024-1616">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1616">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="fc024-1617">Облако</span><span class="sxs-lookup"><span data-stu-id="fc024-1617">Cloud</span></span>

* <span data-ttu-id="fc024-1618">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="fc024-1618">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="fc024-1619">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-1619">Container</span></span>

* <span data-ttu-id="fc024-1620">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1620">Added support to open multiple ports</span></span>
* <span data-ttu-id="fc024-1621">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1621">Added container group restart policy</span></span>
* <span data-ttu-id="fc024-1622">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="fc024-1622">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="fc024-1623">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="fc024-1623">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="fc024-1624">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="fc024-1624">Data Lake Analytics</span></span>

* <span data-ttu-id="fc024-1625">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="fc024-1625">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="fc024-1626">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fc024-1626">Data Lake Store</span></span>

* <span data-ttu-id="fc024-1627">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="fc024-1627">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="fc024-1628">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="fc024-1628">Extension</span></span>

* <span data-ttu-id="fc024-1629">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="fc024-1629">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="fc024-1630">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="fc024-1630">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="fc024-1631">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="fc024-1631">IoT</span></span>

* <span data-ttu-id="fc024-1632">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1632">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-1633">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-1633">Monitor</span></span>

* <span data-ttu-id="fc024-1634">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1634">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1635">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1635">Network</span></span>

* <span data-ttu-id="fc024-1636">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="fc024-1636">Added support for CAA DNS records</span></span>
* <span data-ttu-id="fc024-1637">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1637">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="fc024-1638">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="fc024-1638">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="fc024-1639">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1639">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="fc024-1640">Резервирование</span><span class="sxs-lookup"><span data-stu-id="fc024-1640">Reservations</span></span>

* <span data-ttu-id="fc024-1641">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="fc024-1641">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-1642">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-1642">Resource</span></span>

* <span data-ttu-id="fc024-1643">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1643">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-1644">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-1644">SQL</span></span>

* <span data-ttu-id="fc024-1645">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1645">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1646">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1646">Storage</span></span>

* <span data-ttu-id="fc024-1647">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-1647">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="fc024-1648">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="fc024-1648">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="fc024-1649">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1649">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="fc024-1650">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1650">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="fc024-1651">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1651">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="fc024-1652">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1652">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="fc024-1653">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1653">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1654">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1654">VM</span></span>

* <span data-ttu-id="fc024-1655">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1655">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="fc024-1656">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1656">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="fc024-1657">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1657">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="fc024-1658">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1658">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="fc024-1659">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="fc024-1659">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="fc024-1660">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1660">October 24, 2017</span></span>

<span data-ttu-id="fc024-1661">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="fc024-1661">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="fc024-1662">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-1662">Core</span></span>

* <span data-ttu-id="fc024-1663">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="fc024-1663">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-1664">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-1664">ACR</span></span>

* <span data-ttu-id="fc024-1665">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="fc024-1665">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="fc024-1666">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="fc024-1666">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="fc024-1667">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="fc024-1667">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1668">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1668">ACS</span></span>

* <span data-ttu-id="fc024-1669">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="fc024-1669">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="fc024-1670">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="fc024-1670">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1671">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1671">Appservice</span></span>

* <span data-ttu-id="fc024-1672">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="fc024-1672">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="fc024-1673">Компонент</span><span class="sxs-lookup"><span data-stu-id="fc024-1673">Component</span></span>

* <span data-ttu-id="fc024-1674">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="fc024-1674">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-1675">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-1675">Monitor</span></span>

* <span data-ttu-id="fc024-1676">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1676">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-1677">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-1677">Resource</span></span>

* <span data-ttu-id="fc024-1678">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="fc024-1678">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="fc024-1679">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="fc024-1679">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1680">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1680">VM</span></span>

* <span data-ttu-id="fc024-1681">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="fc024-1681">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="fc024-1682">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1682">October 9, 2017</span></span>

<span data-ttu-id="fc024-1683">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="fc024-1683">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="fc024-1684">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-1684">Core</span></span>

* <span data-ttu-id="fc024-1685">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="fc024-1685">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1686">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1686">Appservice</span></span>

* <span data-ttu-id="fc024-1687">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1687">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="fc024-1688">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-1688">Batch</span></span>

* <span data-ttu-id="fc024-1689">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="fc024-1689">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="fc024-1690">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="fc024-1690">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="fc024-1691">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-1691">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="fc024-1692">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1692">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="fc024-1693">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="fc024-1693">Batchai</span></span>

* <span data-ttu-id="fc024-1694">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="fc024-1694">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc024-1695">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="fc024-1695">Keyvault</span></span>

* <span data-ttu-id="fc024-1696">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="fc024-1696">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="fc024-1697">(#4448)</span><span class="sxs-lookup"><span data-stu-id="fc024-1697">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="fc024-1698">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1698">Network</span></span>

* <span data-ttu-id="fc024-1699">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="fc024-1699">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="fc024-1700">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="fc024-1700">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-1701">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-1701">Resource</span></span>

* <span data-ttu-id="fc024-1702">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1702">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="fc024-1703">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="fc024-1703">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="fc024-1704">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="fc024-1704">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="fc024-1705">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="fc024-1705">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-1706">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-1706">Sql</span></span>

* <span data-ttu-id="fc024-1707">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="fc024-1707">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="fc024-1708">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="fc024-1708">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="fc024-1709">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="fc024-1709">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1710">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1710">Storage</span></span>

* <span data-ttu-id="fc024-1711">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1711">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1712">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="fc024-1712">Vm</span></span>

* <span data-ttu-id="fc024-1713">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1713">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="fc024-1714">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1714">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="fc024-1715">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1715">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="fc024-1716">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1716">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="fc024-1717">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="fc024-1717">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="fc024-1718">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1718">September 22, 2017</span></span>

<span data-ttu-id="fc024-1719">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="fc024-1719">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-1720">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-1720">Resource</span></span>

* <span data-ttu-id="fc024-1721">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="fc024-1721">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="fc024-1722">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="fc024-1722">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="fc024-1723">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="fc024-1723">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="fc024-1724">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1724">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1725">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1725">Network</span></span>

* <span data-ttu-id="fc024-1726">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="fc024-1726">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="fc024-1727">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="fc024-1727">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="fc024-1728">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="fc024-1728">Added `asg` application security group commands</span></span>
* <span data-ttu-id="fc024-1729">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="fc024-1729">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="fc024-1730">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fc024-1730">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="fc024-1731">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fc024-1731">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="fc024-1732">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1732">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1733">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1733">Storage</span></span>

* <span data-ttu-id="fc024-1734">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="fc024-1734">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="fc024-1735">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="fc024-1735">Eventgrid</span></span>

* <span data-ttu-id="fc024-1736">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="fc024-1736">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-1737">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-1737">SQL</span></span>

* <span data-ttu-id="fc024-1738">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="fc024-1738">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="fc024-1739">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="fc024-1739">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="fc024-1740">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="fc024-1740">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc024-1741">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="fc024-1741">Keyvault</span></span>

* <span data-ttu-id="fc024-1742">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="fc024-1742">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1743">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1743">VM</span></span>

* <span data-ttu-id="fc024-1744">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="fc024-1744">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="fc024-1745">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="fc024-1745">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="fc024-1746">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="fc024-1746">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="fc024-1747">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="fc024-1747">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="fc024-1748">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="fc024-1748">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="fc024-1749">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="fc024-1749">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1750">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1750">ACS</span></span>

* <span data-ttu-id="fc024-1751">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="fc024-1751">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1752">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1752">Appservice</span></span>

* <span data-ttu-id="fc024-1753">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="fc024-1753">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="fc024-1754">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="fc024-1754">Backup</span></span>

* <span data-ttu-id="fc024-1755">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="fc024-1755">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="fc024-1756">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1756">September 11, 2017</span></span>

<span data-ttu-id="fc024-1757">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="fc024-1757">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="fc024-1758">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-1758">Core</span></span>

* <span data-ttu-id="fc024-1759">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="fc024-1759">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="fc024-1760">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="fc024-1760">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1761">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1761">Acs</span></span>

* <span data-ttu-id="fc024-1762">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1762">Added `acs list-locations` command</span></span>
* <span data-ttu-id="fc024-1763">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-1763">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1764">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1764">Appservice</span></span>

* <span data-ttu-id="fc024-1765">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="fc024-1765">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="fc024-1766">CDN</span><span class="sxs-lookup"><span data-stu-id="fc024-1766">CDN</span></span>

* <span data-ttu-id="fc024-1767">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1767">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="fc024-1768">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="fc024-1768">Extension</span></span>

* <span data-ttu-id="fc024-1769">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="fc024-1769">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc024-1770">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="fc024-1770">Keyvault</span></span>

* <span data-ttu-id="fc024-1771">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1771">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1772">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1772">Network</span></span>

* <span data-ttu-id="fc024-1773">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1773">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="fc024-1774">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1774">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="fc024-1775">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1775">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="fc024-1776">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1776">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="fc024-1777">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1777">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-1778">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-1778">Resource</span></span>

* <span data-ttu-id="fc024-1779">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1779">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="fc024-1780">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1780">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="fc024-1781">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1781">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="fc024-1782">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="fc024-1782">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-1783">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-1783">SQL</span></span>

* <span data-ttu-id="fc024-1784">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1784">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1785">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1785">VM</span></span>

* <span data-ttu-id="fc024-1786">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="fc024-1786">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="fc024-1787">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="fc024-1787">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="fc024-1788">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1788">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="fc024-1789">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="fc024-1789">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="fc024-1790">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="fc024-1790">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="fc024-1791">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1791">August 31, 2017</span></span>

<span data-ttu-id="fc024-1792">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="fc024-1792">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc024-1793">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="fc024-1793">Keyvault</span></span>

* <span data-ttu-id="fc024-1794">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1794">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="fc024-1795">Sf</span><span class="sxs-lookup"><span data-stu-id="fc024-1795">Sf</span></span>

* <span data-ttu-id="fc024-1796">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="fc024-1796">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1797">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1797">Storage</span></span>

* <span data-ttu-id="fc024-1798">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="fc024-1798">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="fc024-1799">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="fc024-1799">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="fc024-1800">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1800">August 28, 2017</span></span>

<span data-ttu-id="fc024-1801">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="fc024-1801">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="fc024-1802">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="fc024-1802">CLI</span></span>

* <span data-ttu-id="fc024-1803">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="fc024-1803">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1804">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1804">ACS</span></span>

* <span data-ttu-id="fc024-1805">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="fc024-1805">Corrected preview regions</span></span>
* <span data-ttu-id="fc024-1806">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1806">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="fc024-1807">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="fc024-1807">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1808">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1808">Appservice</span></span>

* <span data-ttu-id="fc024-1809">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1809">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="fc024-1810">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1810">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="fc024-1811">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1811">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="fc024-1812">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="fc024-1812">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="fc024-1813">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="fc024-1813">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="fc024-1814">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="fc024-1814">IoT</span></span>

* <span data-ttu-id="fc024-1815">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="fc024-1815">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1816">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1816">Network</span></span>

* <span data-ttu-id="fc024-1817">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1817">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="fc024-1818">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1818">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="fc024-1819">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1819">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="fc024-1820">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1820">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="fc024-1821">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1821">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="fc024-1822">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-1822">Profile</span></span>

* <span data-ttu-id="fc024-1823">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="fc024-1823">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fc024-1824">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fc024-1824">Service Fabric</span></span>

* <span data-ttu-id="fc024-1825">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="fc024-1825">Preview release</span></span>
* <span data-ttu-id="fc024-1826">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="fc024-1826">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="fc024-1827">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="fc024-1827">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="fc024-1828">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1828">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1829">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1829">Storage</span></span>

* <span data-ttu-id="fc024-1830">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="fc024-1830">Enabled setting blob tier</span></span>
* <span data-ttu-id="fc024-1831">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-1831">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="fc024-1832">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1832">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="fc024-1833">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="fc024-1833">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="fc024-1834">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1834">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="fc024-1835">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1835">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1836">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1836">VM</span></span>

* <span data-ttu-id="fc024-1837">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1837">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="fc024-1838">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1838">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="fc024-1839">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="fc024-1839">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="fc024-1840">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="fc024-1840">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="fc024-1841">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="fc024-1841">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="fc024-1842">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1842">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="fc024-1843">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1843">August 15, 2017</span></span>

<span data-ttu-id="fc024-1844">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="fc024-1844">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1845">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1845">ACS</span></span>

* <span data-ttu-id="fc024-1846">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="fc024-1846">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1847">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1847">Appservice</span></span>

* <span data-ttu-id="fc024-1848">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="fc024-1848">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="fc024-1849">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-1849">Event Grid</span></span>

* <span data-ttu-id="fc024-1850">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="fc024-1850">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="fc024-1851">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1851">August 11, 2017</span></span>

<span data-ttu-id="fc024-1852">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="fc024-1852">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1853">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1853">ACS</span></span>

* <span data-ttu-id="fc024-1854">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="fc024-1854">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="fc024-1855">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-1855">Batch</span></span>

* <span data-ttu-id="fc024-1856">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="fc024-1856">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="fc024-1857">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="fc024-1857">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="fc024-1858">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1858">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="fc024-1859">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="fc024-1859">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="fc024-1860">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="fc024-1860">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="fc024-1861">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="fc024-1861">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="fc024-1862">Компонент</span><span class="sxs-lookup"><span data-stu-id="fc024-1862">Component</span></span>

* <span data-ttu-id="fc024-1863">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="fc024-1863">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="fc024-1864">Контейнер</span><span class="sxs-lookup"><span data-stu-id="fc024-1864">Container</span></span>

* <span data-ttu-id="fc024-1865">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="fc024-1865">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="fc024-1866">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fc024-1866">Data Lake Store</span></span>

* <span data-ttu-id="fc024-1867">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="fc024-1867">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="fc024-1868">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-1868">Event Grid</span></span>

* <span data-ttu-id="fc024-1869">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="fc024-1869">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1870">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1870">Network</span></span>

* <span data-ttu-id="fc024-1871">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="fc024-1871">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="fc024-1872">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1872">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="fc024-1873">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1873">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="fc024-1874">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1874">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="fc024-1875">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-1875">Profile</span></span>

* <span data-ttu-id="fc024-1876">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="fc024-1876">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-1877">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-1877">Storage</span></span>

* <span data-ttu-id="fc024-1878">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="fc024-1878">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-1879">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-1879">VM</span></span>

* <span data-ttu-id="fc024-1880">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="fc024-1880">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="fc024-1881">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1881">Exposed `list-skus` command</span></span>
* <span data-ttu-id="fc024-1882">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="fc024-1882">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="fc024-1883">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="fc024-1883">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="fc024-1884">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="fc024-1884">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="fc024-1885">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-1885">July 28, 2017</span></span>

<span data-ttu-id="fc024-1886">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="fc024-1886">Version 2.0.12</span></span>

* <span data-ttu-id="fc024-1887">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1887">Added container commands</span></span>
* <span data-ttu-id="fc024-1888">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1888">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="fc024-1889">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-1889">Core</span></span>

* <span data-ttu-id="fc024-1890">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="fc024-1890">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="fc024-1891">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="fc024-1891">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="fc024-1892">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="fc024-1892">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="fc024-1893">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="fc024-1893">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="fc024-1894">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="fc024-1894">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="fc024-1895">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="fc024-1895">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="fc024-1896">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="fc024-1896">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="fc024-1897">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="fc024-1897">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="fc024-1898">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="fc024-1898">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="fc024-1899">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="fc024-1899">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="fc024-1900">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="fc024-1900">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="fc024-1901">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="fc024-1901">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="fc024-1902">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="fc024-1902">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="fc024-1903">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="fc024-1903">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="fc024-1904">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="fc024-1904">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="fc024-1905">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="fc024-1905">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="fc024-1906">ACR</span><span class="sxs-lookup"><span data-stu-id="fc024-1906">ACR</span></span>

* <span data-ttu-id="fc024-1907">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1907">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="fc024-1908">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="fc024-1908">Support SKU update for managed registries</span></span>
* <span data-ttu-id="fc024-1909">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="fc024-1909">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="fc024-1910">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="fc024-1910">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="fc024-1911">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="fc024-1911">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="fc024-1912">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="fc024-1912">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-1913">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-1913">ACS</span></span>

* <span data-ttu-id="fc024-1914">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="fc024-1914">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-1915">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="fc024-1915">Appservice</span></span>

* <span data-ttu-id="fc024-1916">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="fc024-1916">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="fc024-1917">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="fc024-1917">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="fc024-1918">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1918">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="fc024-1919">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="fc024-1919">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="fc024-1920">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="fc024-1920">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="fc024-1921">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="fc024-1921">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="fc024-1922">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="fc024-1922">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="fc024-1923">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="fc024-1923">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="fc024-1924">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="fc024-1924">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="fc024-1925">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1925">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="fc024-1926">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="fc024-1926">Batch</span></span>

* <span data-ttu-id="fc024-1927">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="fc024-1927">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="fc024-1928">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1928">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="fc024-1929">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1929">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="fc024-1930">CDN</span><span class="sxs-lookup"><span data-stu-id="fc024-1930">CDN</span></span>

* <span data-ttu-id="fc024-1931">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="fc024-1931">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="fc024-1932">Облако</span><span class="sxs-lookup"><span data-stu-id="fc024-1932">Cloud</span></span>

* <span data-ttu-id="fc024-1933">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="fc024-1933">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="fc024-1934">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="fc024-1934">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="fc024-1935">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="fc024-1935">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="fc024-1936">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="fc024-1936">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="fc024-1937">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1937">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc024-1938">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc024-1938">CosmosDB</span></span>

* <span data-ttu-id="fc024-1939">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="fc024-1939">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="fc024-1940">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="fc024-1940">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="fc024-1941">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="fc024-1941">Data Lake Analytics</span></span>

* <span data-ttu-id="fc024-1942">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1942">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="fc024-1943">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1943">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="fc024-1944">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1944">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="fc024-1945">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fc024-1945">Data Lake Store</span></span>

* <span data-ttu-id="fc024-1946">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1946">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="fc024-1947">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="fc024-1947">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="fc024-1948">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1948">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="fc024-1949">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="fc024-1949">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="fc024-1950">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="fc024-1950">Interactive</span></span>

* <span data-ttu-id="fc024-1951">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="fc024-1951">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="fc024-1952">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="fc024-1952">Increased test coverage</span></span>
* <span data-ttu-id="fc024-1953">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="fc024-1953">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="fc024-1954">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="fc024-1954">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="fc024-1955">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="fc024-1955">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="fc024-1956">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="fc024-1956">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="fc024-1957">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="fc024-1957">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="fc024-1958">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1958">Added `--progress` flag</span></span>
* <span data-ttu-id="fc024-1959">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1959">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="fc024-1960">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="fc024-1960">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="fc024-1961">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="fc024-1961">IoT</span></span>

* <span data-ttu-id="fc024-1962">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="fc024-1962">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="fc024-1963">(3934).</span><span class="sxs-lookup"><span data-stu-id="fc024-1963">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="fc024-1964">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="fc024-1964">Key vault</span></span>

* <span data-ttu-id="fc024-1965">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="fc024-1965">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="fc024-1966">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1966">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="fc024-1967">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="fc024-1967">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="fc024-1968">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="fc024-1968">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="fc024-1969">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1969">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="fc024-1970">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="fc024-1970">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="fc024-1971">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="fc024-1971">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="fc024-1972">(3307).</span><span class="sxs-lookup"><span data-stu-id="fc024-1972">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="fc024-1973">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="fc024-1973">Lab</span></span>

* <span data-ttu-id="fc024-1974">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1974">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="fc024-1975">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1975">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-1976">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-1976">Monitor</span></span>

* <span data-ttu-id="fc024-1977">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="fc024-1977">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="fc024-1978">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1978">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="fc024-1979">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1979">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="fc024-1980">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1980">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="fc024-1981">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1981">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="fc024-1982">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="fc024-1982">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="fc024-1983">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="fc024-1983">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="fc024-1984">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="fc024-1984">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="fc024-1985">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="fc024-1985">`location` no longer required</span></span>
  * <span data-ttu-id="fc024-1986">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="fc024-1986">Add name and ID support for target</span></span>
  * <span data-ttu-id="fc024-1987">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="fc024-1987">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="fc024-1988">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="fc024-1988">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="fc024-1989">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="fc024-1989">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="fc024-1990">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="fc024-1990">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="fc024-1991">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1991">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="fc024-1992">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1992">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="fc024-1993">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-1993">Network</span></span>

* <span data-ttu-id="fc024-1994">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1994">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="fc024-1995">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1995">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="fc024-1996">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="fc024-1996">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="fc024-1997">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1997">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="fc024-1998">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1998">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="fc024-1999">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="fc024-1999">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="fc024-2000">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2000">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="fc024-2001">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2001">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="fc024-2002">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2002">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="fc024-2003">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2003">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="fc024-2004">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2004">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="fc024-2005">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2005">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="fc024-2006">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2006">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="fc024-2007">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2007">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="fc024-2008">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2008">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="fc024-2009">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2009">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="fc024-2010">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="fc024-2010">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="fc024-2011">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2011">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="fc024-2012">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2012">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="fc024-2013">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2013">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="fc024-2014">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2014">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="fc024-2015">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2015">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="fc024-2016">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2016">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="fc024-2017">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="fc024-2017">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="fc024-2018">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="fc024-2018">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="fc024-2019">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="fc024-2019">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="fc024-2020">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="fc024-2020">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="fc024-2021">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-2021">Profile</span></span>

* <span data-ttu-id="fc024-2022">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="fc024-2022">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="fc024-2023">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="fc024-2023">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="fc024-2024">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="fc024-2024">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="fc024-2025">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="fc024-2025">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="fc024-2026">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="fc024-2026">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="fc024-2027">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="fc024-2027">RDBMS</span></span>

* <span data-ttu-id="fc024-2028">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="fc024-2028">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="fc024-2029">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="fc024-2029">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="fc024-2030">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="fc024-2030">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="fc024-2031">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="fc024-2031">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-2032">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-2032">Resource</span></span>

* <span data-ttu-id="fc024-2033">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2033">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="fc024-2034">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2034">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="fc024-2035">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2035">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="fc024-2036">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2036">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="fc024-2037">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="fc024-2037">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="fc024-2038">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2038">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="fc024-2039">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="fc024-2039">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="fc024-2040">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2040">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="fc024-2041">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-2041">Role</span></span>

* <span data-ttu-id="fc024-2042">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="fc024-2042">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="fc024-2043">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="fc024-2043">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="fc024-2044">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="fc024-2044">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="fc024-2045">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="fc024-2045">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="fc024-2046">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2046">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="fc024-2047">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="fc024-2047">Service Fabric</span></span>
* <span data-ttu-id="fc024-2048">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="fc024-2048">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="fc024-2049">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="fc024-2049">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="fc024-2050">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="fc024-2050">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-2051">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-2051">SQL</span></span>

* <span data-ttu-id="fc024-2052">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2052">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="fc024-2053">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2053">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="fc024-2054">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2054">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-2055">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-2055">Storage</span></span>

* <span data-ttu-id="fc024-2056">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="fc024-2056">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="fc024-2057">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="fc024-2057">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="fc024-2058">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="fc024-2058">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="fc024-2059">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="fc024-2059">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="fc024-2060">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="fc024-2060">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="fc024-2061">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="fc024-2061">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-2062">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-2062">VM</span></span>

* <span data-ttu-id="fc024-2063">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="fc024-2063">Support configuring nsg</span></span>
* <span data-ttu-id="fc024-2064">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="fc024-2064">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="fc024-2065">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="fc024-2065">Support managed service identities</span></span>
* <span data-ttu-id="fc024-2066">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2066">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="fc024-2067">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="fc024-2067">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="fc024-2068">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-2068">May 10, 2017</span></span>

<span data-ttu-id="fc024-2069">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="fc024-2069">Version 2.0.6</span></span>

* <span data-ttu-id="fc024-2070">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="fc024-2070">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="fc024-2071">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="fc024-2071">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="fc024-2072">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="fc024-2072">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="fc024-2073">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="fc024-2073">Include Cognitive Services module</span></span>
* <span data-ttu-id="fc024-2074">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="fc024-2074">Include Service Fabric module</span></span>
* <span data-ttu-id="fc024-2075">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="fc024-2075">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="fc024-2076">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="fc024-2076">Add support for CDN commands</span></span>
* <span data-ttu-id="fc024-2077">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="fc024-2077">Remove Container module</span></span>
* <span data-ttu-id="fc024-2078">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2078">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="fc024-2079">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2079">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="fc024-2080">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-2080">Core</span></span>

* <span data-ttu-id="fc024-2081">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="fc024-2081">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="fc024-2082">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2082">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="fc024-2083">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2083">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="fc024-2084">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2084">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="fc024-2085">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2085">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="fc024-2086">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2086">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="fc024-2087">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2087">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="fc024-2088">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2088">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="fc024-2089">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2089">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="fc024-2090">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="fc024-2090">core: Improved performance</span></span>
* <span data-ttu-id="fc024-2091">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="fc024-2091">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="fc024-2092">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="fc024-2092">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-2093">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-2093">ACS</span></span>

* <span data-ttu-id="fc024-2094">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="fc024-2094">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="fc024-2095">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="fc024-2095">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="fc024-2096">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="fc024-2096">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="fc024-2097">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2097">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-2098">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-2098">AppService</span></span>

* <span data-ttu-id="fc024-2099">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="fc024-2099">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="fc024-2100">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="fc024-2100">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="fc024-2101">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="fc024-2101">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="fc024-2102">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="fc024-2102">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="fc024-2103">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="fc024-2103">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="fc024-2104">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2104">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="fc024-2105">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="fc024-2105">support slot swap with preview</span></span>
* <span data-ttu-id="fc024-2106">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2106">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="fc024-2107">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2107">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="fc024-2108">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc024-2108">CosmosDB</span></span>

* <span data-ttu-id="fc024-2109">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="fc024-2109">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="fc024-2110">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="fc024-2110">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="fc024-2111">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="fc024-2111">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="fc024-2112">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="fc024-2112">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="fc024-2113">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="fc024-2113">Data Lake Analytics</span></span>

* <span data-ttu-id="fc024-2114">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="fc024-2114">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="fc024-2115">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="fc024-2115">Add support for new catalog item type: package.</span></span> <span data-ttu-id="fc024-2116">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2116">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="fc024-2117">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="fc024-2117">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="fc024-2118">Таблица</span><span class="sxs-lookup"><span data-stu-id="fc024-2118">Table</span></span>
  * <span data-ttu-id="fc024-2119">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="fc024-2119">Table valued function</span></span>
  * <span data-ttu-id="fc024-2120">Просмотр</span><span class="sxs-lookup"><span data-stu-id="fc024-2120">View</span></span>
  * <span data-ttu-id="fc024-2121">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="fc024-2121">Table Statistics.</span></span> <span data-ttu-id="fc024-2122">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="fc024-2122">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="fc024-2123">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="fc024-2123">Data Lake Store</span></span>

* <span data-ttu-id="fc024-2124">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="fc024-2124">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="fc024-2125">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2125">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="fc024-2126">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="fc024-2126">missed help for access show.</span></span> <span data-ttu-id="fc024-2127">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="fc024-2127">adding it.</span></span> <span data-ttu-id="fc024-2128">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="fc024-2128">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="fc024-2129">Поиск</span><span class="sxs-lookup"><span data-stu-id="fc024-2129">Find</span></span>

* <span data-ttu-id="fc024-2130">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="fc024-2130">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="fc024-2131">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="fc024-2131">KeyVault</span></span>

* <span data-ttu-id="fc024-2132">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="fc024-2132">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="fc024-2133">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="fc024-2133">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="fc024-2134">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="fc024-2134">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="fc024-2135">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="fc024-2135">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="fc024-2136">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2136">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="fc024-2137">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="fc024-2137">Lab</span></span>

* <span data-ttu-id="fc024-2138">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="fc024-2138">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="fc024-2139">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="fc024-2139">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="fc024-2140">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="fc024-2140">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="fc024-2141">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="fc024-2141">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="fc024-2142">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="fc024-2142">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="fc024-2143">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="fc024-2143">Monitor</span></span>

* <span data-ttu-id="fc024-2144">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2144">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="fc024-2145">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2145">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="fc024-2146">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-2146">Network</span></span>

* <span data-ttu-id="fc024-2147">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2147">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="fc024-2148">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2148">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="fc024-2149">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="fc024-2149">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="fc024-2150">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="fc024-2150">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="fc024-2151">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="fc024-2151">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="fc024-2152">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="fc024-2152">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="fc024-2153">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="fc024-2153">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="fc024-2154">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="fc024-2154">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="fc024-2155">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2155">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="fc024-2156">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="fc024-2156">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="fc024-2157">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2157">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="fc024-2158">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2158">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="fc024-2159">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="fc024-2159">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="fc024-2160">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="fc024-2160">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="fc024-2161">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="fc024-2161">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="fc024-2162">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="fc024-2162">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="fc024-2163">Профиль</span><span class="sxs-lookup"><span data-stu-id="fc024-2163">Profile</span></span>

* <span data-ttu-id="fc024-2164">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2164">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="fc024-2165">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2165">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="fc024-2166">Redis</span><span class="sxs-lookup"><span data-stu-id="fc024-2166">Redis</span></span>

* <span data-ttu-id="fc024-2167">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="fc024-2167">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="fc024-2168">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="fc024-2168">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="fc024-2169">Ресурс</span><span class="sxs-lookup"><span data-stu-id="fc024-2169">Resource</span></span>

* <span data-ttu-id="fc024-2170">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2170">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="fc024-2171">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2171">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="fc024-2172">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2172">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="fc024-2173">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="fc024-2173">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="fc024-2174">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="fc024-2174">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="fc024-2175">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="fc024-2175">Add docs for az lock update.</span></span> <span data-ttu-id="fc024-2176">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="fc024-2176">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="fc024-2177">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="fc024-2177">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="fc024-2178">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="fc024-2178">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="fc024-2179">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="fc024-2179">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="fc024-2180">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="fc024-2180">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="fc024-2181">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2181">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="fc024-2182">Роль</span><span class="sxs-lookup"><span data-stu-id="fc024-2182">Role</span></span>

* <span data-ttu-id="fc024-2183">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2183">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="fc024-2184">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2184">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="fc024-2185">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2185">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="fc024-2186">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="fc024-2186">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="fc024-2187">SQL</span><span class="sxs-lookup"><span data-stu-id="fc024-2187">SQL</span></span>

* <span data-ttu-id="fc024-2188">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="fc024-2188">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="fc024-2189">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2189">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="fc024-2190">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-2190">Storage</span></span>

* <span data-ttu-id="fc024-2191">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2191">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="fc024-2192">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="fc024-2192">Add support for incremental blob copy</span></span>
* <span data-ttu-id="fc024-2193">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="fc024-2193">Add support for large block blob upload</span></span>
* <span data-ttu-id="fc024-2194">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="fc024-2194">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-2195">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-2195">VM</span></span>

* <span data-ttu-id="fc024-2196">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="fc024-2196">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="fc024-2197">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="fc024-2197">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="fc024-2198">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="fc024-2198">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="fc024-2199">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="fc024-2199">az vm/vmss disk</span></span>
  3. <span data-ttu-id="fc024-2200">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="fc024-2200">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="fc024-2201">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="fc024-2201">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="fc024-2202">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2202">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="fc024-2203">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-2203">April 3, 2017</span></span>

<span data-ttu-id="fc024-2204">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="fc024-2204">Version 2.0.2</span></span>

<span data-ttu-id="fc024-2205">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="fc024-2205">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="fc024-2206">Core</span><span class="sxs-lookup"><span data-stu-id="fc024-2206">Core</span></span>

* <span data-ttu-id="fc024-2207">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-2207">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="fc024-2208">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2208">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="fc024-2209">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2209">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="fc024-2210">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2210">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="fc024-2211">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2211">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="fc024-2212">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="fc024-2212">Add prompting for missing template parameters.</span></span> <span data-ttu-id="fc024-2213">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2213">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="fc024-2214">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc024-2214">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="fc024-2215">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="fc024-2215">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="fc024-2216">ACS</span><span class="sxs-lookup"><span data-stu-id="fc024-2216">ACS</span></span>

* <span data-ttu-id="fc024-2217">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2217">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="fc024-2218">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="fc024-2218">Add support for ssh key password prompting.</span></span> <span data-ttu-id="fc024-2219">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2219">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="fc024-2220">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="fc024-2220">Add support for windows clusters.</span></span> <span data-ttu-id="fc024-2221">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2221">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="fc024-2222">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="fc024-2222">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="fc024-2223">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2223">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="fc024-2224">AppService</span><span class="sxs-lookup"><span data-stu-id="fc024-2224">AppService</span></span>

* <span data-ttu-id="fc024-2225">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2225">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="fc024-2226">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2226">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="fc024-2227">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2227">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="fc024-2228">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2228">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="fc024-2229">Data Lake</span><span class="sxs-lookup"><span data-stu-id="fc024-2229">DataLake</span></span>

* <span data-ttu-id="fc024-2230">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="fc024-2230">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="fc024-2231">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="fc024-2231">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="fc024-2232">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="fc024-2232">DocuemntDB</span></span>

* <span data-ttu-id="fc024-2233">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2233">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="fc024-2234">ВМ</span><span class="sxs-lookup"><span data-stu-id="fc024-2234">VM</span></span>

* <span data-ttu-id="fc024-2235">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2235">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="fc024-2236">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2236">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="fc024-2237">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2237">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="fc024-2238">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2238">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="fc024-2239">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2239">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="fc024-2240">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2240">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="fc024-2241">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="fc024-2241">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="fc024-2242">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="fc024-2242">February 27, 2017</span></span>

<span data-ttu-id="fc024-2243">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="fc024-2243">Version 2.0.0</span></span>

<span data-ttu-id="fc024-2244">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="fc024-2244">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="fc024-2245">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="fc024-2245">Container Service (acs)</span></span>
- <span data-ttu-id="fc024-2246">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="fc024-2246">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="fc024-2247">Сеть</span><span class="sxs-lookup"><span data-stu-id="fc024-2247">Networking</span></span>
- <span data-ttu-id="fc024-2248">Хранилище</span><span class="sxs-lookup"><span data-stu-id="fc024-2248">Storage</span></span>

<span data-ttu-id="fc024-2249">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2249">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="fc024-2250">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="fc024-2250">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="fc024-2251">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="fc024-2251">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="fc024-2252">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="fc024-2252">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="fc024-2253">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="fc024-2253">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="fc024-2254">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="fc024-2254">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="fc024-2255">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="fc024-2255">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="fc024-2256">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="fc024-2256">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="fc024-2257">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="fc024-2257">Provide feedback from the command line with the `az feedback` command</span></span>

