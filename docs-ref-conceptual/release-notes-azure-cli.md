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
ms.openlocfilehash: 9f35084eeecab491e5be63eb856b0bb64a6157d0
ms.sourcegitcommit: 9fb008f2802ca6a58f33e01263bf55a80d01f031
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/27/2019
ms.locfileid: "56891217"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="bde46-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="bde46-103">Azure CLI release notes</span></span>
## <a name="february-26-2019"></a><span data-ttu-id="bde46-104">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-104">February 26, 2019</span></span>

<span data-ttu-id="bde46-105">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="bde46-105">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="bde46-106">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-106">Core</span></span>

* <span data-ttu-id="bde46-107">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="bde46-107">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-108">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-108">ACR</span></span>

* <span data-ttu-id="bde46-109">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-109">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="bde46-110">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="bde46-110">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-111">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-111">ACS</span></span>

* <span data-ttu-id="bde46-112">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="bde46-112">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-113">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-113">AppService</span></span>

* <span data-ttu-id="bde46-114">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="bde46-114">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="bde46-115">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-115">Batch</span></span>
* <span data-ttu-id="bde46-116">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="bde46-116">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="bde46-117">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="bde46-117">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="bde46-118">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="bde46-118">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="bde46-119">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="bde46-119">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="bde46-120">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="bde46-120">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="bde46-121">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bde46-121">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bde46-122">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bde46-122">CosmosDB</span></span>

* <span data-ttu-id="bde46-123">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="bde46-123">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="bde46-124">Kusto</span><span class="sxs-lookup"><span data-stu-id="bde46-124">Kusto</span></span>

* <span data-ttu-id="bde46-125">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="bde46-125">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="bde46-126">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-126">Network</span></span>

* <span data-ttu-id="bde46-127">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bde46-127">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="bde46-128">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="bde46-128">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="bde46-129">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="bde46-129">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="bde46-130">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-130">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="bde46-131">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-131">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="bde46-132">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bde46-132">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="bde46-133">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="bde46-133">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-134">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-134">Resource</span></span>

* <span data-ttu-id="bde46-135">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="bde46-135">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="bde46-136">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-136">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="bde46-137">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-137">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="bde46-138">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-138">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="bde46-139">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="bde46-139">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="bde46-140">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-140">Role</span></span>

* <span data-ttu-id="bde46-141">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-141">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-142">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-142">VM</span></span>

* <span data-ttu-id="bde46-143">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="bde46-143">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="bde46-144">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-144">February 12, 2019</span></span>

<span data-ttu-id="bde46-145">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="bde46-145">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="bde46-146">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-146">Core</span></span>

* <span data-ttu-id="bde46-147">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="bde46-147">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="bde46-148">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="bde46-148">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-149">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-149">ACR</span></span>
* <span data-ttu-id="bde46-150">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="bde46-150">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="bde46-151">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="bde46-151">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-152">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-152">ACS</span></span>
* <span data-ttu-id="bde46-153">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="bde46-153">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="bde46-154">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="bde46-154">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="bde46-155">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="bde46-155">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="bde46-156">AMS</span><span class="sxs-lookup"><span data-stu-id="bde46-156">AMS</span></span>
* <span data-ttu-id="bde46-157">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-157">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="bde46-158">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-158">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-159">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-159">Appservice</span></span>
* <span data-ttu-id="bde46-160">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="bde46-160">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="bde46-161">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="bde46-161">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="bde46-162">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-162">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="bde46-163">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="bde46-163">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="bde46-164">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="bde46-164">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="bde46-165">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="bde46-165">Botservice</span></span>
* <span data-ttu-id="bde46-166">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="bde46-166">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="bde46-167">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="bde46-167">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="bde46-168">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-168">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="bde46-169">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="bde46-169">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="bde46-170">[УСТАРЕЛО.] Аргумент `--proj-name` не поддерживается. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="bde46-170">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="bde46-171">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="bde46-171">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="bde46-172">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="bde46-172">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="bde46-173">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="bde46-173">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="bde46-174">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="bde46-174">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="bde46-175">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="bde46-175">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="bde46-176">Key Vault</span><span class="sxs-lookup"><span data-stu-id="bde46-176">Key Vault</span></span>
* <span data-ttu-id="bde46-177">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="bde46-177">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-178">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-178">Monitor</span></span>
* <span data-ttu-id="bde46-179">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="bde46-179">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="bde46-180">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-180">Network</span></span>
* <span data-ttu-id="bde46-181">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="bde46-181">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="bde46-182">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="bde46-182">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="bde46-183">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="bde46-183">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="bde46-184">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="bde46-184">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="bde46-185">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="bde46-185">Policy Insights</span></span>
* <span data-ttu-id="bde46-186">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bde46-186">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="bde46-187">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bde46-187">RDBMS</span></span>
* <span data-ttu-id="bde46-188">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="bde46-188">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="bde46-189">Redis</span><span class="sxs-lookup"><span data-stu-id="bde46-189">Redis</span></span>
* <span data-ttu-id="bde46-190">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="bde46-190">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="bde46-191">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="bde46-191">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="bde46-192">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="bde46-192">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="bde46-193">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="bde46-193">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="bde46-194">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="bde46-194">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="bde46-195">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="bde46-195">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="bde46-196">[УСТРАРЕЛО.] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bde46-196">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="bde46-197">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-197">Role</span></span>
* <span data-ttu-id="bde46-198">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="bde46-198">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="bde46-199">ВМ SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-199">SQL VM</span></span>
* <span data-ttu-id="bde46-200">[УСТАРЕЛО.] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="bde46-200">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-201">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-201">VM</span></span>
* <span data-ttu-id="bde46-202">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="bde46-202">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="bde46-203">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-203">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="bde46-204">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="bde46-204">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="bde46-205">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="bde46-205">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="bde46-206">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-206">January 31, 2019</span></span>

<span data-ttu-id="bde46-207">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="bde46-207">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="bde46-208">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-208">Core</span></span>

* <span data-ttu-id="bde46-209">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="bde46-209">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="bde46-210">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-210">January 28, 2019</span></span>

<span data-ttu-id="bde46-211">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="bde46-211">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-212">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-212">ACR</span></span>
* <span data-ttu-id="bde46-213">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="bde46-213">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-214">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-214">ACS</span></span>
* <span data-ttu-id="bde46-215">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="bde46-215">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="bde46-216">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="bde46-216">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="bde46-217">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="bde46-217">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="bde46-218">AMS</span><span class="sxs-lookup"><span data-stu-id="bde46-218">AMS</span></span>
* <span data-ttu-id="bde46-219">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="bde46-219">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="bde46-220">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="bde46-220">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-221">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-221">Appservice</span></span>
* <span data-ttu-id="bde46-222">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-222">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="bde46-223">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="bde46-223">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="bde46-224">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="bde46-224">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="bde46-225">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-225">Container</span></span>
* <span data-ttu-id="bde46-226">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="bde46-226">Added `container start` command</span></span>
* <span data-ttu-id="bde46-227">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-227">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="bde46-228">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="bde46-228">EventGrid</span></span>
* <span data-ttu-id="bde46-229">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-229">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="bde46-230">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="bde46-230">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="bde46-231">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="bde46-231">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="bde46-232">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="bde46-232">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="bde46-233">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="bde46-233">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="bde46-234">HDInsight</span><span class="sxs-lookup"><span data-stu-id="bde46-234">HDInsight</span></span>
* <span data-ttu-id="bde46-235">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="bde46-235">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="bde46-236">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="bde46-236">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="bde46-237">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-237">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="bde46-238">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="bde46-238">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="bde46-239">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="bde46-239">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="bde46-240">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-240">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="bde46-241">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bde46-241">IoT</span></span>
* <span data-ttu-id="bde46-242">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="bde46-242">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="bde46-243">Kusto</span><span class="sxs-lookup"><span data-stu-id="bde46-243">Kusto</span></span>
* <span data-ttu-id="bde46-244">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="bde46-244">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-245">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-245">Monitor</span></span>
* <span data-ttu-id="bde46-246">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="bde46-246">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="bde46-247">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-247">Profile</span></span>
* <span data-ttu-id="bde46-248">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-248">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="bde46-249">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-249">Network</span></span>
* <span data-ttu-id="bde46-250">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="bde46-250">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="bde46-251">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="bde46-251">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-252">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-252">Resource</span></span>
* <span data-ttu-id="bde46-253">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-253">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="bde46-254">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-254">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="bde46-255">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-255">SQL Virtual Machine</span></span>
* <span data-ttu-id="bde46-256">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="bde46-256">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-257">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-257">Storage</span></span>
* <span data-ttu-id="bde46-258">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="bde46-258">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="bde46-259">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="bde46-259">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-260">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-260">VM</span></span>
* <span data-ttu-id="bde46-261">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="bde46-261">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="bde46-262">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="bde46-262">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="bde46-263">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-263">January 15, 2019</span></span>

<span data-ttu-id="bde46-264">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="bde46-264">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-265">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-265">ACR</span></span>
* <span data-ttu-id="bde46-266">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="bde46-266">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="bde46-267">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="bde46-267">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="bde46-268">[УСТАРЕЛО.] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="bde46-268">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="bde46-269">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-269">ACS</span></span>
* <span data-ttu-id="bde46-270">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="bde46-270">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-271">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-271">Appservice</span></span>
* <span data-ttu-id="bde46-272">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="bde46-272">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="bde46-273">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="bde46-273">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="bde46-274">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="bde46-274">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="bde46-275">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="bde46-275">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="bde46-276">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="bde46-276">Botservice</span></span>
* <span data-ttu-id="bde46-277">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-277">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="bde46-278">Настройка</span><span class="sxs-lookup"><span data-stu-id="bde46-278">Configure</span></span>
* <span data-ttu-id="bde46-279">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="bde46-279">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bde46-280">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bde46-280">CosmosDB</span></span>
* <span data-ttu-id="bde46-281">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="bde46-281">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="bde46-282">HDInsight</span><span class="sxs-lookup"><span data-stu-id="bde46-282">HDInsight</span></span>
* <span data-ttu-id="bde46-283">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="bde46-283">Added commands for managing applications</span></span>
* <span data-ttu-id="bde46-284">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="bde46-284">Added commands for managing script actions</span></span>
* <span data-ttu-id="bde46-285">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="bde46-285">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="bde46-286">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="bde46-286">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="bde46-287">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-287">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="bde46-288">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-288">Network</span></span>
* <span data-ttu-id="bde46-289">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bde46-289">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="bde46-290">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="bde46-290">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="bde46-291">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bde46-291">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="bde46-292">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-292">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="bde46-293">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-293">Role</span></span>
* <span data-ttu-id="bde46-294">[УСТАРЕЛО.] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bde46-294">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="bde46-295">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="bde46-295">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="bde46-296">Безопасность</span><span class="sxs-lookup"><span data-stu-id="bde46-296">Security</span></span>
* <span data-ttu-id="bde46-297">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bde46-297">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-298">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-298">Storage</span></span>
* <span data-ttu-id="bde46-299">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="bde46-299">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="bde46-300">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="bde46-300">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="bde46-301">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="bde46-301">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="bde46-302">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="bde46-302">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="bde46-303">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="bde46-303">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-304">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-304">VM</span></span>
* <span data-ttu-id="bde46-305">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="bde46-305">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="bde46-306">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-306">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="bde46-307">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="bde46-307">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="bde46-308">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="bde46-308">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="bde46-309">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-309">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="bde46-310">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="bde46-310">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="bde46-311">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-311">December 20, 2018</span></span>

<span data-ttu-id="bde46-312">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="bde46-312">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="bde46-313">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-313">Appservice</span></span>
* <span data-ttu-id="bde46-314">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="bde46-314">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="bde46-315">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="bde46-315">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="bde46-316">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="bde46-316">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="bde46-317">IoT Central</span><span class="sxs-lookup"><span data-stu-id="bde46-317">IoTCentral</span></span>
* <span data-ttu-id="bde46-318">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="bde46-318">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="bde46-319">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-319">Role</span></span>
* <span data-ttu-id="bde46-320">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="bde46-320">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-321">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-321">SQL</span></span>
* <span data-ttu-id="bde46-322">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="bde46-322">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-323">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-323">VM</span></span>
* <span data-ttu-id="bde46-324">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-324">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="bde46-325">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-325">December 18, 2018</span></span>

<span data-ttu-id="bde46-326">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="bde46-326">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="bde46-327">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-327">ACR</span></span>
* <span data-ttu-id="bde46-328">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-328">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="bde46-329">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="bde46-329">Condensed the table layout for task list</span></span>
* <span data-ttu-id="bde46-330">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="bde46-330">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-331">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-331">ACS</span></span>
* <span data-ttu-id="bde46-332">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="bde46-332">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="bde46-333">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="bde46-333">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="bde46-334">[УСТАРЕЛО] Команды `az acs` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="bde46-334">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="bde46-335">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-335">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="bde46-336">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="bde46-336">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="bde46-337">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="bde46-337">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-338">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-338">Appservice</span></span>
* <span data-ttu-id="bde46-339">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="bde46-339">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="bde46-340">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="bde46-340">Botservice</span></span>
* <span data-ttu-id="bde46-341">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-341">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="bde46-342">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="bde46-342">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="bde46-343">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="bde46-343">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="bde46-344">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="bde46-344">Reduced Kudu network calls</span></span>
* <span data-ttu-id="bde46-345">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="bde46-345">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="bde46-346">Потребление</span><span class="sxs-lookup"><span data-stu-id="bde46-346">Consumption</span></span>
* <span data-ttu-id="bde46-347">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="bde46-347">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bde46-348">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bde46-348">CosmosDB</span></span>
* <span data-ttu-id="bde46-349">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="bde46-349">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="bde46-350">Карты</span><span class="sxs-lookup"><span data-stu-id="bde46-350">Maps</span></span>
* <span data-ttu-id="bde46-351">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="bde46-351">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="bde46-352">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-352">Network</span></span>
* <span data-ttu-id="bde46-353">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="bde46-353">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="bde46-354">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="bde46-354">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-355">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-355">Resource</span></span>
* <span data-ttu-id="bde46-356">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-356">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="bde46-357">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-357">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-358">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-358">Storage</span></span>
*  <span data-ttu-id="bde46-359">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="bde46-359">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-360">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-360">VM</span></span>
* <span data-ttu-id="bde46-361">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-361">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="bde46-362">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-362">December 4, 2018</span></span>

<span data-ttu-id="bde46-363">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="bde46-363">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="bde46-364">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-364">Core</span></span>
* <span data-ttu-id="bde46-365">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-365">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="bde46-366">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="bde46-366">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-367">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-367">Appservice</span></span>
* <span data-ttu-id="bde46-368">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="bde46-368">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="bde46-369">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="bde46-369">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="bde46-370">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-370">Network</span></span>
* <span data-ttu-id="bde46-371">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="bde46-371">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="bde46-372">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-372">Role</span></span>
* <span data-ttu-id="bde46-373">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="bde46-373">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="bde46-374">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-374">VM</span></span>
* <span data-ttu-id="bde46-375">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` устарел.</span><span class="sxs-lookup"><span data-stu-id="bde46-375">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="bde46-376">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="bde46-376">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="bde46-377">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="bde46-377">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="bde46-378">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="bde46-378">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="bde46-379">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-379">November 20, 2018</span></span>

<span data-ttu-id="bde46-380">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="bde46-380">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="bde46-381">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-381">Core</span></span>
* <span data-ttu-id="bde46-382">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="bde46-382">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-383">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-383">ACR</span></span>
* <span data-ttu-id="bde46-384">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="bde46-384">Added context token to task step</span></span>
* <span data-ttu-id="bde46-385">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="bde46-385">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="bde46-386">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="bde46-386">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-387">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-387">Appservice</span></span>
* <span data-ttu-id="bde46-388">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="bde46-388">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="bde46-389">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-389">Updated the default `node_version`.</span></span> <span data-ttu-id="bde46-390">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="bde46-390">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="bde46-391">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="bde46-391">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="bde46-392">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="bde46-392">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="bde46-393">IotCentral</span><span class="sxs-lookup"><span data-stu-id="bde46-393">IotCentral</span></span>
* <span data-ttu-id="bde46-394">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="bde46-394">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="bde46-395">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bde46-395">KeyVault</span></span>
* <span data-ttu-id="bde46-396">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="bde46-396">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="bde46-397">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-397">Network</span></span>
* <span data-ttu-id="bde46-398">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="bde46-398">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="bde46-399">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="bde46-399">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="bde46-400">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="bde46-400">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="bde46-401">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="bde46-401">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="bde46-402">Rdbms</span><span class="sxs-lookup"><span data-stu-id="bde46-402">Rdbms</span></span>
* <span data-ttu-id="bde46-403">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="bde46-403">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="bde46-404">RBAC:</span><span class="sxs-lookup"><span data-stu-id="bde46-404">Rbac</span></span>
* <span data-ttu-id="bde46-405">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-405">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="bde46-406">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="bde46-406">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="bde46-407">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-407">Storage</span></span>
* <span data-ttu-id="bde46-408">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="bde46-408">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="bde46-409">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="bde46-409">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="bde46-410">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="bde46-410">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="bde46-411">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="bde46-411">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-412">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-412">VM</span></span>
* <span data-ttu-id="bde46-413">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="bde46-413">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="bde46-414">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="bde46-414">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="bde46-415">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="bde46-415">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="bde46-416">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="bde46-416">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="bde46-417">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-417">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="bde46-418">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-418">Added `snapshot wait` command</span></span>
* <span data-ttu-id="bde46-419">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="bde46-419">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="bde46-420">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-420">November 6, 2018</span></span>

<span data-ttu-id="bde46-421">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="bde46-421">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="bde46-422">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-422">Core</span></span>
* <span data-ttu-id="bde46-423">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="bde46-423">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-424">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-424">ACR</span></span>
* <span data-ttu-id="bde46-425">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="bde46-425">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="bde46-426">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="bde46-426">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-427">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-427">ACS</span></span>
* <span data-ttu-id="bde46-428">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-428">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="bde46-429">Помощник</span><span class="sxs-lookup"><span data-stu-id="bde46-429">Advisor</span></span>
* <span data-ttu-id="bde46-430">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="bde46-430">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="bde46-431">AMS</span><span class="sxs-lookup"><span data-stu-id="bde46-431">AMS</span></span>
* <span data-ttu-id="bde46-432">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="bde46-432">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="bde46-433">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="bde46-433">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="bde46-434">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-434">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="bde46-435">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="bde46-435">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="bde46-436">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="bde46-436">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="bde46-437">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="bde46-437">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="bde46-438">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="bde46-438">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="bde46-439">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="bde46-439">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="bde46-440">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="bde46-440">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="bde46-441">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="bde46-441">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="bde46-442">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="bde46-442">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="bde46-443">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="bde46-443">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="bde46-444">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="bde46-444">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="bde46-445">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="bde46-445">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="bde46-446">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="bde46-446">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="bde46-447">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="bde46-447">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="bde46-448">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="bde46-448">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-449">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-449">AppService</span></span>
* <span data-ttu-id="bde46-450">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="bde46-450">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="bde46-451">Настройка</span><span class="sxs-lookup"><span data-stu-id="bde46-451">Configure</span></span>
* <span data-ttu-id="bde46-452">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="bde46-452">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="bde46-453">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-453">Container</span></span>
* <span data-ttu-id="bde46-454">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="bde46-454">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="bde46-455">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="bde46-455">EventHub</span></span>
* <span data-ttu-id="bde46-456">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-456">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-457">Interactive</span><span class="sxs-lookup"><span data-stu-id="bde46-457">Interactive</span></span>
* <span data-ttu-id="bde46-458">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="bde46-458">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-459">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-459">Monitor</span></span>
* <span data-ttu-id="bde46-460">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-460">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="bde46-461">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-461">Network</span></span>
* <span data-ttu-id="bde46-462">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="bde46-462">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="bde46-463">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="bde46-463">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="bde46-464">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-464">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="bde46-465">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-465">Profile</span></span>
* <span data-ttu-id="bde46-466">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="bde46-466">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="bde46-467">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bde46-467">RDBMS</span></span>
* <span data-ttu-id="bde46-468">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="bde46-468">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-469">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-469">Resource</span></span>
* <span data-ttu-id="bde46-470">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="bde46-470">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="bde46-471">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-471">Role</span></span>
* <span data-ttu-id="bde46-472">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="bde46-472">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="bde46-473">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-473">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="bde46-474">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="bde46-474">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-475">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-475">Storage</span></span>
* <span data-ttu-id="bde46-476">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="bde46-476">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-477">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-477">VM</span></span>
* <span data-ttu-id="bde46-478">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="bde46-478">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="bde46-479">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="bde46-479">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="bde46-480">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="bde46-480">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="bde46-481">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="bde46-481">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="bde46-482">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="bde46-482">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="bde46-483">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="bde46-483">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="bde46-484">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-484">October 23, 2018</span></span>

<span data-ttu-id="bde46-485">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="bde46-485">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="bde46-486">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-486">Core</span></span>
* <span data-ttu-id="bde46-487">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="bde46-487">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="bde46-488">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="bde46-488">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-489">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-489">ACR</span></span>
* <span data-ttu-id="bde46-490">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="bde46-490">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="bde46-491">CDN</span><span class="sxs-lookup"><span data-stu-id="bde46-491">CDN</span></span>
* <span data-ttu-id="bde46-492">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-492">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="bde46-493">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="bde46-493">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="bde46-494">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-494">Container</span></span>
* <span data-ttu-id="bde46-495">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="bde46-495">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="bde46-496">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="bde46-496">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="bde46-497">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bde46-497">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="bde46-498">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-498">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="bde46-499">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="bde46-499">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="bde46-500">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="bde46-500">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="bde46-501">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-501">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bde46-502">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bde46-502">CosmosDB</span></span>
* <span data-ttu-id="bde46-503">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="bde46-503">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-504">Interactive</span><span class="sxs-lookup"><span data-stu-id="bde46-504">Interactive</span></span>
* <span data-ttu-id="bde46-505">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="bde46-505">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="bde46-506">IoT Central</span><span class="sxs-lookup"><span data-stu-id="bde46-506">IoT Central</span></span>
* <span data-ttu-id="bde46-507">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="bde46-507">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="bde46-508">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="bde46-508">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-509">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-509">Monitor</span></span>
* <span data-ttu-id="bde46-510">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="bde46-510">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="bde46-511">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="bde46-511">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="bde46-512">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="bde46-512">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="bde46-513">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="bde46-513">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="bde46-514">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="bde46-514">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="bde46-515">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="bde46-515">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="bde46-516">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="bde46-516">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="bde46-517">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="bde46-517">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="bde46-518">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="bde46-518">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="bde46-519">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-519">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="bde46-520">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-520">Network</span></span>
* <span data-ttu-id="bde46-521">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="bde46-521">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="bde46-522">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="bde46-522">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="bde46-523">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="bde46-523">ServiceBus</span></span>
* <span data-ttu-id="bde46-524">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="bde46-524">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-525">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-525">SQL</span></span>
* <span data-ttu-id="bde46-526">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="bde46-526">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-527">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-527">Storage</span></span>
* <span data-ttu-id="bde46-528">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-528">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="bde46-529">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="bde46-529">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-530">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-530">VM</span></span>
* <span data-ttu-id="bde46-531">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="bde46-531">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="bde46-532">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="bde46-532">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="bde46-533">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="bde46-533">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="bde46-534">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-534">October 16, 2018</span></span>

<span data-ttu-id="bde46-535">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="bde46-535">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-536">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-536">VM</span></span>
* <span data-ttu-id="bde46-537">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="bde46-537">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="bde46-538">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-538">October 9, 2018</span></span>

<span data-ttu-id="bde46-539">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="bde46-539">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="bde46-540">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-540">Core</span></span>
* <span data-ttu-id="bde46-541">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="bde46-541">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-542">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-542">ACR</span></span>
* <span data-ttu-id="bde46-543">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="bde46-543">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-544">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-544">ACS</span></span>
* <span data-ttu-id="bde46-545">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="bde46-545">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="bde46-546">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="bde46-546">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="bde46-547">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="bde46-547">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="bde46-548">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="bde46-548">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="bde46-549">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-549">Container</span></span>
* <span data-ttu-id="bde46-550">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="bde46-550">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="bde46-551">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="bde46-551">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="bde46-552">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="bde46-552">Event Hub</span></span>
* <span data-ttu-id="bde46-553">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-553">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="bde46-554">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="bde46-554">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="bde46-555">расширения.</span><span class="sxs-lookup"><span data-stu-id="bde46-555">Extensions</span></span>
* <span data-ttu-id="bde46-556">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="bde46-556">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="bde46-557">HDInsight</span><span class="sxs-lookup"><span data-stu-id="bde46-557">HDInsight</span></span>
* <span data-ttu-id="bde46-558">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bde46-558">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="bde46-559">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bde46-559">IoT</span></span>
* <span data-ttu-id="bde46-560">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="bde46-560">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="bde46-561">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bde46-561">KeyVault</span></span>
* <span data-ttu-id="bde46-562">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="bde46-562">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="bde46-563">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-563">Network</span></span>
* <span data-ttu-id="bde46-564">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-564">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="bde46-565">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="bde46-565">See #6052</span></span>
* <span data-ttu-id="bde46-566">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-566">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="bde46-567">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="bde46-567">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="bde46-568">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="bde46-568">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="bde46-569">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="bde46-569">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="bde46-570">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="bde46-570">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="bde46-571">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-571">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="bde46-572">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-572">Role</span></span>
* <span data-ttu-id="bde46-573">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="bde46-573">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="bde46-574">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="bde46-574">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="bde46-575">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="bde46-575">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="bde46-576">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="bde46-576">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="bde46-577">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-577">Service Bus</span></span>
* <span data-ttu-id="bde46-578">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="bde46-578">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-579">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-579">VM</span></span>
* <span data-ttu-id="bde46-580">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="bde46-580">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="bde46-581">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="bde46-581">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="bde46-582">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="bde46-582">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="bde46-583">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="bde46-583">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="bde46-584">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="bde46-584">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="bde46-585">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="bde46-585">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="bde46-586">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-586">September 21, 2018</span></span>

<span data-ttu-id="bde46-587">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="bde46-587">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-588">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-588">ACR</span></span>
* <span data-ttu-id="bde46-589">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="bde46-589">Added ACR Task commands</span></span>
* <span data-ttu-id="bde46-590">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="bde46-590">Added quick run command</span></span>
* <span data-ttu-id="bde46-591">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="bde46-591">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="bde46-592">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="bde46-592">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="bde46-593">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="bde46-593">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="bde46-594">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="bde46-594">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-595">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-595">ACS</span></span>
* <span data-ttu-id="bde46-596">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="bde46-596">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="bde46-597">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="bde46-597">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-598">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-598">AppService</span></span>

* <span data-ttu-id="bde46-599">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="bde46-599">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="bde46-600">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="bde46-600">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="bde46-601">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="bde46-601">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="bde46-602">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="bde46-602">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="bde46-603">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-603">Batch</span></span>
* <span data-ttu-id="bde46-604">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="bde46-604">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="bde46-605">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="bde46-605">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="bde46-606">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-606">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="bde46-607">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="bde46-607">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="bde46-608">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bde46-608">Batch AI</span></span> 
* <span data-ttu-id="bde46-609">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-609">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="bde46-610">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="bde46-610">Cognitive Services</span></span>
* <span data-ttu-id="bde46-611">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="bde46-611">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="bde46-612">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="bde46-612">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="bde46-613">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="bde46-613">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="bde46-614">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="bde46-614">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="bde46-615">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="bde46-615">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="bde46-616">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="bde46-616">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="bde46-617">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-617">Container</span></span>
* <span data-ttu-id="bde46-618">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-618">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="bde46-619">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="bde46-619">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="bde46-620">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="bde46-620">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="bde46-621">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-621">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="bde46-622">Data Lake</span><span class="sxs-lookup"><span data-stu-id="bde46-622">Datalake</span></span>
* <span data-ttu-id="bde46-623">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="bde46-623">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="bde46-624">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="bde46-624">Interactive Shell</span></span>
* <span data-ttu-id="bde46-625">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="bde46-625">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="bde46-626">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="bde46-626">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="bde46-627">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bde46-627">IoT</span></span>
* <span data-ttu-id="bde46-628">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="bde46-628">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="bde46-629">Key Vault</span><span class="sxs-lookup"><span data-stu-id="bde46-629">Key Vault</span></span>
* <span data-ttu-id="bde46-630">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="bde46-630">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="bde46-631">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-631">Network</span></span>
* <span data-ttu-id="bde46-632">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="bde46-632">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="bde46-633">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-633">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="bde46-634">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="bde46-634">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="bde46-635">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="bde46-635">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="bde46-636">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-636">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="bde46-637">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-637">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="bde46-638">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="bde46-638">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="bde46-639">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="bde46-639">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="bde46-640">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="bde46-640">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="bde46-641">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="bde46-641">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="bde46-642">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="bde46-642">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="bde46-643">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="bde46-643">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="bde46-644">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="bde46-644">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="bde46-645">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="bde46-645">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="bde46-646">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="bde46-646">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="bde46-647">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="bde46-647">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="bde46-648">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="bde46-648">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="bde46-649">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="bde46-649">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="bde46-650">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bde46-650">RDBMS</span></span>
* <span data-ttu-id="bde46-651">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="bde46-651">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="bde46-652">резервирование.</span><span class="sxs-lookup"><span data-stu-id="bde46-652">Reservation</span></span>
* <span data-ttu-id="bde46-653">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bde46-653">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="bde46-654">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="bde46-654">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="bde46-655">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="bde46-655">Manage App</span></span>
* <span data-ttu-id="bde46-656">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="bde46-656">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="bde46-657">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="bde46-657">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="bde46-658">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-658">Role</span></span>
* <span data-ttu-id="bde46-659">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="bde46-659">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="bde46-660">SignalR</span><span class="sxs-lookup"><span data-stu-id="bde46-660">SignalR</span></span>
* <span data-ttu-id="bde46-661">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bde46-661">First release</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-662">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-662">Storage</span></span>
* <span data-ttu-id="bde46-663">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="bde46-663">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="bde46-664">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="bde46-664">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-665">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-665">VM</span></span>
* <span data-ttu-id="bde46-666">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="bde46-666">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="bde46-667">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="bde46-667">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="bde46-668">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-668">August 28, 2018</span></span>

<span data-ttu-id="bde46-669">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="bde46-669">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="bde46-670">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-670">Core</span></span>

* <span data-ttu-id="bde46-671">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bde46-671">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="bde46-672">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="bde46-672">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-673">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-673">ACR</span></span>

* <span data-ttu-id="bde46-674">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="bde46-674">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="bde46-675">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="bde46-675">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-676">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-676">ACS</span></span>

* <span data-ttu-id="bde46-677">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="bde46-677">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="bde46-678">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="bde46-678">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-679">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-679">AppService</span></span>

* <span data-ttu-id="bde46-680">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="bde46-680">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="bde46-681">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="bde46-681">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="bde46-682">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bde46-682">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="bde46-683">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="bde46-683">Backup</span></span>

* <span data-ttu-id="bde46-684">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bde46-684">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="bde46-685">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="bde46-685">Bot Service</span></span>

* <span data-ttu-id="bde46-686">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="bde46-686">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="bde46-687">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="bde46-687">Cognitive Services</span></span>

* <span data-ttu-id="bde46-688">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="bde46-688">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="bde46-689">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bde46-689">IoT</span></span>

* <span data-ttu-id="bde46-690">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="bde46-690">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-691">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-691">Monitor</span></span>

* <span data-ttu-id="bde46-692">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="bde46-692">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="bde46-693">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="bde46-693">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="bde46-694">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-694">Network</span></span>

* <span data-ttu-id="bde46-695">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bde46-695">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-696">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-696">Resource</span></span>

* <span data-ttu-id="bde46-697">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bde46-697">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-698">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-698">Storage</span></span>

* <span data-ttu-id="bde46-699">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bde46-699">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-700">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-700">VM</span></span>

* <span data-ttu-id="bde46-701">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="bde46-701">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="bde46-702">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-702">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="bde46-703">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-703">Auguest 14, 2018</span></span>

<span data-ttu-id="bde46-704">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="bde46-704">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="bde46-705">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-705">Core</span></span>

* <span data-ttu-id="bde46-706">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="bde46-706">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="bde46-707">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="bde46-707">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="bde46-708">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="bde46-708">Telemetry</span></span>

* <span data-ttu-id="bde46-709">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="bde46-709">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-710">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-710">ACR</span></span>

* <span data-ttu-id="bde46-711">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="bde46-711">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="bde46-712">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="bde46-712">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-713">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-713">ACS</span></span>

* <span data-ttu-id="bde46-714">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="bde46-714">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="bde46-715">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="bde46-715">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="bde46-716">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="bde46-716">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="bde46-717">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="bde46-717">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="bde46-718">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="bde46-718">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="bde46-719">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-719">AppService</span></span>

* <span data-ttu-id="bde46-720">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bde46-720">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="bde46-721">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="bde46-721">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="bde46-722">Batch AI</span><span class="sxs-lookup"><span data-stu-id="bde46-722">BatchAI</span></span>

* <span data-ttu-id="bde46-723">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="bde46-723">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="bde46-724">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-724">Container</span></span>

* <span data-ttu-id="bde46-725">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="bde46-725">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="bde46-726">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bde46-726">IoT</span></span>

* <span data-ttu-id="bde46-727">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="bde46-727">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="bde46-728">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="bde46-728">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="bde46-729">IoT Central</span><span class="sxs-lookup"><span data-stu-id="bde46-729">Iot Central</span></span>

* <span data-ttu-id="bde46-730">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="bde46-730">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="bde46-731">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bde46-731">KeyVault</span></span>


* <span data-ttu-id="bde46-732">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="bde46-732">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="bde46-733">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="bde46-733">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="bde46-734">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="bde46-734">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="bde46-735">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="bde46-735">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="bde46-736">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="bde46-736">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="bde46-737">Передача</span><span class="sxs-lookup"><span data-stu-id="bde46-737">Relay</span></span>

* <span data-ttu-id="bde46-738">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bde46-738">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-739">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-739">Sql</span></span>

* <span data-ttu-id="bde46-740">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="bde46-740">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-741">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-741">Storage</span></span>

* <span data-ttu-id="bde46-742">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="bde46-742">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="bde46-743">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="bde46-743">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="bde46-744">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="bde46-744">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="bde46-745">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="bde46-745">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="bde46-746">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="bde46-746">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-747">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-747">VM</span></span>

* <span data-ttu-id="bde46-748">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="bde46-748">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="bde46-749">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-749">July 31, 2018</span></span>

<span data-ttu-id="bde46-750">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="bde46-750">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-751">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-751">ACR</span></span>

* <span data-ttu-id="bde46-752">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="bde46-752">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="bde46-753">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="bde46-753">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-754">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-754">ACS</span></span>

* <span data-ttu-id="bde46-755">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="bde46-755">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="bde46-756">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-756">Batch</span></span>

* <span data-ttu-id="bde46-757">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="bde46-757">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="bde46-758">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-758">Container</span></span>

* <span data-ttu-id="bde46-759">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="bde46-759">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="bde46-760">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-760">Network</span></span>

* <span data-ttu-id="bde46-761">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="bde46-761">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="bde46-762">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-762">Resource</span></span>

* <span data-ttu-id="bde46-763">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="bde46-763">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="bde46-764">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="bde46-764">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="bde46-765">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-765">Role</span></span>

* <span data-ttu-id="bde46-766">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="bde46-766">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="bde46-767">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="bde46-767">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="bde46-768">поиска</span><span class="sxs-lookup"><span data-stu-id="bde46-768">Search</span></span>

* <span data-ttu-id="bde46-769">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="bde46-769">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="bde46-770">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-770">Service Bus</span></span>

* <span data-ttu-id="bde46-771">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="bde46-771">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="bde46-772">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="bde46-772">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="bde46-773">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="bde46-773">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="bde46-774">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="bde46-774">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-775">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-775">Storage</span></span>

* <span data-ttu-id="bde46-776">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="bde46-776">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="bde46-777">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="bde46-777">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-778">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-778">VM</span></span>

* <span data-ttu-id="bde46-779">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="bde46-779">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="bde46-780">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="bde46-780">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="bde46-781">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="bde46-781">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="bde46-782">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="bde46-782">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="bde46-783">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-783">July 18, 2018</span></span>

<span data-ttu-id="bde46-784">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="bde46-784">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="bde46-785">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-785">Core</span></span>

* <span data-ttu-id="bde46-786">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="bde46-786">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="bde46-787">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="bde46-787">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="bde46-788">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="bde46-788">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-789">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-789">ACR</span></span>

* <span data-ttu-id="bde46-790">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="bde46-790">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="bde46-791">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-791">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="bde46-792">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="bde46-792">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="bde46-793">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="bde46-793">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-794">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-794">ACS</span></span>

* <span data-ttu-id="bde46-795">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="bde46-795">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-796">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-796">AppService</span></span>

* <span data-ttu-id="bde46-797">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="bde46-797">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="bde46-798">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-798">Batch</span></span>

* <span data-ttu-id="bde46-799">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="bde46-799">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="bde46-800">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="bde46-800">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="bde46-801">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bde46-801">Batch AI</span></span>

* <span data-ttu-id="bde46-802">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="bde46-802">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="bde46-803">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-803">Container</span></span>

* <span data-ttu-id="bde46-804">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="bde46-804">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="bde46-805">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="bde46-805">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="bde46-806">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-806">Network</span></span>

* <span data-ttu-id="bde46-807">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-807">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="bde46-808">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-808">Added `network nic wait`</span></span>
* <span data-ttu-id="bde46-809">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="bde46-809">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="bde46-810">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="bde46-810">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="bde46-811">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-811">Resource</span></span>

* <span data-ttu-id="bde46-812">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-812">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="bde46-813">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-813">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="bde46-814">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-814">Added `deployment wait` command</span></span>
* <span data-ttu-id="bde46-815">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="bde46-815">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-816">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-816">SQL</span></span>

* <span data-ttu-id="bde46-817">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-817">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="bde46-818">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="bde46-818">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="bde46-819">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="bde46-819">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-820">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-820">Storage</span></span>

* <span data-ttu-id="bde46-821">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="bde46-821">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-822">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-822">VM</span></span>

* <span data-ttu-id="bde46-823">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-823">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="bde46-824">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-824">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="bde46-825">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-825">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="bde46-826">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-826">July 3, 2018</span></span>

<span data-ttu-id="bde46-827">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="bde46-827">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="bde46-828">AKS</span><span class="sxs-lookup"><span data-stu-id="bde46-828">AKS</span></span>

* <span data-ttu-id="bde46-829">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="bde46-829">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="bde46-830">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-830">July 3, 2018</span></span>

<span data-ttu-id="bde46-831">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="bde46-831">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="bde46-832">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-832">Core</span></span>

* <span data-ttu-id="bde46-833">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="bde46-833">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-834">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-834">ACR</span></span>

* <span data-ttu-id="bde46-835">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="bde46-835">Added polling build status</span></span>
* <span data-ttu-id="bde46-836">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="bde46-836">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="bde46-837">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="bde46-837">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-838">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-838">ACS</span></span>

* <span data-ttu-id="bde46-839">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-839">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="bde46-840">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-840">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="bde46-841">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="bde46-841">Updated options for `aks browse` command.</span></span> <span data-ttu-id="bde46-842">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="bde46-842">Added `--listen-port` support</span></span>
* <span data-ttu-id="bde46-843">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="bde46-843">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="bde46-844">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="bde46-844">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="bde46-845">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="bde46-845">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-846">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-846">AppService</span></span>

* <span data-ttu-id="bde46-847">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="bde46-847">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="bde46-848">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="bde46-848">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="bde46-849">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="bde46-849">Backup</span></span>

* <span data-ttu-id="bde46-850">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="bde46-850">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="bde46-851">Batch AI</span><span class="sxs-lookup"><span data-stu-id="bde46-851">BatchAI</span></span>

* <span data-ttu-id="bde46-852">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="bde46-852">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="bde46-853">Облако</span><span class="sxs-lookup"><span data-stu-id="bde46-853">Cloud</span></span>

* <span data-ttu-id="bde46-854">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="bde46-854">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="bde46-855">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-855">Container</span></span>

* <span data-ttu-id="bde46-856">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="bde46-856">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="bde46-857">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="bde46-857">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="bde46-858">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="bde46-858">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="bde46-859">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bde46-859">Extension</span></span>

* <span data-ttu-id="bde46-860">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="bde46-860">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="bde46-861">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-861">Network</span></span>

* <span data-ttu-id="bde46-862">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="bde46-862">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="bde46-863">Rdbms</span><span class="sxs-lookup"><span data-stu-id="bde46-863">Rdbms</span></span>

* <span data-ttu-id="bde46-864">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="bde46-864">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-865">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-865">Resource</span></span>

* <span data-ttu-id="bde46-866">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="bde46-866">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-867">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-867">VM</span></span>

* <span data-ttu-id="bde46-868">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="bde46-868">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="bde46-869">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-869">June 25, 2018</span></span>

<span data-ttu-id="bde46-870">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="bde46-870">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="bde46-871">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="bde46-871">CLI</span></span>

* <span data-ttu-id="bde46-872">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="bde46-872">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="bde46-873">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-873">June 19, 2018</span></span>

<span data-ttu-id="bde46-874">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="bde46-874">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="bde46-875">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-875">Core</span></span>

* <span data-ttu-id="bde46-876">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="bde46-876">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-877">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-877">ACR</span></span>

* <span data-ttu-id="bde46-878">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="bde46-878">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="bde46-879">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="bde46-879">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-880">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-880">ACS</span></span>

* <span data-ttu-id="bde46-881">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="bde46-881">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="bde46-882">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-882">Added `--update` support</span></span>
* <span data-ttu-id="bde46-883">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="bde46-883">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="bde46-884">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="bde46-884">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="bde46-885">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="bde46-885">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="bde46-886">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="bde46-886">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="bde46-887">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="bde46-887">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="bde46-888">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="bde46-888">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-889">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-889">AppService</span></span>

* <span data-ttu-id="bde46-890">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="bde46-890">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="bde46-891">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bde46-891">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="bde46-892">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-892">Batch</span></span>

* <span data-ttu-id="bde46-893">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="bde46-893">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="bde46-894">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bde46-894">Batch AI</span></span>

* <span data-ttu-id="bde46-895">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="bde46-895">Added support for workspaces.</span></span> <span data-ttu-id="bde46-896">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bde46-896">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="bde46-897">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="bde46-897">Added support for experiments.</span></span> <span data-ttu-id="bde46-898">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="bde46-898">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="bde46-899">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="bde46-899">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="bde46-900">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="bde46-900">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="bde46-901">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="bde46-901">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="bde46-902">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="bde46-902">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="bde46-903">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="bde46-903">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="bde46-904">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="bde46-904">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="bde46-905">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-905">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="bde46-906">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="bde46-906">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="bde46-907">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-907">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="bde46-908">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="bde46-908">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="bde46-909">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="bde46-909">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="bde46-910">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="bde46-910">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="bde46-911">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-911">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="bde46-912">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="bde46-912">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="bde46-913">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="bde46-913">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="bde46-914">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="bde46-914">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="bde46-915">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="bde46-915">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="bde46-916">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="bde46-916">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="bde46-917">Карты</span><span class="sxs-lookup"><span data-stu-id="bde46-917">Maps</span></span>

* <span data-ttu-id="bde46-918">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="bde46-918">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="bde46-919">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-919">Network</span></span>

* <span data-ttu-id="bde46-920">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="bde46-920">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="bde46-921">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="bde46-921">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="bde46-922">#6502</span><span class="sxs-lookup"><span data-stu-id="bde46-922">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="bde46-923">Резервирование</span><span class="sxs-lookup"><span data-stu-id="bde46-923">Reservations</span></span>

* <span data-ttu-id="bde46-924">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-924">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="bde46-925">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-925">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="bde46-926">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="bde46-926">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="bde46-927">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="bde46-927">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="bde46-928">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="bde46-928">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="bde46-929">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-929">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="bde46-930">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-930">Role</span></span>

* <span data-ttu-id="bde46-931">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="bde46-931">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-932">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-932">SQL</span></span>

* <span data-ttu-id="bde46-933">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="bde46-933">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-934">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-934">Storage</span></span>

* <span data-ttu-id="bde46-935">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="bde46-935">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-936">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-936">VM</span></span>

* <span data-ttu-id="bde46-937">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-937">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="bde46-938">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="bde46-938">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="bde46-939">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="bde46-939">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="bde46-940">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-940">June 13, 2018</span></span>

<span data-ttu-id="bde46-941">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="bde46-941">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="bde46-942">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-942">Core</span></span>

* <span data-ttu-id="bde46-943">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="bde46-943">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="bde46-944">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-944">June 13, 2018</span></span>

<span data-ttu-id="bde46-945">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="bde46-945">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="bde46-946">AKS</span><span class="sxs-lookup"><span data-stu-id="bde46-946">AKS</span></span>

* <span data-ttu-id="bde46-947">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="bde46-947">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="bde46-948">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="bde46-948">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="bde46-949">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="bde46-949">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="bde46-950">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="bde46-950">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="bde46-951">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bde46-951">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-952">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-952">AppService</span></span>

* <span data-ttu-id="bde46-953">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="bde46-953">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="bde46-954">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-954">June 5, 2018</span></span>

<span data-ttu-id="bde46-955">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="bde46-955">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-956">Interactive</span><span class="sxs-lookup"><span data-stu-id="bde46-956">Interactive</span></span>

* <span data-ttu-id="bde46-957">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="bde46-957">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="bde46-958">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-958">June 5, 2018</span></span>

<span data-ttu-id="bde46-959">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="bde46-959">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="bde46-960">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-960">Core</span></span>

* <span data-ttu-id="bde46-961">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="bde46-961">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="bde46-962">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="bde46-962">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-963">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-963">ACR</span></span>

* <span data-ttu-id="bde46-964">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="bde46-964">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="bde46-965">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="bde46-965">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="bde46-966">AKS</span><span class="sxs-lookup"><span data-stu-id="bde46-966">AKS</span></span>

* <span data-ttu-id="bde46-967">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="bde46-967">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="bde46-968">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-968">Batch</span></span>

* <span data-ttu-id="bde46-969">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="bde46-969">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="bde46-970">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bde46-970">IOT</span></span>

* <span data-ttu-id="bde46-971">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="bde46-971">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="bde46-972">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-972">Network</span></span>

* <span data-ttu-id="bde46-973">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="bde46-973">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="bde46-974">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="bde46-974">Policy Insights</span></span>

* <span data-ttu-id="bde46-975">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bde46-975">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="bde46-976">ARM</span><span class="sxs-lookup"><span data-stu-id="bde46-976">ARM</span></span>

* <span data-ttu-id="bde46-977">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="bde46-977">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-978">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-978">SQL</span></span>

* <span data-ttu-id="bde46-979">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="bde46-979">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="bde46-980">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="bde46-980">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="bde46-981">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-981">Storage</span></span>

* <span data-ttu-id="bde46-982">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="bde46-982">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-983">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-983">VM</span></span>

* <span data-ttu-id="bde46-984">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="bde46-984">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="bde46-985">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-985">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="bde46-986">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-986">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="bde46-987">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-987">May 22, 2018</span></span>

<span data-ttu-id="bde46-988">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="bde46-988">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="bde46-989">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-989">Core</span></span>

* <span data-ttu-id="bde46-990">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="bde46-990">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-991">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-991">ACS</span></span>

* <span data-ttu-id="bde46-992">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="bde46-992">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="bde46-993">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="bde46-993">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-994">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-994">AppService</span></span>

* <span data-ttu-id="bde46-995">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="bde46-995">Improved generic update commands</span></span>
* <span data-ttu-id="bde46-996">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="bde46-996">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="bde46-997">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-997">Container</span></span>

* <span data-ttu-id="bde46-998">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="bde46-998">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="bde46-999">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-999">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="bde46-1000">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bde46-1000">Extension</span></span>

* <span data-ttu-id="bde46-1001">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="bde46-1001">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-1002">Interactive</span><span class="sxs-lookup"><span data-stu-id="bde46-1002">Interactive</span></span>

* <span data-ttu-id="bde46-1003">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="bde46-1003">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="bde46-1004">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="bde46-1004">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="bde46-1005">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bde46-1005">KeyVault</span></span>

* <span data-ttu-id="bde46-1006">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="bde46-1006">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1007">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1007">Network</span></span>

* <span data-ttu-id="bde46-1008">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="bde46-1008">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="bde46-1009">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="bde46-1009">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-1010">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-1010">SQL</span></span>

* <span data-ttu-id="bde46-1011">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="bde46-1011">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="bde46-1012">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1012">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="bde46-1013">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1013">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="bde46-1014">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="bde46-1014">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="bde46-1015">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="bde46-1015">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="bde46-1016">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1016">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="bde46-1017">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1017">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="bde46-1018">`edition`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1018">`edition`.</span></span> <span data-ttu-id="bde46-1019">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1019">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="bde46-1020">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1020">`elasticPoolName`.</span></span> <span data-ttu-id="bde46-1021">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1021">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="bde46-1022">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="bde46-1022">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="bde46-1023">`edition`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1023">`edition`.</span></span> <span data-ttu-id="bde46-1024">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1024">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="bde46-1025">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1025">`dtu`.</span></span> <span data-ttu-id="bde46-1026">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1026">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="bde46-1027">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1027">`databaseDtuMin`.</span></span> <span data-ttu-id="bde46-1028">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1028">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="bde46-1029">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1029">`databaseDtuMax`.</span></span> <span data-ttu-id="bde46-1030">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1030">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="bde46-1031">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1031">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="bde46-1032">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1032">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1033">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1033">Storage</span></span>

* <span data-ttu-id="bde46-1034">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1034">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="bde46-1035">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1035">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1036">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1036">VM</span></span>

* <span data-ttu-id="bde46-1037">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1037">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="bde46-1038">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1038">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="bde46-1039">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1039">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="bde46-1040">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="bde46-1040">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="bde46-1041">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1041">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="bde46-1042">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1042">May 7, 2018</span></span>

<span data-ttu-id="bde46-1043">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="bde46-1043">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="bde46-1044">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-1044">Core</span></span>

* <span data-ttu-id="bde46-1045">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="bde46-1045">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="bde46-1046">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1046">Added limited support for positional arguments</span></span>
* <span data-ttu-id="bde46-1047">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1047">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="bde46-1048">#5591</span><span class="sxs-lookup"><span data-stu-id="bde46-1048">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="bde46-1049">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1049">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="bde46-1050">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="bde46-1050">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="bde46-1051">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="bde46-1051">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="bde46-1052">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1052">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="bde46-1053">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="bde46-1053">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-1054">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-1054">ACR</span></span>

* <span data-ttu-id="bde46-1055">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="bde46-1055">Added ACR Build commands</span></span>
* <span data-ttu-id="bde46-1056">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="bde46-1056">Improved resource not found error messages</span></span>
* <span data-ttu-id="bde46-1057">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="bde46-1057">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="bde46-1058">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="bde46-1058">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="bde46-1059">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="bde46-1059">Improved repository commands error messages</span></span>
* <span data-ttu-id="bde46-1060">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="bde46-1060">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1061">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1061">ACS</span></span>

* <span data-ttu-id="bde46-1062">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-1062">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="bde46-1063">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="bde46-1063">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="bde46-1064">AMS</span><span class="sxs-lookup"><span data-stu-id="bde46-1064">AMS</span></span>

* <span data-ttu-id="bde46-1065">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="bde46-1065">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1066">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1066">Appservice</span></span>

* <span data-ttu-id="bde46-1067">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="bde46-1067">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="bde46-1068">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1068">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="bde46-1069">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="bde46-1069">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="bde46-1070">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1070">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="bde46-1071">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bde46-1071">Batch AI</span></span>

* <span data-ttu-id="bde46-1072">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="bde46-1072">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="bde46-1073">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="bde46-1073">Cognitive Services</span></span>

* <span data-ttu-id="bde46-1074">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="bde46-1074">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="bde46-1075">Потребление</span><span class="sxs-lookup"><span data-stu-id="bde46-1075">Consumption</span></span>

* <span data-ttu-id="bde46-1076">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="bde46-1076">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="bde46-1077">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-1077">Container</span></span>

* <span data-ttu-id="bde46-1078">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="bde46-1078">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="bde46-1079">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="bde46-1079">Cosmos DB</span></span>

* <span data-ttu-id="bde46-1080">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bde46-1080">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="bde46-1081">DMS</span><span class="sxs-lookup"><span data-stu-id="bde46-1081">DMS</span></span>

* <span data-ttu-id="bde46-1082">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="bde46-1082">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="bde46-1083">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bde46-1083">Extension</span></span>

* <span data-ttu-id="bde46-1084">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="bde46-1084">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-1085">Interactive</span><span class="sxs-lookup"><span data-stu-id="bde46-1085">Interactive</span></span>

* <span data-ttu-id="bde46-1086">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="bde46-1086">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="bde46-1087">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="bde46-1087">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="bde46-1088">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="bde46-1088">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="bde46-1089">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="bde46-1089">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="bde46-1090">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="bde46-1090">Lab</span></span>

* <span data-ttu-id="bde46-1091">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="bde46-1091">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1092">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1092">Network</span></span>

* <span data-ttu-id="bde46-1093">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="bde46-1093">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="bde46-1094">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-1094">Profile</span></span>

* <span data-ttu-id="bde46-1095">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1095">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="bde46-1096">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="bde46-1096">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="bde46-1097">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1097">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="bde46-1098">Redis</span><span class="sxs-lookup"><span data-stu-id="bde46-1098">Redis</span></span>

* <span data-ttu-id="bde46-1099">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1099">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="bde46-1100">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="bde46-1100">Deprecated `redis list-all`.</span></span> <span data-ttu-id="bde46-1101">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1101">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="bde46-1102">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1102">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="bde46-1103">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="bde46-1103">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="bde46-1104">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-1104">Role</span></span>

* <span data-ttu-id="bde46-1105">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="bde46-1105">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1106">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1106">Storage</span></span>

* <span data-ttu-id="bde46-1107">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="bde46-1107">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="bde46-1108">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="bde46-1108">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="bde46-1109">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="bde46-1109">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="bde46-1110">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="bde46-1110">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="bde46-1111">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="bde46-1111">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1112">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1112">VM</span></span>

* <span data-ttu-id="bde46-1113">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="bde46-1113">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="bde46-1114">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="bde46-1114">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="bde46-1115">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="bde46-1115">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="bde46-1116">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1116">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="bde46-1117">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="bde46-1117">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="bde46-1118">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="bde46-1118">Added write accelerator support</span></span>
* <span data-ttu-id="bde46-1119">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1119">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="bde46-1120">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="bde46-1120">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="bde46-1121">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="bde46-1121">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="bde46-1122">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1122">April 10, 2018</span></span>

<span data-ttu-id="bde46-1123">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="bde46-1123">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-1124">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-1124">ACR</span></span>

* <span data-ttu-id="bde46-1125">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="bde46-1125">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1126">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1126">ACS</span></span>

* <span data-ttu-id="bde46-1127">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="bde46-1127">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1128">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1128">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="bde46-1130">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="bde46-1130">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="bde46-1131">Batch AI</span><span class="sxs-lookup"><span data-stu-id="bde46-1131">BatchAI</span></span>

* <span data-ttu-id="bde46-1132">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="bde46-1132">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="bde46-1133">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="bde46-1133">Job level mounting</span></span>
  - <span data-ttu-id="bde46-1134">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1134">Environment variables with secret values</span></span>
  - <span data-ttu-id="bde46-1135">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="bde46-1135">Performance counters settings</span></span>
  - <span data-ttu-id="bde46-1136">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="bde46-1136">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="bde46-1137">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1137">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="bde46-1138">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="bde46-1138">Usage and limits reporting</span></span>
  - <span data-ttu-id="bde46-1139">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1139">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="bde46-1140">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1140">Support for custom images</span></span>
  - <span data-ttu-id="bde46-1141">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="bde46-1141">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="bde46-1142">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="bde46-1142">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="bde46-1143">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1143">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="bde46-1144">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="bde46-1144">National clouds are supported</span></span>
* <span data-ttu-id="bde46-1145">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bde46-1145">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="bde46-1146">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="bde46-1146">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="bde46-1147">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="bde46-1147">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="bde46-1148">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bde46-1148">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="bde46-1149">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="bde46-1149">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="bde46-1150">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="bde46-1150">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="bde46-1151">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1151">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="bde46-1152">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="bde46-1152">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="bde46-1153">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="bde46-1153">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="bde46-1154">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1154">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="bde46-1155">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="bde46-1155">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="bde46-1156">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1156">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="bde46-1157">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1157">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="bde46-1158">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="bde46-1158">Billing</span></span>

* <span data-ttu-id="bde46-1159">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="bde46-1159">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="bde46-1160">Потребление</span><span class="sxs-lookup"><span data-stu-id="bde46-1160">Consumption</span></span>

* <span data-ttu-id="bde46-1161">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1161">Added `marketplace` commands</span></span>
* <span data-ttu-id="bde46-1162">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1162">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="bde46-1163">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1163">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="bde46-1164">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1164">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="bde46-1165">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1165">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="bde46-1166">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1166">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="bde46-1167">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-1167">Container</span></span>

* <span data-ttu-id="bde46-1168">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1168">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="bde46-1169">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="bde46-1169">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="bde46-1170">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bde46-1170">Extension</span></span>

* <span data-ttu-id="bde46-1171">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="bde46-1171">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-1172">Interactive</span><span class="sxs-lookup"><span data-stu-id="bde46-1172">Interactive</span></span>

* <span data-ttu-id="bde46-1173">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="bde46-1173">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="bde46-1174">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="bde46-1174">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="bde46-1175">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1175">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1176">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1176">Network</span></span>

* <span data-ttu-id="bde46-1177">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1177">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="bde46-1178">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1178">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="bde46-1179">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="bde46-1179">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="bde46-1180">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="bde46-1180">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="bde46-1181">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="bde46-1181">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="bde46-1182">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1182">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="bde46-1183">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1183">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="bde46-1184">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="bde46-1184">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="bde46-1185">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-1185">Profile</span></span>

* <span data-ttu-id="bde46-1186">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1186">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="bde46-1187">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1187">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="bde46-1188">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bde46-1188">RDBMS</span></span>

* <span data-ttu-id="bde46-1189">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1189">Added `georestore` command</span></span>
* <span data-ttu-id="bde46-1190">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="bde46-1190">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1191">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1191">Resource</span></span>

* <span data-ttu-id="bde46-1192">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1192">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="bde46-1193">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1193">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-1194">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-1194">SQL</span></span>

* <span data-ttu-id="bde46-1195">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1195">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1196">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1196">Storage</span></span>

* <span data-ttu-id="bde46-1197">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="bde46-1197">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1198">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1198">VM</span></span>

* <span data-ttu-id="bde46-1199">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="bde46-1199">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="bde46-1200">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="bde46-1200">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="bde46-1202">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1202">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="bde46-1203">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="bde46-1203">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="bde46-1204">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="bde46-1204">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="bde46-1205">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="bde46-1205">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="bde46-1206">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1206">March 27, 2018</span></span>

<span data-ttu-id="bde46-1207">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="bde46-1207">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="bde46-1208">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-1208">Core</span></span>

* <span data-ttu-id="bde46-1209">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="bde46-1209">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1210">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1210">ACS</span></span>

* <span data-ttu-id="bde46-1211">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="bde46-1211">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1212">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1212">Appservice</span></span>

* <span data-ttu-id="bde46-1213">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1213">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="bde46-1214">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1214">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="bde46-1215">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="bde46-1215">Backup</span></span>

* <span data-ttu-id="bde46-1216">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1216">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="bde46-1217">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="bde46-1217">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="bde46-1218">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="bde46-1218">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="bde46-1219">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1219">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="bde46-1220">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-1220">Container</span></span>

* <span data-ttu-id="bde46-1221">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1221">Added `container exec` command.</span></span> <span data-ttu-id="bde46-1222">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1222">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="bde46-1223">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1223">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="bde46-1224">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bde46-1224">Extension</span></span>

* <span data-ttu-id="bde46-1225">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="bde46-1225">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="bde46-1226">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1226">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="bde46-1227">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-1227">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-1228">Interactive</span><span class="sxs-lookup"><span data-stu-id="bde46-1228">Interactive</span></span>

* <span data-ttu-id="bde46-1229">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="bde46-1229">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="bde46-1230">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1230">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="bde46-1231">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="bde46-1231">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="bde46-1232">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="bde46-1232">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="bde46-1233">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="bde46-1233">Lab</span></span>

* <span data-ttu-id="bde46-1234">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1234">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-1235">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-1235">Monitor</span></span>

* <span data-ttu-id="bde46-1236">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="bde46-1236">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="bde46-1237">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="bde46-1237">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="bde46-1238">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="bde46-1238">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1239">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1239">Network</span></span>

* <span data-ttu-id="bde46-1240">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="bde46-1240">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="bde46-1241">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-1241">Profile</span></span>

* <span data-ttu-id="bde46-1242">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1242">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="bde46-1243">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bde46-1243">RDBMS</span></span>

* <span data-ttu-id="bde46-1244">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="bde46-1244">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1245">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1245">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="bde46-1247">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-1247">Role</span></span>

* <span data-ttu-id="bde46-1248">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1248">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="bde46-1249">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="bde46-1249">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="bde46-1250">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="bde46-1250">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="bde46-1251">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1251">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="bde46-1252">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1252">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1253">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1253">Storage</span></span>

* <span data-ttu-id="bde46-1254">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="bde46-1254">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="bde46-1255">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="bde46-1255">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1256">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1256">VM</span></span>

* <span data-ttu-id="bde46-1257">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1257">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="bde46-1258">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1258">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="bde46-1259">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="bde46-1259">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="bde46-1260">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="bde46-1260">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="bde46-1261">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1261">March 13, 2018</span></span>

<span data-ttu-id="bde46-1262">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="bde46-1262">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-1263">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-1263">ACR</span></span>

* <span data-ttu-id="bde46-1264">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1264">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="bde46-1265">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="bde46-1265">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="bde46-1266">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="bde46-1266">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1267">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1267">ACS</span></span>

* <span data-ttu-id="bde46-1268">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="bde46-1268">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="bde46-1269">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="bde46-1269">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="bde46-1270">Помощник</span><span class="sxs-lookup"><span data-stu-id="bde46-1270">Advisor</span></span>

* <span data-ttu-id="bde46-1271">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1271">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="bde46-1272">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1272">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="bde46-1273">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1273">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="bde46-1274">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1274">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="bde46-1275">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1275">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1276">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1276">Appservice</span></span>

* <span data-ttu-id="bde46-1277">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="bde46-1277">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="bde46-1278">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1278">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="bde46-1279">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="bde46-1279">Eventhubs</span></span>

* <span data-ttu-id="bde46-1280">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bde46-1280">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="bde46-1281">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bde46-1281">Extension</span></span>

* <span data-ttu-id="bde46-1282">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="bde46-1282">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-1283">Interactive</span><span class="sxs-lookup"><span data-stu-id="bde46-1283">Interactive</span></span>

* <span data-ttu-id="bde46-1284">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="bde46-1284">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="bde46-1285">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="bde46-1285">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="bde46-1286">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="bde46-1286">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="bde46-1287">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="bde46-1287">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-1288">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-1288">Monitor</span></span>

* <span data-ttu-id="bde46-1289">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="bde46-1289">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="bde46-1290">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1290">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="bde46-1291">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1291">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="bde46-1292">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1292">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1293">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1293">Network</span></span>

* <span data-ttu-id="bde46-1294">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1294">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="bde46-1295">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="bde46-1295">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="bde46-1296">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1296">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="bde46-1297">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1297">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="bde46-1298">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-1298">Profile</span></span>

* <span data-ttu-id="bde46-1299">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="bde46-1299">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="bde46-1300">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1300">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="bde46-1301">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bde46-1301">RDBMS</span></span>

* <span data-ttu-id="bde46-1302">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="bde46-1302">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="bde46-1303">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-1303">Service Bus</span></span>

* <span data-ttu-id="bde46-1304">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bde46-1304">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1305">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1305">Storage</span></span>

* <span data-ttu-id="bde46-1306">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="bde46-1306">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="bde46-1307">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="bde46-1307">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1308">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1308">VM</span></span>

* <span data-ttu-id="bde46-1309">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="bde46-1309">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="bde46-1310">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="bde46-1310">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="bde46-1311">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1311">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="bde46-1312">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="bde46-1312">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="bde46-1313">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="bde46-1313">February 27, 2018</span></span>

<span data-ttu-id="bde46-1314">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="bde46-1314">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="bde46-1315">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-1315">Core</span></span>

* <span data-ttu-id="bde46-1316">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="bde46-1316">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="bde46-1317">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="bde46-1317">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="bde46-1318">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1318">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1319">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1319">ACS</span></span>

* <span data-ttu-id="bde46-1320">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-1320">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="bde46-1321">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="bde46-1321">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="bde46-1322">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1322">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="bde46-1323">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1323">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1324">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1324">Appservice</span></span>

* <span data-ttu-id="bde46-1325">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="bde46-1325">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="bde46-1326">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="bde46-1326">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="bde46-1327">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="bde46-1327">Cognitive Services</span></span>

* <span data-ttu-id="bde46-1328">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="bde46-1328">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="bde46-1329">Потребление</span><span class="sxs-lookup"><span data-stu-id="bde46-1329">Consumption</span></span>

* <span data-ttu-id="bde46-1330">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="bde46-1330">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="bde46-1331">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="bde46-1331">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="bde46-1332">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-1332">Container</span></span>

* <span data-ttu-id="bde46-1333">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="bde46-1333">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1334">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1334">Network</span></span>

* <span data-ttu-id="bde46-1335">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1335">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1336">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1336">Resource</span></span>

* <span data-ttu-id="bde46-1337">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="bde46-1337">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="bde46-1338">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-1338">Role</span></span>

* <span data-ttu-id="bde46-1339">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-1339">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-1340">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-1340">SQL</span></span>

* <span data-ttu-id="bde46-1341">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1341">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1342">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1342">Storage</span></span>

* <span data-ttu-id="bde46-1343">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1343">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1344">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1344">VM</span></span>

* <span data-ttu-id="bde46-1345">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="bde46-1345">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="bde46-1346">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1346">February 13, 2018</span></span>

<span data-ttu-id="bde46-1347">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="bde46-1347">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="bde46-1348">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-1348">Core</span></span>

* <span data-ttu-id="bde46-1349">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="bde46-1349">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1350">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1350">ACS</span></span>

* <span data-ttu-id="bde46-1351">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="bde46-1351">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="bde46-1352">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1352">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="bde46-1353">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="bde46-1353">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="bde46-1354">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="bde46-1354">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="bde46-1355">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="bde46-1355">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="bde46-1356">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1356">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="bde46-1357">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="bde46-1357">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="bde46-1358">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1358">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1359">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1359">Appservice</span></span>

* <span data-ttu-id="bde46-1360">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="bde46-1360">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="bde46-1361">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1361">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="bde46-1362">CDN</span><span class="sxs-lookup"><span data-stu-id="bde46-1362">CDN</span></span>

* <span data-ttu-id="bde46-1363">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1363">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="bde46-1364">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-1364">Container</span></span>

* <span data-ttu-id="bde46-1365">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="bde46-1365">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="bde46-1366">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1366">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bde46-1367">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bde46-1367">CosmosDB</span></span>

* <span data-ttu-id="bde46-1368">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1368">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="bde46-1369">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bde46-1369">Extension</span></span>

* <span data-ttu-id="bde46-1370">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1370">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="bde46-1371">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1371">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="bde46-1372">Отзыв</span><span class="sxs-lookup"><span data-stu-id="bde46-1372">Feedback</span></span>

* <span data-ttu-id="bde46-1373">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="bde46-1373">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-1374">Interactive</span><span class="sxs-lookup"><span data-stu-id="bde46-1374">Interactive</span></span>

* <span data-ttu-id="bde46-1375">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="bde46-1375">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="bde46-1376">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1376">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="bde46-1377">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bde46-1377">IoT</span></span>

* <span data-ttu-id="bde46-1378">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="bde46-1378">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="bde46-1379">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="bde46-1379">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="bde46-1380">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1380">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="bde46-1381">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="bde46-1381">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-1382">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-1382">Monitor</span></span>

* <span data-ttu-id="bde46-1383">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1383">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1384">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1384">Network</span></span>

* <span data-ttu-id="bde46-1385">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="bde46-1385">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="bde46-1386">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-1386">Profile</span></span>

* <span data-ttu-id="bde46-1387">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="bde46-1387">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1388">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1388">Resource</span></span>

* <span data-ttu-id="bde46-1389">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1389">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="bde46-1390">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-1390">Role</span></span>

* <span data-ttu-id="bde46-1391">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="bde46-1391">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-1392">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-1392">SQL</span></span>

* <span data-ttu-id="bde46-1393">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1393">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="bde46-1394">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1394">Added `sql db rename`</span></span>
* <span data-ttu-id="bde46-1395">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="bde46-1395">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1396">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1396">Storage</span></span>

* <span data-ttu-id="bde46-1397">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="bde46-1397">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1398">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1398">VM</span></span>

* <span data-ttu-id="bde46-1399">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="bde46-1399">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="bde46-1400">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="bde46-1400">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="bde46-1401">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="bde46-1401">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="bde46-1402">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1402">January 31, 2018</span></span>

<span data-ttu-id="bde46-1403">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="bde46-1403">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="bde46-1404">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-1404">Core</span></span>

* <span data-ttu-id="bde46-1405">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="bde46-1405">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="bde46-1406">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="bde46-1406">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="bde46-1407">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="bde46-1407">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="bde46-1408">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="bde46-1408">Use `--verbose` to see</span></span>
* <span data-ttu-id="bde46-1409">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="bde46-1409">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1410">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1410">ACS</span></span>

* <span data-ttu-id="bde46-1411">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1411">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="bde46-1412">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1412">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1413">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1413">Appservice</span></span>

* <span data-ttu-id="bde46-1414">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="bde46-1414">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="bde46-1415">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="bde46-1415">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="bde46-1416">CDN</span><span class="sxs-lookup"><span data-stu-id="bde46-1416">CDN</span></span>

* <span data-ttu-id="bde46-1417">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1417">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bde46-1418">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bde46-1418">CosmosDB</span></span>

* <span data-ttu-id="bde46-1419">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="bde46-1419">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-1420">Interactive</span><span class="sxs-lookup"><span data-stu-id="bde46-1420">Interactive</span></span>

* <span data-ttu-id="bde46-1421">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="bde46-1421">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1422">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1422">Network</span></span>

* <span data-ttu-id="bde46-1423">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1423">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="bde46-1424">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-1424">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="bde46-1425">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1425">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="bde46-1426">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1426">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="bde46-1427">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1427">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="bde46-1428">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="bde46-1428">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="bde46-1429">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="bde46-1429">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="bde46-1430">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="bde46-1430">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="bde46-1431">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1431">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="bde46-1432">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1432">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="bde46-1433">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-1433">Profile</span></span>

* <span data-ttu-id="bde46-1434">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="bde46-1434">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1435">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1435">Resource</span></span>

* <span data-ttu-id="bde46-1436">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="bde46-1436">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1437">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1437">Storage</span></span>

* <span data-ttu-id="bde46-1438">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="bde46-1438">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="bde46-1439">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="bde46-1439">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="bde46-1440">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1440">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="bde46-1441">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1441">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="bde46-1442">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="bde46-1442">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1443">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1443">VM</span></span>

* <span data-ttu-id="bde46-1444">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="bde46-1444">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="bde46-1445">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1445">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="bde46-1446">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="bde46-1446">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="bde46-1447">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1447">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="bde46-1448">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1448">January 17, 2018</span></span>

<span data-ttu-id="bde46-1449">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="bde46-1449">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-1450">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-1450">ACR</span></span>

* <span data-ttu-id="bde46-1451">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="bde46-1451">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="bde46-1452">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="bde46-1452">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1453">ACS</span></span>

* <span data-ttu-id="bde46-1454">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1454">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="bde46-1455">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-1455">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1456">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1456">Appservice</span></span>

* <span data-ttu-id="bde46-1457">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="bde46-1457">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="bde46-1458">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1458">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="bde46-1459">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1459">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="bde46-1460">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="bde46-1460">Backup</span></span>

* <span data-ttu-id="bde46-1461">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="bde46-1461">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="bde46-1462">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="bde46-1462">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="bde46-1463">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="bde46-1463">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="bde46-1464">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="bde46-1464">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="bde46-1465">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="bde46-1465">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="bde46-1466">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-1466">Batch</span></span>

* <span data-ttu-id="bde46-1467">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="bde46-1467">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="bde46-1468">Облако</span><span class="sxs-lookup"><span data-stu-id="bde46-1468">Cloud</span></span>

* <span data-ttu-id="bde46-1469">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="bde46-1469">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="bde46-1470">Потребление</span><span class="sxs-lookup"><span data-stu-id="bde46-1470">Consumption</span></span>

* <span data-ttu-id="bde46-1471">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1471">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="bde46-1472">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-1472">Event Grid</span></span>

* <span data-ttu-id="bde46-1473">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1473">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="bde46-1474">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1474">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="bde46-1475">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1475">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="bde46-1476">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1476">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="bde46-1477">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1477">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="bde46-1478">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1478">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="bde46-1479">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1479">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="bde46-1480">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1480">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-1481">Interactive</span><span class="sxs-lookup"><span data-stu-id="bde46-1481">Interactive</span></span>

* <span data-ttu-id="bde46-1482">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="bde46-1482">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="bde46-1483">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="bde46-1483">Fixed errors on startup</span></span>
* <span data-ttu-id="bde46-1484">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="bde46-1484">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="bde46-1485">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bde46-1485">IoT</span></span>

* <span data-ttu-id="bde46-1486">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="bde46-1486">Added support for device provisioning service</span></span>
* <span data-ttu-id="bde46-1487">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="bde46-1487">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="bde46-1488">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="bde46-1488">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-1489">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-1489">Monitor</span></span>

* <span data-ttu-id="bde46-1490">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="bde46-1490">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="bde46-1491">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1491">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="bde46-1492">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="bde46-1492">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1493">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1493">Network</span></span>

* <span data-ttu-id="bde46-1494">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="bde46-1494">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="bde46-1495">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="bde46-1495">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="bde46-1496">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-1496">Profile</span></span>

* <span data-ttu-id="bde46-1497">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="bde46-1497">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="bde46-1498">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-1498">Role</span></span>

* <span data-ttu-id="bde46-1499">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1499">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="bde46-1500">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bde46-1500">Service Fabric</span></span>

* <span data-ttu-id="bde46-1501">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="bde46-1501">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="bde46-1502">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="bde46-1502">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1503">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1503">VM</span></span>

* <span data-ttu-id="bde46-1504">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1504">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="bde46-1505">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="bde46-1505">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="bde46-1506">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1506">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="bde46-1507">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="bde46-1507">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="bde46-1508">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="bde46-1508">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="bde46-1509">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1509">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="bde46-1510">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1510">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="bde46-1511">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1511">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="bde46-1512">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1512">December 19, 2017</span></span>

<span data-ttu-id="bde46-1513">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="bde46-1513">Version 2.0.23</span></span>

* <span data-ttu-id="bde46-1514">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="bde46-1514">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="bde46-1515">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-1515">Container</span></span>

* <span data-ttu-id="bde46-1516">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1516">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1517">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1517">Network</span></span>

* <span data-ttu-id="bde46-1518">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bde46-1518">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="bde46-1519">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bde46-1519">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1520">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1520">Storage</span></span>

* <span data-ttu-id="bde46-1521">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="bde46-1521">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1522">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1522">VM</span></span>

* <span data-ttu-id="bde46-1523">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="bde46-1523">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="bde46-1524">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1524">December 5, 2017</span></span>

<span data-ttu-id="bde46-1525">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="bde46-1525">Version 2.0.22</span></span>

* <span data-ttu-id="bde46-1526">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1526">Removed `az component` commands.</span></span> <span data-ttu-id="bde46-1527">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1527">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="bde46-1528">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-1528">Core</span></span>
* <span data-ttu-id="bde46-1529">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="bde46-1529">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="bde46-1530">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="bde46-1530">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1531">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1531">ACS</span></span>

* <span data-ttu-id="bde46-1532">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1532">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="bde46-1533">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1533">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="bde46-1534">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="bde46-1534">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="bde46-1535">Помощник</span><span class="sxs-lookup"><span data-stu-id="bde46-1535">Advisor</span></span>

* <span data-ttu-id="bde46-1536">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bde46-1536">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1537">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1537">Appservice</span></span>

* <span data-ttu-id="bde46-1538">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1538">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="bde46-1539">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="bde46-1539">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="bde46-1540">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1540">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="bde46-1541">Потребление</span><span class="sxs-lookup"><span data-stu-id="bde46-1541">Consumption</span></span>

* <span data-ttu-id="bde46-1542">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="bde46-1542">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="bde46-1543">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-1543">Container</span></span>

* <span data-ttu-id="bde46-1544">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="bde46-1544">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-1545">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-1545">Monitor</span></span>

* <span data-ttu-id="bde46-1546">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="bde46-1546">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1547">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1547">Resource</span></span>

* <span data-ttu-id="bde46-1548">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="bde46-1548">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="bde46-1549">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-1549">Role</span></span>

* <span data-ttu-id="bde46-1550">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1550">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="bde46-1551">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="bde46-1551">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="bde46-1552">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1552">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-1553">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-1553">SQL</span></span>

* <span data-ttu-id="bde46-1554">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1554">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="bde46-1555">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1555">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1556">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1556">VM</span></span>

* <span data-ttu-id="bde46-1557">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1557">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="bde46-1558">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1558">November 14, 2017</span></span>

<span data-ttu-id="bde46-1559">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="bde46-1559">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-1560">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-1560">ACR</span></span>

* <span data-ttu-id="bde46-1561">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="bde46-1561">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="bde46-1562">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1562">ACS</span></span>

* <span data-ttu-id="bde46-1563">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="bde46-1563">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="bde46-1564">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="bde46-1564">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="bde46-1565">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1565">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="bde46-1566">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="bde46-1566">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="bde46-1567">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="bde46-1567">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1568">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1568">Appservice</span></span>

* <span data-ttu-id="bde46-1569">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="bde46-1569">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="bde46-1570">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1570">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="bde46-1571">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1571">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="bde46-1572">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1572">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="bde46-1573">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="bde46-1573">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="bde46-1574">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="bde46-1574">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="bde46-1575">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-1575">Batch</span></span>

* <span data-ttu-id="bde46-1576">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1576">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="bde46-1577">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bde46-1577">Batchai</span></span>

* <span data-ttu-id="bde46-1578">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1578">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="bde46-1579">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1579">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="bde46-1580">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1580">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="bde46-1581">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1581">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="bde46-1582">Облако</span><span class="sxs-lookup"><span data-stu-id="bde46-1582">Cloud</span></span>

* <span data-ttu-id="bde46-1583">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="bde46-1583">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="bde46-1584">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-1584">Container</span></span>

* <span data-ttu-id="bde46-1585">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1585">Added support to open multiple ports</span></span>
* <span data-ttu-id="bde46-1586">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1586">Added container group restart policy</span></span>
* <span data-ttu-id="bde46-1587">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="bde46-1587">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="bde46-1588">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="bde46-1588">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bde46-1589">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bde46-1589">Data Lake Analytics</span></span>

* <span data-ttu-id="bde46-1590">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="bde46-1590">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bde46-1591">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bde46-1591">Data Lake Store</span></span>

* <span data-ttu-id="bde46-1592">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="bde46-1592">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="bde46-1593">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bde46-1593">Extension</span></span>

* <span data-ttu-id="bde46-1594">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="bde46-1594">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="bde46-1595">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="bde46-1595">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="bde46-1596">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bde46-1596">IoT</span></span>

* <span data-ttu-id="bde46-1597">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1597">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-1598">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-1598">Monitor</span></span>

* <span data-ttu-id="bde46-1599">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1599">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1600">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1600">Network</span></span>

* <span data-ttu-id="bde46-1601">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="bde46-1601">Added support for CAA DNS records</span></span>
* <span data-ttu-id="bde46-1602">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1602">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="bde46-1603">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="bde46-1603">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="bde46-1604">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1604">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="bde46-1605">Резервирование</span><span class="sxs-lookup"><span data-stu-id="bde46-1605">Reservations</span></span>

* <span data-ttu-id="bde46-1606">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="bde46-1606">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1607">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1607">Resource</span></span>

* <span data-ttu-id="bde46-1608">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1608">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-1609">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-1609">SQL</span></span>

* <span data-ttu-id="bde46-1610">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1610">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1611">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1611">Storage</span></span>

* <span data-ttu-id="bde46-1612">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-1612">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="bde46-1613">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="bde46-1613">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="bde46-1614">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1614">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="bde46-1615">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1615">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="bde46-1616">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1616">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="bde46-1617">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1617">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="bde46-1618">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1618">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1619">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1619">VM</span></span>

* <span data-ttu-id="bde46-1620">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1620">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="bde46-1621">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1621">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="bde46-1622">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1622">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="bde46-1623">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1623">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="bde46-1624">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="bde46-1624">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="bde46-1625">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1625">October 24, 2017</span></span>

<span data-ttu-id="bde46-1626">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="bde46-1626">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="bde46-1627">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-1627">Core</span></span>

* <span data-ttu-id="bde46-1628">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="bde46-1628">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-1629">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-1629">ACR</span></span>

* <span data-ttu-id="bde46-1630">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="bde46-1630">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="bde46-1631">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="bde46-1631">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="bde46-1632">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="bde46-1632">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1633">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1633">ACS</span></span>

* <span data-ttu-id="bde46-1634">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="bde46-1634">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="bde46-1635">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="bde46-1635">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1636">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1636">Appservice</span></span>

* <span data-ttu-id="bde46-1637">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="bde46-1637">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="bde46-1638">Компонент</span><span class="sxs-lookup"><span data-stu-id="bde46-1638">Component</span></span>

* <span data-ttu-id="bde46-1639">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="bde46-1639">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-1640">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-1640">Monitor</span></span>

* <span data-ttu-id="bde46-1641">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1641">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1642">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1642">Resource</span></span>

* <span data-ttu-id="bde46-1643">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="bde46-1643">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="bde46-1644">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="bde46-1644">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1645">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1645">VM</span></span>

* <span data-ttu-id="bde46-1646">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="bde46-1646">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="bde46-1647">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1647">October 9, 2017</span></span>

<span data-ttu-id="bde46-1648">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="bde46-1648">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="bde46-1649">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-1649">Core</span></span>

* <span data-ttu-id="bde46-1650">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="bde46-1650">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1651">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1651">Appservice</span></span>

* <span data-ttu-id="bde46-1652">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1652">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="bde46-1653">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-1653">Batch</span></span>

* <span data-ttu-id="bde46-1654">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="bde46-1654">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="bde46-1655">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="bde46-1655">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="bde46-1656">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-1656">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="bde46-1657">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1657">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="bde46-1658">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bde46-1658">Batchai</span></span>

* <span data-ttu-id="bde46-1659">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="bde46-1659">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="bde46-1660">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bde46-1660">Keyvault</span></span>

* <span data-ttu-id="bde46-1661">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="bde46-1661">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="bde46-1662">(#4448)</span><span class="sxs-lookup"><span data-stu-id="bde46-1662">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="bde46-1663">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1663">Network</span></span>

* <span data-ttu-id="bde46-1664">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="bde46-1664">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="bde46-1665">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="bde46-1665">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1666">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1666">Resource</span></span>

* <span data-ttu-id="bde46-1667">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1667">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="bde46-1668">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="bde46-1668">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="bde46-1669">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="bde46-1669">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="bde46-1670">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="bde46-1670">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-1671">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-1671">Sql</span></span>

* <span data-ttu-id="bde46-1672">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="bde46-1672">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="bde46-1673">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="bde46-1673">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="bde46-1674">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="bde46-1674">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1675">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1675">Storage</span></span>

* <span data-ttu-id="bde46-1676">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1676">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1677">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="bde46-1677">Vm</span></span>

* <span data-ttu-id="bde46-1678">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1678">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="bde46-1679">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1679">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="bde46-1680">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1680">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="bde46-1681">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1681">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="bde46-1682">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="bde46-1682">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="bde46-1683">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1683">September 22, 2017</span></span>

<span data-ttu-id="bde46-1684">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="bde46-1684">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1685">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1685">Resource</span></span>

* <span data-ttu-id="bde46-1686">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="bde46-1686">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="bde46-1687">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="bde46-1687">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="bde46-1688">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="bde46-1688">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="bde46-1689">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1689">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1690">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1690">Network</span></span>

* <span data-ttu-id="bde46-1691">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="bde46-1691">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="bde46-1692">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="bde46-1692">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="bde46-1693">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="bde46-1693">Added `asg` application security group commands</span></span>
* <span data-ttu-id="bde46-1694">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="bde46-1694">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="bde46-1695">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bde46-1695">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="bde46-1696">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bde46-1696">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="bde46-1697">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1697">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1698">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1698">Storage</span></span>

* <span data-ttu-id="bde46-1699">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="bde46-1699">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="bde46-1700">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="bde46-1700">Eventgrid</span></span>

* <span data-ttu-id="bde46-1701">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="bde46-1701">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-1702">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-1702">SQL</span></span>

* <span data-ttu-id="bde46-1703">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="bde46-1703">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="bde46-1704">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="bde46-1704">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="bde46-1705">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="bde46-1705">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="bde46-1706">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bde46-1706">Keyvault</span></span>

* <span data-ttu-id="bde46-1707">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="bde46-1707">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1708">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1708">VM</span></span>

* <span data-ttu-id="bde46-1709">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="bde46-1709">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="bde46-1710">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="bde46-1710">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="bde46-1711">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="bde46-1711">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="bde46-1712">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="bde46-1712">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="bde46-1713">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="bde46-1713">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="bde46-1714">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="bde46-1714">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1715">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1715">ACS</span></span>

* <span data-ttu-id="bde46-1716">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="bde46-1716">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1717">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1717">Appservice</span></span>

* <span data-ttu-id="bde46-1718">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="bde46-1718">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="bde46-1719">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="bde46-1719">Backup</span></span>

* <span data-ttu-id="bde46-1720">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="bde46-1720">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="bde46-1721">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1721">September 11, 2017</span></span>

<span data-ttu-id="bde46-1722">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="bde46-1722">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="bde46-1723">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-1723">Core</span></span>

* <span data-ttu-id="bde46-1724">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="bde46-1724">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="bde46-1725">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="bde46-1725">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1726">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1726">Acs</span></span>

* <span data-ttu-id="bde46-1727">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1727">Added `acs list-locations` command</span></span>
* <span data-ttu-id="bde46-1728">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-1728">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1729">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1729">Appservice</span></span>

* <span data-ttu-id="bde46-1730">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="bde46-1730">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="bde46-1731">CDN</span><span class="sxs-lookup"><span data-stu-id="bde46-1731">CDN</span></span>

* <span data-ttu-id="bde46-1732">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1732">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="bde46-1733">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="bde46-1733">Extension</span></span>

* <span data-ttu-id="bde46-1734">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bde46-1734">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="bde46-1735">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bde46-1735">Keyvault</span></span>

* <span data-ttu-id="bde46-1736">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1736">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1737">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1737">Network</span></span>

* <span data-ttu-id="bde46-1738">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1738">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="bde46-1739">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1739">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="bde46-1740">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1740">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="bde46-1741">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1741">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="bde46-1742">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1742">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1743">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1743">Resource</span></span>

* <span data-ttu-id="bde46-1744">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1744">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="bde46-1745">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1745">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="bde46-1746">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1746">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="bde46-1747">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="bde46-1747">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-1748">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-1748">SQL</span></span>

* <span data-ttu-id="bde46-1749">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1749">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1750">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1750">VM</span></span>

* <span data-ttu-id="bde46-1751">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="bde46-1751">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="bde46-1752">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="bde46-1752">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="bde46-1753">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1753">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="bde46-1754">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="bde46-1754">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="bde46-1755">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="bde46-1755">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="bde46-1756">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1756">August 31, 2017</span></span>

<span data-ttu-id="bde46-1757">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="bde46-1757">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="bde46-1758">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bde46-1758">Keyvault</span></span>

* <span data-ttu-id="bde46-1759">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1759">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="bde46-1760">Sf</span><span class="sxs-lookup"><span data-stu-id="bde46-1760">Sf</span></span>

* <span data-ttu-id="bde46-1761">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="bde46-1761">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1762">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1762">Storage</span></span>

* <span data-ttu-id="bde46-1763">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="bde46-1763">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="bde46-1764">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="bde46-1764">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="bde46-1765">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1765">August 28, 2017</span></span>

<span data-ttu-id="bde46-1766">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="bde46-1766">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="bde46-1767">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="bde46-1767">CLI</span></span>

* <span data-ttu-id="bde46-1768">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="bde46-1768">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1769">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1769">ACS</span></span>

* <span data-ttu-id="bde46-1770">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="bde46-1770">Corrected preview regions</span></span>
* <span data-ttu-id="bde46-1771">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1771">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="bde46-1772">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="bde46-1772">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1773">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1773">Appservice</span></span>

* <span data-ttu-id="bde46-1774">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1774">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="bde46-1775">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1775">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="bde46-1776">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1776">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="bde46-1777">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="bde46-1777">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="bde46-1778">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="bde46-1778">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="bde46-1779">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bde46-1779">IoT</span></span>

* <span data-ttu-id="bde46-1780">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="bde46-1780">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1781">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1781">Network</span></span>

* <span data-ttu-id="bde46-1782">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1782">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="bde46-1783">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1783">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="bde46-1784">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1784">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="bde46-1785">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1785">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="bde46-1786">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1786">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="bde46-1787">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-1787">Profile</span></span>

* <span data-ttu-id="bde46-1788">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="bde46-1788">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="bde46-1789">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bde46-1789">Service Fabric</span></span>

* <span data-ttu-id="bde46-1790">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="bde46-1790">Preview release</span></span>
* <span data-ttu-id="bde46-1791">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="bde46-1791">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="bde46-1792">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="bde46-1792">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="bde46-1793">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1793">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1794">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1794">Storage</span></span>

* <span data-ttu-id="bde46-1795">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="bde46-1795">Enabled setting blob tier</span></span>
* <span data-ttu-id="bde46-1796">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-1796">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="bde46-1797">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1797">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="bde46-1798">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="bde46-1798">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="bde46-1799">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1799">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="bde46-1800">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1800">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1801">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1801">VM</span></span>

* <span data-ttu-id="bde46-1802">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1802">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="bde46-1803">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1803">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="bde46-1804">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="bde46-1804">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="bde46-1805">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="bde46-1805">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="bde46-1806">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="bde46-1806">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="bde46-1807">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1807">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="bde46-1808">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1808">August 15, 2017</span></span>

<span data-ttu-id="bde46-1809">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="bde46-1809">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1810">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1810">ACS</span></span>

* <span data-ttu-id="bde46-1811">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="bde46-1811">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1812">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1812">Appservice</span></span>

* <span data-ttu-id="bde46-1813">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="bde46-1813">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="bde46-1814">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-1814">Event Grid</span></span>

* <span data-ttu-id="bde46-1815">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="bde46-1815">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="bde46-1816">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1816">August 11, 2017</span></span>

<span data-ttu-id="bde46-1817">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="bde46-1817">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1818">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1818">ACS</span></span>

* <span data-ttu-id="bde46-1819">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="bde46-1819">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="bde46-1820">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-1820">Batch</span></span>

* <span data-ttu-id="bde46-1821">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="bde46-1821">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="bde46-1822">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="bde46-1822">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="bde46-1823">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1823">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="bde46-1824">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="bde46-1824">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="bde46-1825">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="bde46-1825">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="bde46-1826">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="bde46-1826">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="bde46-1827">Компонент</span><span class="sxs-lookup"><span data-stu-id="bde46-1827">Component</span></span>

* <span data-ttu-id="bde46-1828">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="bde46-1828">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="bde46-1829">Контейнер</span><span class="sxs-lookup"><span data-stu-id="bde46-1829">Container</span></span>

* <span data-ttu-id="bde46-1830">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="bde46-1830">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="bde46-1831">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bde46-1831">Data Lake Store</span></span>

* <span data-ttu-id="bde46-1832">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="bde46-1832">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="bde46-1833">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-1833">Event Grid</span></span>

* <span data-ttu-id="bde46-1834">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="bde46-1834">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1835">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1835">Network</span></span>

* <span data-ttu-id="bde46-1836">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="bde46-1836">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="bde46-1837">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1837">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="bde46-1838">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1838">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="bde46-1839">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1839">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="bde46-1840">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-1840">Profile</span></span>

* <span data-ttu-id="bde46-1841">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="bde46-1841">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-1842">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-1842">Storage</span></span>

* <span data-ttu-id="bde46-1843">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="bde46-1843">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-1844">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-1844">VM</span></span>

* <span data-ttu-id="bde46-1845">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="bde46-1845">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="bde46-1846">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1846">Exposed `list-skus` command</span></span>
* <span data-ttu-id="bde46-1847">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="bde46-1847">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="bde46-1848">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="bde46-1848">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="bde46-1849">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="bde46-1849">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="bde46-1850">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-1850">July 28, 2017</span></span>

<span data-ttu-id="bde46-1851">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="bde46-1851">Version 2.0.12</span></span>

* <span data-ttu-id="bde46-1852">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1852">Added container commands</span></span>
* <span data-ttu-id="bde46-1853">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1853">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="bde46-1854">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-1854">Core</span></span>

* <span data-ttu-id="bde46-1855">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="bde46-1855">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="bde46-1856">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="bde46-1856">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="bde46-1857">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="bde46-1857">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="bde46-1858">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="bde46-1858">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="bde46-1859">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="bde46-1859">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="bde46-1860">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="bde46-1860">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="bde46-1861">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="bde46-1861">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="bde46-1862">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="bde46-1862">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="bde46-1863">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="bde46-1863">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="bde46-1864">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="bde46-1864">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="bde46-1865">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="bde46-1865">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="bde46-1866">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="bde46-1866">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="bde46-1867">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="bde46-1867">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="bde46-1868">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="bde46-1868">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="bde46-1869">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="bde46-1869">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="bde46-1870">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="bde46-1870">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="bde46-1871">ACR</span><span class="sxs-lookup"><span data-stu-id="bde46-1871">ACR</span></span>

* <span data-ttu-id="bde46-1872">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1872">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="bde46-1873">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="bde46-1873">Support SKU update for managed registries</span></span>
* <span data-ttu-id="bde46-1874">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="bde46-1874">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="bde46-1875">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="bde46-1875">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="bde46-1876">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="bde46-1876">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="bde46-1877">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="bde46-1877">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-1878">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-1878">ACS</span></span>

* <span data-ttu-id="bde46-1879">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="bde46-1879">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-1880">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="bde46-1880">Appservice</span></span>

* <span data-ttu-id="bde46-1881">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="bde46-1881">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="bde46-1882">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="bde46-1882">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="bde46-1883">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1883">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="bde46-1884">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="bde46-1884">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="bde46-1885">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="bde46-1885">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="bde46-1886">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="bde46-1886">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="bde46-1887">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="bde46-1887">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="bde46-1888">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="bde46-1888">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="bde46-1889">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="bde46-1889">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="bde46-1890">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1890">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="bde46-1891">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="bde46-1891">Batch</span></span>

* <span data-ttu-id="bde46-1892">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="bde46-1892">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="bde46-1893">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1893">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="bde46-1894">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1894">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="bde46-1895">CDN</span><span class="sxs-lookup"><span data-stu-id="bde46-1895">CDN</span></span>

* <span data-ttu-id="bde46-1896">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="bde46-1896">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="bde46-1897">Облако</span><span class="sxs-lookup"><span data-stu-id="bde46-1897">Cloud</span></span>

* <span data-ttu-id="bde46-1898">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="bde46-1898">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="bde46-1899">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="bde46-1899">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="bde46-1900">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="bde46-1900">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="bde46-1901">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="bde46-1901">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="bde46-1902">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1902">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bde46-1903">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bde46-1903">CosmosDB</span></span>

* <span data-ttu-id="bde46-1904">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="bde46-1904">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="bde46-1905">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="bde46-1905">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bde46-1906">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bde46-1906">Data Lake Analytics</span></span>

* <span data-ttu-id="bde46-1907">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1907">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="bde46-1908">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1908">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="bde46-1909">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1909">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bde46-1910">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bde46-1910">Data Lake Store</span></span>

* <span data-ttu-id="bde46-1911">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1911">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="bde46-1912">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="bde46-1912">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="bde46-1913">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1913">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="bde46-1914">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="bde46-1914">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="bde46-1915">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="bde46-1915">Interactive</span></span>

* <span data-ttu-id="bde46-1916">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="bde46-1916">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="bde46-1917">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="bde46-1917">Increased test coverage</span></span>
* <span data-ttu-id="bde46-1918">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="bde46-1918">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="bde46-1919">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="bde46-1919">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="bde46-1920">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="bde46-1920">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="bde46-1921">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="bde46-1921">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="bde46-1922">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="bde46-1922">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="bde46-1923">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1923">Added `--progress` flag</span></span>
* <span data-ttu-id="bde46-1924">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1924">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="bde46-1925">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="bde46-1925">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="bde46-1926">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="bde46-1926">IoT</span></span>

* <span data-ttu-id="bde46-1927">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="bde46-1927">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="bde46-1928">(3934).</span><span class="sxs-lookup"><span data-stu-id="bde46-1928">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="bde46-1929">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bde46-1929">Key vault</span></span>

* <span data-ttu-id="bde46-1930">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="bde46-1930">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="bde46-1931">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1931">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="bde46-1932">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="bde46-1932">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="bde46-1933">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="bde46-1933">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="bde46-1934">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1934">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="bde46-1935">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="bde46-1935">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="bde46-1936">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="bde46-1936">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="bde46-1937">(3307).</span><span class="sxs-lookup"><span data-stu-id="bde46-1937">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="bde46-1938">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="bde46-1938">Lab</span></span>

* <span data-ttu-id="bde46-1939">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1939">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="bde46-1940">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1940">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-1941">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-1941">Monitor</span></span>

* <span data-ttu-id="bde46-1942">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="bde46-1942">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="bde46-1943">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1943">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="bde46-1944">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1944">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="bde46-1945">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1945">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="bde46-1946">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1946">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="bde46-1947">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="bde46-1947">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="bde46-1948">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="bde46-1948">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="bde46-1949">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="bde46-1949">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="bde46-1950">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="bde46-1950">`location` no longer required</span></span>
  * <span data-ttu-id="bde46-1951">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="bde46-1951">Add name and ID support for target</span></span>
  * <span data-ttu-id="bde46-1952">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="bde46-1952">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="bde46-1953">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="bde46-1953">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="bde46-1954">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="bde46-1954">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="bde46-1955">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="bde46-1955">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="bde46-1956">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1956">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="bde46-1957">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1957">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="bde46-1958">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-1958">Network</span></span>

* <span data-ttu-id="bde46-1959">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1959">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="bde46-1960">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1960">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="bde46-1961">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="bde46-1961">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="bde46-1962">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1962">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="bde46-1963">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1963">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="bde46-1964">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1964">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="bde46-1965">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1965">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="bde46-1966">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1966">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="bde46-1967">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1967">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="bde46-1968">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1968">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="bde46-1969">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1969">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="bde46-1970">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1970">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="bde46-1971">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1971">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="bde46-1972">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1972">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="bde46-1973">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1973">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="bde46-1974">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1974">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="bde46-1975">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="bde46-1975">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="bde46-1976">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1976">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="bde46-1977">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1977">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="bde46-1978">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1978">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="bde46-1979">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1979">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="bde46-1980">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1980">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="bde46-1981">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1981">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="bde46-1982">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="bde46-1982">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="bde46-1983">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="bde46-1983">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="bde46-1984">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="bde46-1984">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="bde46-1985">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="bde46-1985">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="bde46-1986">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-1986">Profile</span></span>

* <span data-ttu-id="bde46-1987">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="bde46-1987">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="bde46-1988">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="bde46-1988">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="bde46-1989">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="bde46-1989">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="bde46-1990">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="bde46-1990">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="bde46-1991">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="bde46-1991">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="bde46-1992">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="bde46-1992">RDBMS</span></span>

* <span data-ttu-id="bde46-1993">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="bde46-1993">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="bde46-1994">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="bde46-1994">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="bde46-1995">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="bde46-1995">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="bde46-1996">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="bde46-1996">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-1997">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-1997">Resource</span></span>

* <span data-ttu-id="bde46-1998">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1998">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="bde46-1999">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="bde46-1999">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="bde46-2000">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2000">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="bde46-2001">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2001">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="bde46-2002">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="bde46-2002">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="bde46-2003">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2003">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="bde46-2004">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="bde46-2004">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="bde46-2005">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2005">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="bde46-2006">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-2006">Role</span></span>

* <span data-ttu-id="bde46-2007">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="bde46-2007">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="bde46-2008">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="bde46-2008">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="bde46-2009">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="bde46-2009">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="bde46-2010">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="bde46-2010">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="bde46-2011">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2011">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="bde46-2012">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="bde46-2012">Service Fabric</span></span>
* <span data-ttu-id="bde46-2013">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="bde46-2013">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="bde46-2014">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="bde46-2014">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="bde46-2015">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="bde46-2015">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-2016">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-2016">SQL</span></span>

* <span data-ttu-id="bde46-2017">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2017">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="bde46-2018">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2018">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="bde46-2019">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2019">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-2020">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-2020">Storage</span></span>

* <span data-ttu-id="bde46-2021">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="bde46-2021">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="bde46-2022">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="bde46-2022">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="bde46-2023">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="bde46-2023">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="bde46-2024">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="bde46-2024">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="bde46-2025">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="bde46-2025">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="bde46-2026">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="bde46-2026">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-2027">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-2027">VM</span></span>

* <span data-ttu-id="bde46-2028">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="bde46-2028">Support configuring nsg</span></span>
* <span data-ttu-id="bde46-2029">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="bde46-2029">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="bde46-2030">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="bde46-2030">Support managed service identities</span></span>
* <span data-ttu-id="bde46-2031">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2031">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="bde46-2032">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="bde46-2032">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="bde46-2033">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-2033">May 10, 2017</span></span>

<span data-ttu-id="bde46-2034">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="bde46-2034">Version 2.0.6</span></span>

* <span data-ttu-id="bde46-2035">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="bde46-2035">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="bde46-2036">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="bde46-2036">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="bde46-2037">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="bde46-2037">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="bde46-2038">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="bde46-2038">Include Cognitive Services module</span></span>
* <span data-ttu-id="bde46-2039">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="bde46-2039">Include Service Fabric module</span></span>
* <span data-ttu-id="bde46-2040">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="bde46-2040">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="bde46-2041">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="bde46-2041">Add support for CDN commands</span></span>
* <span data-ttu-id="bde46-2042">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="bde46-2042">Remove Container module</span></span>
* <span data-ttu-id="bde46-2043">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2043">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="bde46-2044">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2044">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="bde46-2045">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-2045">Core</span></span>

* <span data-ttu-id="bde46-2046">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="bde46-2046">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="bde46-2047">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2047">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="bde46-2048">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2048">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="bde46-2049">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2049">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="bde46-2050">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2050">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="bde46-2051">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2051">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="bde46-2052">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2052">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="bde46-2053">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2053">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="bde46-2054">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2054">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="bde46-2055">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="bde46-2055">core: Improved performance</span></span>
* <span data-ttu-id="bde46-2056">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="bde46-2056">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="bde46-2057">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="bde46-2057">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-2058">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-2058">ACS</span></span>

* <span data-ttu-id="bde46-2059">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="bde46-2059">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="bde46-2060">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="bde46-2060">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="bde46-2061">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="bde46-2061">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="bde46-2062">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2062">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-2063">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-2063">AppService</span></span>

* <span data-ttu-id="bde46-2064">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="bde46-2064">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="bde46-2065">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="bde46-2065">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="bde46-2066">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="bde46-2066">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="bde46-2067">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="bde46-2067">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="bde46-2068">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="bde46-2068">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="bde46-2069">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2069">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="bde46-2070">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="bde46-2070">support slot swap with preview</span></span>
* <span data-ttu-id="bde46-2071">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2071">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="bde46-2072">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2072">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="bde46-2073">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="bde46-2073">CosmosDB</span></span>

* <span data-ttu-id="bde46-2074">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="bde46-2074">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="bde46-2075">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="bde46-2075">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="bde46-2076">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="bde46-2076">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="bde46-2077">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="bde46-2077">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="bde46-2078">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="bde46-2078">Data Lake Analytics</span></span>

* <span data-ttu-id="bde46-2079">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="bde46-2079">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="bde46-2080">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="bde46-2080">Add support for new catalog item type: package.</span></span> <span data-ttu-id="bde46-2081">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2081">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="bde46-2082">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="bde46-2082">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="bde46-2083">Таблица</span><span class="sxs-lookup"><span data-stu-id="bde46-2083">Table</span></span>
  * <span data-ttu-id="bde46-2084">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="bde46-2084">Table valued function</span></span>
  * <span data-ttu-id="bde46-2085">Просмотр</span><span class="sxs-lookup"><span data-stu-id="bde46-2085">View</span></span>
  * <span data-ttu-id="bde46-2086">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="bde46-2086">Table Statistics.</span></span> <span data-ttu-id="bde46-2087">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="bde46-2087">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="bde46-2088">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="bde46-2088">Data Lake Store</span></span>

* <span data-ttu-id="bde46-2089">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="bde46-2089">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="bde46-2090">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2090">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="bde46-2091">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="bde46-2091">missed help for access show.</span></span> <span data-ttu-id="bde46-2092">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="bde46-2092">adding it.</span></span> <span data-ttu-id="bde46-2093">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="bde46-2093">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="bde46-2094">Поиск</span><span class="sxs-lookup"><span data-stu-id="bde46-2094">Find</span></span>

* <span data-ttu-id="bde46-2095">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="bde46-2095">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="bde46-2096">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="bde46-2096">KeyVault</span></span>

* <span data-ttu-id="bde46-2097">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="bde46-2097">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="bde46-2098">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="bde46-2098">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="bde46-2099">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="bde46-2099">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="bde46-2100">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="bde46-2100">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="bde46-2101">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2101">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="bde46-2102">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="bde46-2102">Lab</span></span>

* <span data-ttu-id="bde46-2103">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="bde46-2103">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="bde46-2104">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="bde46-2104">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="bde46-2105">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="bde46-2105">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="bde46-2106">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="bde46-2106">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="bde46-2107">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="bde46-2107">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="bde46-2108">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="bde46-2108">Monitor</span></span>

* <span data-ttu-id="bde46-2109">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2109">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="bde46-2110">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2110">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="bde46-2111">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-2111">Network</span></span>

* <span data-ttu-id="bde46-2112">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2112">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="bde46-2113">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2113">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="bde46-2114">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="bde46-2114">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="bde46-2115">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="bde46-2115">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="bde46-2116">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="bde46-2116">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="bde46-2117">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="bde46-2117">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="bde46-2118">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="bde46-2118">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="bde46-2119">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="bde46-2119">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="bde46-2120">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2120">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="bde46-2121">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="bde46-2121">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="bde46-2122">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2122">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="bde46-2123">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2123">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="bde46-2124">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="bde46-2124">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="bde46-2125">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="bde46-2125">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="bde46-2126">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="bde46-2126">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="bde46-2127">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="bde46-2127">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="bde46-2128">Профиль</span><span class="sxs-lookup"><span data-stu-id="bde46-2128">Profile</span></span>

* <span data-ttu-id="bde46-2129">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2129">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="bde46-2130">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2130">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="bde46-2131">Redis</span><span class="sxs-lookup"><span data-stu-id="bde46-2131">Redis</span></span>

* <span data-ttu-id="bde46-2132">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="bde46-2132">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="bde46-2133">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="bde46-2133">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="bde46-2134">Ресурс</span><span class="sxs-lookup"><span data-stu-id="bde46-2134">Resource</span></span>

* <span data-ttu-id="bde46-2135">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2135">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="bde46-2136">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2136">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="bde46-2137">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2137">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="bde46-2138">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="bde46-2138">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="bde46-2139">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="bde46-2139">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="bde46-2140">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="bde46-2140">Add docs for az lock update.</span></span> <span data-ttu-id="bde46-2141">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="bde46-2141">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="bde46-2142">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="bde46-2142">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="bde46-2143">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="bde46-2143">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="bde46-2144">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="bde46-2144">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="bde46-2145">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="bde46-2145">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="bde46-2146">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2146">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="bde46-2147">Роль</span><span class="sxs-lookup"><span data-stu-id="bde46-2147">Role</span></span>

* <span data-ttu-id="bde46-2148">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2148">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="bde46-2149">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2149">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="bde46-2150">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2150">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="bde46-2151">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="bde46-2151">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="bde46-2152">SQL</span><span class="sxs-lookup"><span data-stu-id="bde46-2152">SQL</span></span>

* <span data-ttu-id="bde46-2153">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="bde46-2153">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="bde46-2154">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2154">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="bde46-2155">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-2155">Storage</span></span>

* <span data-ttu-id="bde46-2156">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2156">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="bde46-2157">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="bde46-2157">Add support for incremental blob copy</span></span>
* <span data-ttu-id="bde46-2158">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="bde46-2158">Add support for large block blob upload</span></span>
* <span data-ttu-id="bde46-2159">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="bde46-2159">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-2160">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-2160">VM</span></span>

* <span data-ttu-id="bde46-2161">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="bde46-2161">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="bde46-2162">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="bde46-2162">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="bde46-2163">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="bde46-2163">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="bde46-2164">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="bde46-2164">az vm/vmss disk</span></span>
  3. <span data-ttu-id="bde46-2165">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="bde46-2165">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="bde46-2166">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="bde46-2166">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="bde46-2167">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2167">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="bde46-2168">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-2168">April 3, 2017</span></span>

<span data-ttu-id="bde46-2169">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="bde46-2169">Version 2.0.2</span></span>

<span data-ttu-id="bde46-2170">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="bde46-2170">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="bde46-2171">Core</span><span class="sxs-lookup"><span data-stu-id="bde46-2171">Core</span></span>

* <span data-ttu-id="bde46-2172">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-2172">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="bde46-2173">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2173">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="bde46-2174">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2174">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="bde46-2175">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2175">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="bde46-2176">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2176">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="bde46-2177">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="bde46-2177">Add prompting for missing template parameters.</span></span> <span data-ttu-id="bde46-2178">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2178">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="bde46-2179">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bde46-2179">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="bde46-2180">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="bde46-2180">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="bde46-2181">ACS</span><span class="sxs-lookup"><span data-stu-id="bde46-2181">ACS</span></span>

* <span data-ttu-id="bde46-2182">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2182">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="bde46-2183">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="bde46-2183">Add support for ssh key password prompting.</span></span> <span data-ttu-id="bde46-2184">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2184">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="bde46-2185">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="bde46-2185">Add support for windows clusters.</span></span> <span data-ttu-id="bde46-2186">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2186">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="bde46-2187">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="bde46-2187">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="bde46-2188">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2188">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="bde46-2189">AppService</span><span class="sxs-lookup"><span data-stu-id="bde46-2189">AppService</span></span>

* <span data-ttu-id="bde46-2190">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2190">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="bde46-2191">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2191">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="bde46-2192">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2192">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="bde46-2193">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2193">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="bde46-2194">Data Lake</span><span class="sxs-lookup"><span data-stu-id="bde46-2194">DataLake</span></span>

* <span data-ttu-id="bde46-2195">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="bde46-2195">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="bde46-2196">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="bde46-2196">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="bde46-2197">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="bde46-2197">DocuemntDB</span></span>

* <span data-ttu-id="bde46-2198">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2198">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="bde46-2199">ВМ</span><span class="sxs-lookup"><span data-stu-id="bde46-2199">VM</span></span>

* <span data-ttu-id="bde46-2200">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2200">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="bde46-2201">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2201">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="bde46-2202">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2202">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="bde46-2203">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2203">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="bde46-2204">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2204">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="bde46-2205">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2205">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="bde46-2206">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="bde46-2206">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="bde46-2207">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="bde46-2207">February 27, 2017</span></span>

<span data-ttu-id="bde46-2208">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="bde46-2208">Version 2.0.0</span></span>

<span data-ttu-id="bde46-2209">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="bde46-2209">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="bde46-2210">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="bde46-2210">Container Service (acs)</span></span>
- <span data-ttu-id="bde46-2211">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="bde46-2211">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="bde46-2212">Сеть</span><span class="sxs-lookup"><span data-stu-id="bde46-2212">Networking</span></span>
- <span data-ttu-id="bde46-2213">Хранилище</span><span class="sxs-lookup"><span data-stu-id="bde46-2213">Storage</span></span>

<span data-ttu-id="bde46-2214">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2214">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="bde46-2215">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="bde46-2215">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="bde46-2216">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="bde46-2216">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="bde46-2217">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="bde46-2217">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="bde46-2218">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="bde46-2218">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="bde46-2219">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="bde46-2219">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="bde46-2220">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="bde46-2220">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="bde46-2221">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="bde46-2221">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="bde46-2222">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="bde46-2222">Provide feedback from the command line with the `az feedback` command</span></span>

