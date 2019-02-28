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
ms.openlocfilehash: 1c6b2cc57b80256faff0a174bec5f13bd84f5a1b
ms.sourcegitcommit: 7f79860c799e78fd8a591d7a5550464080e07aa9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/12/2019
ms.locfileid: "56158732"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="955b5-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="955b5-103">Azure CLI release notes</span></span>
## <a name="february-12-2019"></a><span data-ttu-id="955b5-104">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-104">February 12, 2019</span></span>

<span data-ttu-id="955b5-105">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="955b5-105">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="955b5-106">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-106">Core</span></span>

* <span data-ttu-id="955b5-107">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="955b5-107">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="955b5-108">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="955b5-108">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-109">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-109">ACR</span></span>
* <span data-ttu-id="955b5-110">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="955b5-110">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="955b5-111">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="955b5-111">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-112">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-112">ACS</span></span>
* <span data-ttu-id="955b5-113">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="955b5-113">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="955b5-114">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="955b5-114">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="955b5-115">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="955b5-115">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="955b5-116">AMS</span><span class="sxs-lookup"><span data-stu-id="955b5-116">AMS</span></span>
* <span data-ttu-id="955b5-117">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-117">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="955b5-118">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-118">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-119">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-119">Appservice</span></span>
* <span data-ttu-id="955b5-120">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="955b5-120">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="955b5-121">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="955b5-121">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="955b5-122">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-122">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="955b5-123">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="955b5-123">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="955b5-124">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="955b5-124">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="955b5-125">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="955b5-125">Botservice</span></span>
* <span data-ttu-id="955b5-126">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="955b5-126">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="955b5-127">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="955b5-127">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="955b5-128">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-128">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="955b5-129">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="955b5-129">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="955b5-130">[УСТАРЕЛО.] Аргумент `--proj-name` не поддерживается. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="955b5-130">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="955b5-131">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="955b5-131">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="955b5-132">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="955b5-132">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="955b5-133">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="955b5-133">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="955b5-134">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="955b5-134">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="955b5-135">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="955b5-135">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="955b5-136">Key Vault</span><span class="sxs-lookup"><span data-stu-id="955b5-136">Key Vault</span></span>
* <span data-ttu-id="955b5-137">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="955b5-137">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-138">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-138">Monitor</span></span>
* <span data-ttu-id="955b5-139">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="955b5-139">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="955b5-140">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-140">Network</span></span>
* <span data-ttu-id="955b5-141">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="955b5-141">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="955b5-142">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="955b5-142">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="955b5-143">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="955b5-143">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="955b5-144">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="955b5-144">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="955b5-145">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="955b5-145">Policy Insights</span></span>
* <span data-ttu-id="955b5-146">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="955b5-146">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="955b5-147">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="955b5-147">RDBMS</span></span>
* <span data-ttu-id="955b5-148">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="955b5-148">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="955b5-149">Redis</span><span class="sxs-lookup"><span data-stu-id="955b5-149">Redis</span></span>
* <span data-ttu-id="955b5-150">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="955b5-150">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="955b5-151">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="955b5-151">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="955b5-152">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="955b5-152">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="955b5-153">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="955b5-153">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="955b5-154">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="955b5-154">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="955b5-155">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="955b5-155">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="955b5-156">[УСТРАРЕЛО.] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955b5-156">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="955b5-157">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-157">Role</span></span>
* <span data-ttu-id="955b5-158">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="955b5-158">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="955b5-159">ВМ SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-159">SQL VM</span></span>
* <span data-ttu-id="955b5-160">[УСТАРЕЛО.] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="955b5-160">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-161">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-161">VM</span></span>
* <span data-ttu-id="955b5-162">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="955b5-162">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="955b5-163">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-163">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="955b5-164">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="955b5-164">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="955b5-165">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="955b5-165">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="955b5-166">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-166">January 31, 2019</span></span>

<span data-ttu-id="955b5-167">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="955b5-167">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="955b5-168">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-168">Core</span></span>

* <span data-ttu-id="955b5-169">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="955b5-169">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="955b5-170">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-170">January 28, 2019</span></span>

<span data-ttu-id="955b5-171">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="955b5-171">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-172">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-172">ACR</span></span>
* <span data-ttu-id="955b5-173">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="955b5-173">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-174">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-174">ACS</span></span>
* <span data-ttu-id="955b5-175">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="955b5-175">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="955b5-176">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="955b5-176">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="955b5-177">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="955b5-177">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="955b5-178">AMS</span><span class="sxs-lookup"><span data-stu-id="955b5-178">AMS</span></span>
* <span data-ttu-id="955b5-179">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="955b5-179">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="955b5-180">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="955b5-180">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-181">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-181">Appservice</span></span>
* <span data-ttu-id="955b5-182">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-182">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="955b5-183">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="955b5-183">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="955b5-184">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="955b5-184">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="955b5-185">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-185">Container</span></span>
* <span data-ttu-id="955b5-186">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="955b5-186">Added `container start` command</span></span>
* <span data-ttu-id="955b5-187">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-187">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="955b5-188">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="955b5-188">EventGrid</span></span>
* <span data-ttu-id="955b5-189">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-189">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="955b5-190">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="955b5-190">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="955b5-191">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="955b5-191">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="955b5-192">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="955b5-192">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="955b5-193">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="955b5-193">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="955b5-194">HDInsight</span><span class="sxs-lookup"><span data-stu-id="955b5-194">HDInsight</span></span>
* <span data-ttu-id="955b5-195">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="955b5-195">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="955b5-196">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="955b5-196">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="955b5-197">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-197">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="955b5-198">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="955b5-198">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="955b5-199">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="955b5-199">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="955b5-200">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-200">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="955b5-201">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="955b5-201">IoT</span></span>
* <span data-ttu-id="955b5-202">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="955b5-202">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="955b5-203">Kusto</span><span class="sxs-lookup"><span data-stu-id="955b5-203">Kusto</span></span>
* <span data-ttu-id="955b5-204">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="955b5-204">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-205">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-205">Monitor</span></span>
* <span data-ttu-id="955b5-206">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="955b5-206">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="955b5-207">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-207">Profile</span></span>
* <span data-ttu-id="955b5-208">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-208">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="955b5-209">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-209">Network</span></span>
* <span data-ttu-id="955b5-210">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="955b5-210">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="955b5-211">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="955b5-211">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-212">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-212">Resource</span></span>
* <span data-ttu-id="955b5-213">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-213">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="955b5-214">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-214">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="955b5-215">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-215">SQL Virtual Machine</span></span>
* <span data-ttu-id="955b5-216">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="955b5-216">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-217">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-217">Storage</span></span>
* <span data-ttu-id="955b5-218">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="955b5-218">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="955b5-219">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="955b5-219">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-220">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-220">VM</span></span>
* <span data-ttu-id="955b5-221">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="955b5-221">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="955b5-222">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="955b5-222">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="955b5-223">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-223">January 15, 2019</span></span>

<span data-ttu-id="955b5-224">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="955b5-224">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-225">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-225">ACR</span></span>
* <span data-ttu-id="955b5-226">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="955b5-226">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="955b5-227">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="955b5-227">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="955b5-228">[УСТАРЕЛО.] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="955b5-228">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="955b5-229">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-229">ACS</span></span>
* <span data-ttu-id="955b5-230">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="955b5-230">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-231">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-231">Appservice</span></span>
* <span data-ttu-id="955b5-232">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="955b5-232">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="955b5-233">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="955b5-233">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="955b5-234">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="955b5-234">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="955b5-235">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="955b5-235">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="955b5-236">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="955b5-236">Botservice</span></span>
* <span data-ttu-id="955b5-237">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-237">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="955b5-238">Настройка</span><span class="sxs-lookup"><span data-stu-id="955b5-238">Configure</span></span>
* <span data-ttu-id="955b5-239">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="955b5-239">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="955b5-240">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="955b5-240">CosmosDB</span></span>
* <span data-ttu-id="955b5-241">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="955b5-241">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="955b5-242">HDInsight</span><span class="sxs-lookup"><span data-stu-id="955b5-242">HDInsight</span></span>
* <span data-ttu-id="955b5-243">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="955b5-243">Added commands for managing applications</span></span>
* <span data-ttu-id="955b5-244">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="955b5-244">Added commands for managing script actions</span></span>
* <span data-ttu-id="955b5-245">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="955b5-245">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="955b5-246">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="955b5-246">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="955b5-247">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-247">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="955b5-248">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-248">Network</span></span>
* <span data-ttu-id="955b5-249">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="955b5-249">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="955b5-250">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="955b5-250">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="955b5-251">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="955b5-251">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="955b5-252">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-252">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="955b5-253">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-253">Role</span></span>
* <span data-ttu-id="955b5-254">[УСТАРЕЛО.] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="955b5-254">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="955b5-255">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="955b5-255">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="955b5-256">Безопасность</span><span class="sxs-lookup"><span data-stu-id="955b5-256">Security</span></span>
* <span data-ttu-id="955b5-257">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="955b5-257">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-258">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-258">Storage</span></span>
* <span data-ttu-id="955b5-259">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="955b5-259">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="955b5-260">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="955b5-260">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="955b5-261">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="955b5-261">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="955b5-262">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="955b5-262">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="955b5-263">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="955b5-263">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-264">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-264">VM</span></span>
* <span data-ttu-id="955b5-265">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="955b5-265">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="955b5-266">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-266">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="955b5-267">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="955b5-267">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="955b5-268">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="955b5-268">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="955b5-269">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-269">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="955b5-270">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="955b5-270">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="955b5-271">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-271">December 20, 2018</span></span>

<span data-ttu-id="955b5-272">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="955b5-272">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="955b5-273">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-273">Appservice</span></span>
* <span data-ttu-id="955b5-274">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="955b5-274">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="955b5-275">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="955b5-275">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="955b5-276">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="955b5-276">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="955b5-277">IoT Central</span><span class="sxs-lookup"><span data-stu-id="955b5-277">IoTCentral</span></span>
* <span data-ttu-id="955b5-278">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="955b5-278">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="955b5-279">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-279">Role</span></span>
* <span data-ttu-id="955b5-280">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="955b5-280">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-281">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-281">SQL</span></span>
* <span data-ttu-id="955b5-282">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="955b5-282">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-283">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-283">VM</span></span>
* <span data-ttu-id="955b5-284">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-284">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="955b5-285">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-285">December 18, 2018</span></span>

<span data-ttu-id="955b5-286">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="955b5-286">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="955b5-287">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-287">ACR</span></span>
* <span data-ttu-id="955b5-288">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-288">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="955b5-289">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="955b5-289">Condensed the table layout for task list</span></span>
* <span data-ttu-id="955b5-290">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="955b5-290">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-291">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-291">ACS</span></span>
* <span data-ttu-id="955b5-292">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="955b5-292">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="955b5-293">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="955b5-293">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="955b5-294">[УСТАРЕЛО] Команды `az acs` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="955b5-294">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="955b5-295">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-295">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="955b5-296">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="955b5-296">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="955b5-297">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="955b5-297">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-298">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-298">Appservice</span></span>
* <span data-ttu-id="955b5-299">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="955b5-299">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="955b5-300">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="955b5-300">Botservice</span></span>
* <span data-ttu-id="955b5-301">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-301">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="955b5-302">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="955b5-302">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="955b5-303">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="955b5-303">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="955b5-304">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="955b5-304">Reduced Kudu network calls</span></span>
* <span data-ttu-id="955b5-305">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="955b5-305">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="955b5-306">Потребление</span><span class="sxs-lookup"><span data-stu-id="955b5-306">Consumption</span></span>
* <span data-ttu-id="955b5-307">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="955b5-307">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="955b5-308">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="955b5-308">CosmosDB</span></span>
* <span data-ttu-id="955b5-309">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="955b5-309">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="955b5-310">Карты</span><span class="sxs-lookup"><span data-stu-id="955b5-310">Maps</span></span>
* <span data-ttu-id="955b5-311">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="955b5-311">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="955b5-312">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-312">Network</span></span>
* <span data-ttu-id="955b5-313">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="955b5-313">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="955b5-314">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="955b5-314">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-315">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-315">Resource</span></span>
* <span data-ttu-id="955b5-316">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-316">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="955b5-317">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-317">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-318">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-318">Storage</span></span>
*  <span data-ttu-id="955b5-319">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="955b5-319">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-320">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-320">VM</span></span>
* <span data-ttu-id="955b5-321">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-321">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="955b5-322">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-322">December 4, 2018</span></span>

<span data-ttu-id="955b5-323">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="955b5-323">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="955b5-324">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-324">Core</span></span>
* <span data-ttu-id="955b5-325">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-325">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="955b5-326">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="955b5-326">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-327">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-327">Appservice</span></span>
* <span data-ttu-id="955b5-328">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="955b5-328">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="955b5-329">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="955b5-329">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="955b5-330">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-330">Network</span></span>
* <span data-ttu-id="955b5-331">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="955b5-331">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="955b5-332">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-332">Role</span></span>
* <span data-ttu-id="955b5-333">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="955b5-333">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="955b5-334">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-334">VM</span></span>
* <span data-ttu-id="955b5-335">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` устарел.</span><span class="sxs-lookup"><span data-stu-id="955b5-335">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="955b5-336">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="955b5-336">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="955b5-337">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="955b5-337">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="955b5-338">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="955b5-338">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="955b5-339">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-339">November 20, 2018</span></span>

<span data-ttu-id="955b5-340">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="955b5-340">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="955b5-341">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-341">Core</span></span>
* <span data-ttu-id="955b5-342">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="955b5-342">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-343">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-343">ACR</span></span>
* <span data-ttu-id="955b5-344">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="955b5-344">Added context token to task step</span></span>
* <span data-ttu-id="955b5-345">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="955b5-345">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="955b5-346">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="955b5-346">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-347">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-347">Appservice</span></span>
* <span data-ttu-id="955b5-348">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="955b5-348">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="955b5-349">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-349">Updated the default `node_version`.</span></span> <span data-ttu-id="955b5-350">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="955b5-350">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="955b5-351">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="955b5-351">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="955b5-352">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="955b5-352">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="955b5-353">IotCentral</span><span class="sxs-lookup"><span data-stu-id="955b5-353">IotCentral</span></span>
* <span data-ttu-id="955b5-354">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="955b5-354">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="955b5-355">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="955b5-355">KeyVault</span></span>
* <span data-ttu-id="955b5-356">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="955b5-356">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="955b5-357">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-357">Network</span></span>
* <span data-ttu-id="955b5-358">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="955b5-358">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="955b5-359">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="955b5-359">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="955b5-360">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="955b5-360">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="955b5-361">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="955b5-361">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="955b5-362">Rdbms</span><span class="sxs-lookup"><span data-stu-id="955b5-362">Rdbms</span></span>
* <span data-ttu-id="955b5-363">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="955b5-363">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="955b5-364">RBAC:</span><span class="sxs-lookup"><span data-stu-id="955b5-364">Rbac</span></span>
* <span data-ttu-id="955b5-365">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-365">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="955b5-366">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="955b5-366">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="955b5-367">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-367">Storage</span></span>
* <span data-ttu-id="955b5-368">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="955b5-368">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="955b5-369">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="955b5-369">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="955b5-370">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="955b5-370">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="955b5-371">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="955b5-371">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-372">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-372">VM</span></span>
* <span data-ttu-id="955b5-373">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="955b5-373">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="955b5-374">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="955b5-374">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="955b5-375">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="955b5-375">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="955b5-376">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="955b5-376">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="955b5-377">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-377">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="955b5-378">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-378">Added `snapshot wait` command</span></span>
* <span data-ttu-id="955b5-379">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="955b5-379">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="955b5-380">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-380">November 6, 2018</span></span>

<span data-ttu-id="955b5-381">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="955b5-381">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="955b5-382">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-382">Core</span></span>
* <span data-ttu-id="955b5-383">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="955b5-383">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-384">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-384">ACR</span></span>
* <span data-ttu-id="955b5-385">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="955b5-385">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="955b5-386">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="955b5-386">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-387">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-387">ACS</span></span>
* <span data-ttu-id="955b5-388">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-388">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="955b5-389">Помощник</span><span class="sxs-lookup"><span data-stu-id="955b5-389">Advisor</span></span>
* <span data-ttu-id="955b5-390">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="955b5-390">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="955b5-391">AMS</span><span class="sxs-lookup"><span data-stu-id="955b5-391">AMS</span></span>
* <span data-ttu-id="955b5-392">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="955b5-392">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="955b5-393">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="955b5-393">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="955b5-394">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-394">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="955b5-395">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="955b5-395">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="955b5-396">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="955b5-396">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="955b5-397">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="955b5-397">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="955b5-398">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="955b5-398">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="955b5-399">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="955b5-399">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="955b5-400">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="955b5-400">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="955b5-401">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="955b5-401">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="955b5-402">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="955b5-402">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="955b5-403">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="955b5-403">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="955b5-404">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="955b5-404">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="955b5-405">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="955b5-405">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="955b5-406">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="955b5-406">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="955b5-407">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="955b5-407">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="955b5-408">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="955b5-408">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-409">AppService</span><span class="sxs-lookup"><span data-stu-id="955b5-409">AppService</span></span>
* <span data-ttu-id="955b5-410">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="955b5-410">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="955b5-411">Настройка</span><span class="sxs-lookup"><span data-stu-id="955b5-411">Configure</span></span>
* <span data-ttu-id="955b5-412">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="955b5-412">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="955b5-413">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-413">Container</span></span>
* <span data-ttu-id="955b5-414">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="955b5-414">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="955b5-415">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="955b5-415">EventHub</span></span>
* <span data-ttu-id="955b5-416">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-416">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-417">Interactive</span><span class="sxs-lookup"><span data-stu-id="955b5-417">Interactive</span></span>
* <span data-ttu-id="955b5-418">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="955b5-418">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-419">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-419">Monitor</span></span>
* <span data-ttu-id="955b5-420">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-420">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="955b5-421">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-421">Network</span></span>
* <span data-ttu-id="955b5-422">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="955b5-422">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="955b5-423">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="955b5-423">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="955b5-424">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-424">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="955b5-425">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-425">Profile</span></span>
* <span data-ttu-id="955b5-426">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="955b5-426">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="955b5-427">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="955b5-427">RDBMS</span></span>
* <span data-ttu-id="955b5-428">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="955b5-428">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-429">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-429">Resource</span></span>
* <span data-ttu-id="955b5-430">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="955b5-430">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="955b5-431">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-431">Role</span></span>
* <span data-ttu-id="955b5-432">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="955b5-432">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="955b5-433">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-433">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="955b5-434">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="955b5-434">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-435">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-435">Storage</span></span>
* <span data-ttu-id="955b5-436">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="955b5-436">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-437">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-437">VM</span></span>
* <span data-ttu-id="955b5-438">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="955b5-438">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="955b5-439">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="955b5-439">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="955b5-440">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="955b5-440">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="955b5-441">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="955b5-441">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="955b5-442">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="955b5-442">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="955b5-443">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="955b5-443">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="955b5-444">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-444">October 23, 2018</span></span>

<span data-ttu-id="955b5-445">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="955b5-445">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="955b5-446">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-446">Core</span></span>
* <span data-ttu-id="955b5-447">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="955b5-447">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="955b5-448">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="955b5-448">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-449">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-449">ACR</span></span>
* <span data-ttu-id="955b5-450">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="955b5-450">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="955b5-451">CDN</span><span class="sxs-lookup"><span data-stu-id="955b5-451">CDN</span></span>
* <span data-ttu-id="955b5-452">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-452">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="955b5-453">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="955b5-453">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="955b5-454">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-454">Container</span></span>
* <span data-ttu-id="955b5-455">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="955b5-455">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="955b5-456">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="955b5-456">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="955b5-457">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="955b5-457">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="955b5-458">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-458">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="955b5-459">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="955b5-459">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="955b5-460">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="955b5-460">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="955b5-461">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-461">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="955b5-462">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="955b5-462">CosmosDB</span></span>
* <span data-ttu-id="955b5-463">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="955b5-463">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-464">Interactive</span><span class="sxs-lookup"><span data-stu-id="955b5-464">Interactive</span></span>
* <span data-ttu-id="955b5-465">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="955b5-465">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="955b5-466">IoT Central</span><span class="sxs-lookup"><span data-stu-id="955b5-466">IoT Central</span></span>
* <span data-ttu-id="955b5-467">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="955b5-467">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="955b5-468">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="955b5-468">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-469">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-469">Monitor</span></span>
* <span data-ttu-id="955b5-470">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="955b5-470">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="955b5-471">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="955b5-471">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="955b5-472">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="955b5-472">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="955b5-473">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="955b5-473">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="955b5-474">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="955b5-474">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="955b5-475">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="955b5-475">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="955b5-476">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="955b5-476">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="955b5-477">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="955b5-477">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="955b5-478">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="955b5-478">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="955b5-479">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-479">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="955b5-480">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-480">Network</span></span>
* <span data-ttu-id="955b5-481">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="955b5-481">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="955b5-482">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="955b5-482">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="955b5-483">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="955b5-483">ServiceBus</span></span>
* <span data-ttu-id="955b5-484">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="955b5-484">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-485">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-485">SQL</span></span>
* <span data-ttu-id="955b5-486">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="955b5-486">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-487">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-487">Storage</span></span>
* <span data-ttu-id="955b5-488">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-488">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="955b5-489">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="955b5-489">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-490">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-490">VM</span></span>
* <span data-ttu-id="955b5-491">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="955b5-491">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="955b5-492">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="955b5-492">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="955b5-493">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="955b5-493">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="955b5-494">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-494">October 16, 2018</span></span>

<span data-ttu-id="955b5-495">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="955b5-495">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-496">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-496">VM</span></span>
* <span data-ttu-id="955b5-497">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="955b5-497">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="955b5-498">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-498">October 9, 2018</span></span>

<span data-ttu-id="955b5-499">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="955b5-499">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="955b5-500">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-500">Core</span></span>
* <span data-ttu-id="955b5-501">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="955b5-501">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-502">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-502">ACR</span></span>
* <span data-ttu-id="955b5-503">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="955b5-503">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-504">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-504">ACS</span></span>
* <span data-ttu-id="955b5-505">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="955b5-505">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="955b5-506">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="955b5-506">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="955b5-507">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="955b5-507">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="955b5-508">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="955b5-508">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="955b5-509">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-509">Container</span></span>
* <span data-ttu-id="955b5-510">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="955b5-510">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="955b5-511">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="955b5-511">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="955b5-512">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="955b5-512">Event Hub</span></span>
* <span data-ttu-id="955b5-513">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-513">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="955b5-514">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="955b5-514">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="955b5-515">расширения.</span><span class="sxs-lookup"><span data-stu-id="955b5-515">Extensions</span></span>
* <span data-ttu-id="955b5-516">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="955b5-516">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="955b5-517">HDInsight</span><span class="sxs-lookup"><span data-stu-id="955b5-517">HDInsight</span></span>
* <span data-ttu-id="955b5-518">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="955b5-518">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="955b5-519">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="955b5-519">IoT</span></span>
* <span data-ttu-id="955b5-520">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="955b5-520">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="955b5-521">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="955b5-521">KeyVault</span></span>
* <span data-ttu-id="955b5-522">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="955b5-522">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="955b5-523">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-523">Network</span></span>
* <span data-ttu-id="955b5-524">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-524">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="955b5-525">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="955b5-525">See #6052</span></span>
* <span data-ttu-id="955b5-526">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-526">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="955b5-527">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="955b5-527">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="955b5-528">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="955b5-528">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="955b5-529">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="955b5-529">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="955b5-530">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="955b5-530">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="955b5-531">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-531">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="955b5-532">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-532">Role</span></span>
* <span data-ttu-id="955b5-533">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="955b5-533">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="955b5-534">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="955b5-534">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="955b5-535">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="955b5-535">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="955b5-536">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="955b5-536">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="955b5-537">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-537">Service Bus</span></span>
* <span data-ttu-id="955b5-538">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="955b5-538">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-539">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-539">VM</span></span>
* <span data-ttu-id="955b5-540">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="955b5-540">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="955b5-541">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="955b5-541">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="955b5-542">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="955b5-542">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="955b5-543">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="955b5-543">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="955b5-544">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="955b5-544">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="955b5-545">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="955b5-545">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="955b5-546">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-546">September 21, 2018</span></span>

<span data-ttu-id="955b5-547">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="955b5-547">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-548">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-548">ACR</span></span>
* <span data-ttu-id="955b5-549">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="955b5-549">Added ACR Task commands</span></span>
* <span data-ttu-id="955b5-550">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="955b5-550">Added quick run command</span></span>
* <span data-ttu-id="955b5-551">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="955b5-551">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="955b5-552">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="955b5-552">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="955b5-553">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="955b5-553">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="955b5-554">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="955b5-554">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-555">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-555">ACS</span></span>
* <span data-ttu-id="955b5-556">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="955b5-556">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="955b5-557">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="955b5-557">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-558">AppService</span><span class="sxs-lookup"><span data-stu-id="955b5-558">AppService</span></span>

* <span data-ttu-id="955b5-559">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="955b5-559">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="955b5-560">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="955b5-560">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="955b5-561">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="955b5-561">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="955b5-562">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="955b5-562">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="955b5-563">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-563">Batch</span></span>
* <span data-ttu-id="955b5-564">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="955b5-564">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="955b5-565">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="955b5-565">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="955b5-566">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-566">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="955b5-567">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="955b5-567">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="955b5-568">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="955b5-568">Batch AI</span></span> 
* <span data-ttu-id="955b5-569">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-569">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="955b5-570">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="955b5-570">Cognitive Services</span></span>
* <span data-ttu-id="955b5-571">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="955b5-571">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="955b5-572">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="955b5-572">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="955b5-573">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="955b5-573">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="955b5-574">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="955b5-574">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="955b5-575">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="955b5-575">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="955b5-576">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="955b5-576">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="955b5-577">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-577">Container</span></span>
* <span data-ttu-id="955b5-578">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-578">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="955b5-579">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="955b5-579">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="955b5-580">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="955b5-580">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="955b5-581">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-581">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="955b5-582">Data Lake</span><span class="sxs-lookup"><span data-stu-id="955b5-582">Datalake</span></span>
* <span data-ttu-id="955b5-583">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="955b5-583">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="955b5-584">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="955b5-584">Interactive Shell</span></span>
* <span data-ttu-id="955b5-585">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="955b5-585">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="955b5-586">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="955b5-586">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="955b5-587">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="955b5-587">IoT</span></span>
* <span data-ttu-id="955b5-588">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="955b5-588">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="955b5-589">Key Vault</span><span class="sxs-lookup"><span data-stu-id="955b5-589">Key Vault</span></span>
* <span data-ttu-id="955b5-590">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="955b5-590">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="955b5-591">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-591">Network</span></span>
* <span data-ttu-id="955b5-592">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="955b5-592">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="955b5-593">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-593">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="955b5-594">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="955b5-594">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="955b5-595">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="955b5-595">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="955b5-596">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-596">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="955b5-597">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-597">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="955b5-598">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="955b5-598">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="955b5-599">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="955b5-599">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="955b5-600">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="955b5-600">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="955b5-601">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="955b5-601">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="955b5-602">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="955b5-602">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="955b5-603">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="955b5-603">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="955b5-604">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="955b5-604">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="955b5-605">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="955b5-605">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="955b5-606">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="955b5-606">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="955b5-607">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="955b5-607">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="955b5-608">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="955b5-608">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="955b5-609">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="955b5-609">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="955b5-610">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="955b5-610">RDBMS</span></span>
* <span data-ttu-id="955b5-611">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="955b5-611">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="955b5-612">резервирование.</span><span class="sxs-lookup"><span data-stu-id="955b5-612">Reservation</span></span>
* <span data-ttu-id="955b5-613">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="955b5-613">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="955b5-614">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="955b5-614">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="955b5-615">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="955b5-615">Manage App</span></span>
* <span data-ttu-id="955b5-616">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="955b5-616">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="955b5-617">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="955b5-617">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="955b5-618">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-618">Role</span></span>
* <span data-ttu-id="955b5-619">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="955b5-619">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="955b5-620">SignalR</span><span class="sxs-lookup"><span data-stu-id="955b5-620">SignalR</span></span>
* <span data-ttu-id="955b5-621">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="955b5-621">First release</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-622">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-622">Storage</span></span>
* <span data-ttu-id="955b5-623">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="955b5-623">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="955b5-624">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="955b5-624">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-625">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-625">VM</span></span>
* <span data-ttu-id="955b5-626">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="955b5-626">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="955b5-627">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="955b5-627">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="955b5-628">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-628">August 28, 2018</span></span>

<span data-ttu-id="955b5-629">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="955b5-629">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="955b5-630">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-630">Core</span></span>

* <span data-ttu-id="955b5-631">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="955b5-631">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="955b5-632">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="955b5-632">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-633">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-633">ACR</span></span>

* <span data-ttu-id="955b5-634">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="955b5-634">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="955b5-635">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="955b5-635">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-636">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-636">ACS</span></span>

* <span data-ttu-id="955b5-637">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="955b5-637">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="955b5-638">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="955b5-638">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-639">AppService</span><span class="sxs-lookup"><span data-stu-id="955b5-639">AppService</span></span>

* <span data-ttu-id="955b5-640">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="955b5-640">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="955b5-641">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="955b5-641">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="955b5-642">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="955b5-642">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="955b5-643">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="955b5-643">Backup</span></span>

* <span data-ttu-id="955b5-644">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="955b5-644">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="955b5-645">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="955b5-645">Bot Service</span></span>

* <span data-ttu-id="955b5-646">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="955b5-646">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="955b5-647">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="955b5-647">Cognitive Services</span></span>

* <span data-ttu-id="955b5-648">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="955b5-648">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="955b5-649">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="955b5-649">IoT</span></span>

* <span data-ttu-id="955b5-650">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="955b5-650">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-651">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-651">Monitor</span></span>

* <span data-ttu-id="955b5-652">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="955b5-652">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="955b5-653">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="955b5-653">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="955b5-654">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-654">Network</span></span>

* <span data-ttu-id="955b5-655">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="955b5-655">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-656">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-656">Resource</span></span>

* <span data-ttu-id="955b5-657">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="955b5-657">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-658">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-658">Storage</span></span>

* <span data-ttu-id="955b5-659">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="955b5-659">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-660">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-660">VM</span></span>

* <span data-ttu-id="955b5-661">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="955b5-661">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="955b5-662">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-662">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="955b5-663">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-663">Auguest 14, 2018</span></span>

<span data-ttu-id="955b5-664">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="955b5-664">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="955b5-665">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-665">Core</span></span>

* <span data-ttu-id="955b5-666">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="955b5-666">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="955b5-667">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="955b5-667">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="955b5-668">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="955b5-668">Telemetry</span></span>

* <span data-ttu-id="955b5-669">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="955b5-669">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-670">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-670">ACR</span></span>

* <span data-ttu-id="955b5-671">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="955b5-671">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="955b5-672">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="955b5-672">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-673">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-673">ACS</span></span>

* <span data-ttu-id="955b5-674">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="955b5-674">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="955b5-675">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="955b5-675">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="955b5-676">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="955b5-676">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="955b5-677">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="955b5-677">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="955b5-678">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="955b5-678">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="955b5-679">AppService</span><span class="sxs-lookup"><span data-stu-id="955b5-679">AppService</span></span>

* <span data-ttu-id="955b5-680">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="955b5-680">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="955b5-681">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="955b5-681">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="955b5-682">Batch AI</span><span class="sxs-lookup"><span data-stu-id="955b5-682">BatchAI</span></span>

* <span data-ttu-id="955b5-683">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="955b5-683">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="955b5-684">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-684">Container</span></span>

* <span data-ttu-id="955b5-685">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="955b5-685">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="955b5-686">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="955b5-686">IoT</span></span>

* <span data-ttu-id="955b5-687">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="955b5-687">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="955b5-688">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="955b5-688">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="955b5-689">IoT Central</span><span class="sxs-lookup"><span data-stu-id="955b5-689">Iot Central</span></span>

* <span data-ttu-id="955b5-690">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="955b5-690">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="955b5-691">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="955b5-691">KeyVault</span></span>


* <span data-ttu-id="955b5-692">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="955b5-692">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="955b5-693">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="955b5-693">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="955b5-694">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="955b5-694">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="955b5-695">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="955b5-695">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="955b5-696">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="955b5-696">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="955b5-697">Передача</span><span class="sxs-lookup"><span data-stu-id="955b5-697">Relay</span></span>

* <span data-ttu-id="955b5-698">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="955b5-698">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-699">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-699">Sql</span></span>

* <span data-ttu-id="955b5-700">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="955b5-700">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-701">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-701">Storage</span></span>

* <span data-ttu-id="955b5-702">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="955b5-702">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="955b5-703">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="955b5-703">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="955b5-704">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="955b5-704">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="955b5-705">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="955b5-705">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="955b5-706">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="955b5-706">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-707">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-707">VM</span></span>

* <span data-ttu-id="955b5-708">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="955b5-708">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="955b5-709">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-709">July 31, 2018</span></span>

<span data-ttu-id="955b5-710">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="955b5-710">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-711">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-711">ACR</span></span>

* <span data-ttu-id="955b5-712">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="955b5-712">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="955b5-713">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="955b5-713">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-714">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-714">ACS</span></span>

* <span data-ttu-id="955b5-715">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="955b5-715">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="955b5-716">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-716">Batch</span></span>

* <span data-ttu-id="955b5-717">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="955b5-717">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="955b5-718">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-718">Container</span></span>

* <span data-ttu-id="955b5-719">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="955b5-719">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="955b5-720">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-720">Network</span></span>

* <span data-ttu-id="955b5-721">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="955b5-721">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="955b5-722">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-722">Resource</span></span>

* <span data-ttu-id="955b5-723">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="955b5-723">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="955b5-724">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="955b5-724">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="955b5-725">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-725">Role</span></span>

* <span data-ttu-id="955b5-726">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="955b5-726">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="955b5-727">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="955b5-727">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="955b5-728">поиска</span><span class="sxs-lookup"><span data-stu-id="955b5-728">Search</span></span>

* <span data-ttu-id="955b5-729">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="955b5-729">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="955b5-730">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-730">Service Bus</span></span>

* <span data-ttu-id="955b5-731">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="955b5-731">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="955b5-732">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="955b5-732">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="955b5-733">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="955b5-733">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="955b5-734">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="955b5-734">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-735">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-735">Storage</span></span>

* <span data-ttu-id="955b5-736">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="955b5-736">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="955b5-737">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="955b5-737">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-738">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-738">VM</span></span>

* <span data-ttu-id="955b5-739">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="955b5-739">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="955b5-740">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="955b5-740">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="955b5-741">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="955b5-741">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="955b5-742">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="955b5-742">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="955b5-743">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-743">July 18, 2018</span></span>

<span data-ttu-id="955b5-744">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="955b5-744">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="955b5-745">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-745">Core</span></span>

* <span data-ttu-id="955b5-746">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="955b5-746">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="955b5-747">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="955b5-747">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="955b5-748">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="955b5-748">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-749">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-749">ACR</span></span>

* <span data-ttu-id="955b5-750">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="955b5-750">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="955b5-751">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-751">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="955b5-752">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="955b5-752">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="955b5-753">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="955b5-753">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-754">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-754">ACS</span></span>

* <span data-ttu-id="955b5-755">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="955b5-755">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-756">AppService</span><span class="sxs-lookup"><span data-stu-id="955b5-756">AppService</span></span>

* <span data-ttu-id="955b5-757">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="955b5-757">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="955b5-758">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-758">Batch</span></span>

* <span data-ttu-id="955b5-759">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="955b5-759">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="955b5-760">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="955b5-760">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="955b5-761">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="955b5-761">Batch AI</span></span>

* <span data-ttu-id="955b5-762">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="955b5-762">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="955b5-763">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-763">Container</span></span>

* <span data-ttu-id="955b5-764">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="955b5-764">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="955b5-765">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="955b5-765">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="955b5-766">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-766">Network</span></span>

* <span data-ttu-id="955b5-767">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-767">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="955b5-768">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-768">Added `network nic wait`</span></span>
* <span data-ttu-id="955b5-769">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="955b5-769">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="955b5-770">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="955b5-770">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="955b5-771">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-771">Resource</span></span>

* <span data-ttu-id="955b5-772">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-772">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="955b5-773">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-773">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="955b5-774">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-774">Added `deployment wait` command</span></span>
* <span data-ttu-id="955b5-775">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="955b5-775">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-776">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-776">SQL</span></span>

* <span data-ttu-id="955b5-777">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-777">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="955b5-778">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="955b5-778">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="955b5-779">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="955b5-779">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-780">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-780">Storage</span></span>

* <span data-ttu-id="955b5-781">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="955b5-781">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-782">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-782">VM</span></span>

* <span data-ttu-id="955b5-783">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-783">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="955b5-784">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-784">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="955b5-785">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-785">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="955b5-786">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-786">July 3, 2018</span></span>

<span data-ttu-id="955b5-787">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="955b5-787">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="955b5-788">AKS</span><span class="sxs-lookup"><span data-stu-id="955b5-788">AKS</span></span>

* <span data-ttu-id="955b5-789">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="955b5-789">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="955b5-790">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-790">July 3, 2018</span></span>

<span data-ttu-id="955b5-791">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="955b5-791">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="955b5-792">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-792">Core</span></span>

* <span data-ttu-id="955b5-793">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="955b5-793">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-794">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-794">ACR</span></span>

* <span data-ttu-id="955b5-795">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="955b5-795">Added polling build status</span></span>
* <span data-ttu-id="955b5-796">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="955b5-796">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="955b5-797">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="955b5-797">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-798">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-798">ACS</span></span>

* <span data-ttu-id="955b5-799">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-799">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="955b5-800">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-800">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="955b5-801">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="955b5-801">Updated options for `aks browse` command.</span></span> <span data-ttu-id="955b5-802">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="955b5-802">Added `--listen-port` support</span></span>
* <span data-ttu-id="955b5-803">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="955b5-803">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="955b5-804">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="955b5-804">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="955b5-805">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="955b5-805">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-806">AppService</span><span class="sxs-lookup"><span data-stu-id="955b5-806">AppService</span></span>

* <span data-ttu-id="955b5-807">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="955b5-807">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="955b5-808">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="955b5-808">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="955b5-809">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="955b5-809">Backup</span></span>

* <span data-ttu-id="955b5-810">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="955b5-810">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="955b5-811">Batch AI</span><span class="sxs-lookup"><span data-stu-id="955b5-811">BatchAI</span></span>

* <span data-ttu-id="955b5-812">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="955b5-812">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="955b5-813">Облако</span><span class="sxs-lookup"><span data-stu-id="955b5-813">Cloud</span></span>

* <span data-ttu-id="955b5-814">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="955b5-814">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="955b5-815">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-815">Container</span></span>

* <span data-ttu-id="955b5-816">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="955b5-816">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="955b5-817">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="955b5-817">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="955b5-818">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="955b5-818">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="955b5-819">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="955b5-819">Extension</span></span>

* <span data-ttu-id="955b5-820">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="955b5-820">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="955b5-821">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-821">Network</span></span>

* <span data-ttu-id="955b5-822">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="955b5-822">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="955b5-823">Rdbms</span><span class="sxs-lookup"><span data-stu-id="955b5-823">Rdbms</span></span>

* <span data-ttu-id="955b5-824">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="955b5-824">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-825">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-825">Resource</span></span>

* <span data-ttu-id="955b5-826">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="955b5-826">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-827">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-827">VM</span></span>

* <span data-ttu-id="955b5-828">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="955b5-828">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="955b5-829">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-829">June 25, 2018</span></span>

<span data-ttu-id="955b5-830">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="955b5-830">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="955b5-831">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="955b5-831">CLI</span></span>

* <span data-ttu-id="955b5-832">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="955b5-832">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="955b5-833">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-833">June 19, 2018</span></span>

<span data-ttu-id="955b5-834">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="955b5-834">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="955b5-835">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-835">Core</span></span>

* <span data-ttu-id="955b5-836">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="955b5-836">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-837">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-837">ACR</span></span>

* <span data-ttu-id="955b5-838">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="955b5-838">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="955b5-839">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="955b5-839">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-840">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-840">ACS</span></span>

* <span data-ttu-id="955b5-841">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="955b5-841">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="955b5-842">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-842">Added `--update` support</span></span>
* <span data-ttu-id="955b5-843">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="955b5-843">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="955b5-844">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="955b5-844">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="955b5-845">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="955b5-845">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="955b5-846">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="955b5-846">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="955b5-847">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="955b5-847">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="955b5-848">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="955b5-848">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-849">AppService</span><span class="sxs-lookup"><span data-stu-id="955b5-849">AppService</span></span>

* <span data-ttu-id="955b5-850">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="955b5-850">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="955b5-851">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="955b5-851">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="955b5-852">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-852">Batch</span></span>

* <span data-ttu-id="955b5-853">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="955b5-853">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="955b5-854">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="955b5-854">Batch AI</span></span>

* <span data-ttu-id="955b5-855">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="955b5-855">Added support for workspaces.</span></span> <span data-ttu-id="955b5-856">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="955b5-856">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="955b5-857">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="955b5-857">Added support for experiments.</span></span> <span data-ttu-id="955b5-858">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="955b5-858">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="955b5-859">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="955b5-859">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="955b5-860">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="955b5-860">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="955b5-861">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="955b5-861">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="955b5-862">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="955b5-862">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="955b5-863">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="955b5-863">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="955b5-864">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="955b5-864">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="955b5-865">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-865">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="955b5-866">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="955b5-866">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="955b5-867">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-867">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="955b5-868">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="955b5-868">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="955b5-869">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="955b5-869">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="955b5-870">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="955b5-870">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="955b5-871">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-871">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="955b5-872">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="955b5-872">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="955b5-873">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="955b5-873">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="955b5-874">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="955b5-874">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="955b5-875">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="955b5-875">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="955b5-876">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="955b5-876">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="955b5-877">Карты</span><span class="sxs-lookup"><span data-stu-id="955b5-877">Maps</span></span>

* <span data-ttu-id="955b5-878">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="955b5-878">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="955b5-879">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-879">Network</span></span>

* <span data-ttu-id="955b5-880">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="955b5-880">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="955b5-881">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="955b5-881">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="955b5-882">#6502</span><span class="sxs-lookup"><span data-stu-id="955b5-882">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="955b5-883">Резервирование</span><span class="sxs-lookup"><span data-stu-id="955b5-883">Reservations</span></span>

* <span data-ttu-id="955b5-884">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-884">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="955b5-885">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-885">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="955b5-886">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="955b5-886">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="955b5-887">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="955b5-887">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="955b5-888">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="955b5-888">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="955b5-889">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-889">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="955b5-890">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-890">Role</span></span>

* <span data-ttu-id="955b5-891">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="955b5-891">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-892">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-892">SQL</span></span>

* <span data-ttu-id="955b5-893">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="955b5-893">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-894">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-894">Storage</span></span>

* <span data-ttu-id="955b5-895">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="955b5-895">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-896">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-896">VM</span></span>

* <span data-ttu-id="955b5-897">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-897">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="955b5-898">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="955b5-898">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="955b5-899">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="955b5-899">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="955b5-900">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-900">June 13, 2018</span></span>

<span data-ttu-id="955b5-901">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="955b5-901">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="955b5-902">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-902">Core</span></span>

* <span data-ttu-id="955b5-903">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="955b5-903">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="955b5-904">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-904">June 13, 2018</span></span>

<span data-ttu-id="955b5-905">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="955b5-905">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="955b5-906">AKS</span><span class="sxs-lookup"><span data-stu-id="955b5-906">AKS</span></span>

* <span data-ttu-id="955b5-907">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="955b5-907">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="955b5-908">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="955b5-908">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="955b5-909">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="955b5-909">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="955b5-910">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="955b5-910">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="955b5-911">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="955b5-911">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-912">AppService</span><span class="sxs-lookup"><span data-stu-id="955b5-912">AppService</span></span>

* <span data-ttu-id="955b5-913">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="955b5-913">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="955b5-914">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-914">June 5, 2018</span></span>

<span data-ttu-id="955b5-915">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="955b5-915">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-916">Interactive</span><span class="sxs-lookup"><span data-stu-id="955b5-916">Interactive</span></span>

* <span data-ttu-id="955b5-917">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="955b5-917">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="955b5-918">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-918">June 5, 2018</span></span>

<span data-ttu-id="955b5-919">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="955b5-919">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="955b5-920">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-920">Core</span></span>

* <span data-ttu-id="955b5-921">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="955b5-921">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="955b5-922">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="955b5-922">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-923">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-923">ACR</span></span>

* <span data-ttu-id="955b5-924">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="955b5-924">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="955b5-925">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="955b5-925">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="955b5-926">AKS</span><span class="sxs-lookup"><span data-stu-id="955b5-926">AKS</span></span>

* <span data-ttu-id="955b5-927">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="955b5-927">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="955b5-928">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-928">Batch</span></span>

* <span data-ttu-id="955b5-929">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="955b5-929">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="955b5-930">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="955b5-930">IOT</span></span>

* <span data-ttu-id="955b5-931">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="955b5-931">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="955b5-932">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-932">Network</span></span>

* <span data-ttu-id="955b5-933">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="955b5-933">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="955b5-934">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="955b5-934">Policy Insights</span></span>

* <span data-ttu-id="955b5-935">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="955b5-935">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="955b5-936">ARM</span><span class="sxs-lookup"><span data-stu-id="955b5-936">ARM</span></span>

* <span data-ttu-id="955b5-937">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="955b5-937">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-938">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-938">SQL</span></span>

* <span data-ttu-id="955b5-939">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="955b5-939">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="955b5-940">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="955b5-940">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="955b5-941">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-941">Storage</span></span>

* <span data-ttu-id="955b5-942">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="955b5-942">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-943">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-943">VM</span></span>

* <span data-ttu-id="955b5-944">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="955b5-944">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="955b5-945">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-945">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="955b5-946">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-946">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="955b5-947">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-947">May 22, 2018</span></span>

<span data-ttu-id="955b5-948">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="955b5-948">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="955b5-949">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-949">Core</span></span>

* <span data-ttu-id="955b5-950">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="955b5-950">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-951">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-951">ACS</span></span>

* <span data-ttu-id="955b5-952">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="955b5-952">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="955b5-953">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="955b5-953">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-954">AppService</span><span class="sxs-lookup"><span data-stu-id="955b5-954">AppService</span></span>

* <span data-ttu-id="955b5-955">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="955b5-955">Improved generic update commands</span></span>
* <span data-ttu-id="955b5-956">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="955b5-956">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="955b5-957">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-957">Container</span></span>

* <span data-ttu-id="955b5-958">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="955b5-958">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="955b5-959">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-959">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="955b5-960">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="955b5-960">Extension</span></span>

* <span data-ttu-id="955b5-961">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="955b5-961">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-962">Interactive</span><span class="sxs-lookup"><span data-stu-id="955b5-962">Interactive</span></span>

* <span data-ttu-id="955b5-963">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="955b5-963">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="955b5-964">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="955b5-964">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="955b5-965">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="955b5-965">KeyVault</span></span>

* <span data-ttu-id="955b5-966">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="955b5-966">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="955b5-967">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-967">Network</span></span>

* <span data-ttu-id="955b5-968">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="955b5-968">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="955b5-969">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="955b5-969">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-970">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-970">SQL</span></span>

* <span data-ttu-id="955b5-971">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="955b5-971">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="955b5-972">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="955b5-972">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="955b5-973">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="955b5-973">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="955b5-974">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="955b5-974">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="955b5-975">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="955b5-975">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="955b5-976">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="955b5-976">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="955b5-977">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="955b5-977">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="955b5-978">`edition`.</span><span class="sxs-lookup"><span data-stu-id="955b5-978">`edition`.</span></span> <span data-ttu-id="955b5-979">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="955b5-979">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="955b5-980">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="955b5-980">`elasticPoolName`.</span></span> <span data-ttu-id="955b5-981">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="955b5-981">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="955b5-982">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="955b5-982">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="955b5-983">`edition`.</span><span class="sxs-lookup"><span data-stu-id="955b5-983">`edition`.</span></span> <span data-ttu-id="955b5-984">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="955b5-984">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="955b5-985">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="955b5-985">`dtu`.</span></span> <span data-ttu-id="955b5-986">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="955b5-986">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="955b5-987">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="955b5-987">`databaseDtuMin`.</span></span> <span data-ttu-id="955b5-988">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="955b5-988">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="955b5-989">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="955b5-989">`databaseDtuMax`.</span></span> <span data-ttu-id="955b5-990">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="955b5-990">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="955b5-991">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="955b5-991">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="955b5-992">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="955b5-992">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-993">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-993">Storage</span></span>

* <span data-ttu-id="955b5-994">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="955b5-994">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="955b5-995">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="955b5-995">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-996">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-996">VM</span></span>

* <span data-ttu-id="955b5-997">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-997">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="955b5-998">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="955b5-998">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="955b5-999">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="955b5-999">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="955b5-1000">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="955b5-1000">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="955b5-1001">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1001">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="955b5-1002">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1002">May 7, 2018</span></span>

<span data-ttu-id="955b5-1003">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="955b5-1003">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="955b5-1004">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-1004">Core</span></span>

* <span data-ttu-id="955b5-1005">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="955b5-1005">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="955b5-1006">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1006">Added limited support for positional arguments</span></span>
* <span data-ttu-id="955b5-1007">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1007">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="955b5-1008">#5591</span><span class="sxs-lookup"><span data-stu-id="955b5-1008">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="955b5-1009">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1009">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="955b5-1010">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="955b5-1010">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="955b5-1011">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="955b5-1011">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="955b5-1012">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1012">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="955b5-1013">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="955b5-1013">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-1014">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-1014">ACR</span></span>

* <span data-ttu-id="955b5-1015">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="955b5-1015">Added ACR Build commands</span></span>
* <span data-ttu-id="955b5-1016">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="955b5-1016">Improved resource not found error messages</span></span>
* <span data-ttu-id="955b5-1017">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="955b5-1017">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="955b5-1018">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="955b5-1018">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="955b5-1019">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="955b5-1019">Improved repository commands error messages</span></span>
* <span data-ttu-id="955b5-1020">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="955b5-1020">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1021">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1021">ACS</span></span>

* <span data-ttu-id="955b5-1022">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-1022">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="955b5-1023">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="955b5-1023">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="955b5-1024">AMS</span><span class="sxs-lookup"><span data-stu-id="955b5-1024">AMS</span></span>

* <span data-ttu-id="955b5-1025">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="955b5-1025">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1026">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1026">Appservice</span></span>

* <span data-ttu-id="955b5-1027">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="955b5-1027">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="955b5-1028">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1028">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="955b5-1029">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="955b5-1029">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="955b5-1030">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1030">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="955b5-1031">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="955b5-1031">Batch AI</span></span>

* <span data-ttu-id="955b5-1032">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="955b5-1032">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="955b5-1033">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="955b5-1033">Cognitive Services</span></span>

* <span data-ttu-id="955b5-1034">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="955b5-1034">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="955b5-1035">Потребление</span><span class="sxs-lookup"><span data-stu-id="955b5-1035">Consumption</span></span>

* <span data-ttu-id="955b5-1036">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="955b5-1036">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="955b5-1037">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-1037">Container</span></span>

* <span data-ttu-id="955b5-1038">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="955b5-1038">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="955b5-1039">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="955b5-1039">Cosmos DB</span></span>

* <span data-ttu-id="955b5-1040">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="955b5-1040">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="955b5-1041">DMS</span><span class="sxs-lookup"><span data-stu-id="955b5-1041">DMS</span></span>

* <span data-ttu-id="955b5-1042">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="955b5-1042">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="955b5-1043">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="955b5-1043">Extension</span></span>

* <span data-ttu-id="955b5-1044">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="955b5-1044">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-1045">Interactive</span><span class="sxs-lookup"><span data-stu-id="955b5-1045">Interactive</span></span>

* <span data-ttu-id="955b5-1046">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="955b5-1046">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="955b5-1047">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="955b5-1047">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="955b5-1048">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="955b5-1048">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="955b5-1049">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="955b5-1049">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="955b5-1050">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="955b5-1050">Lab</span></span>

* <span data-ttu-id="955b5-1051">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="955b5-1051">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1052">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1052">Network</span></span>

* <span data-ttu-id="955b5-1053">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="955b5-1053">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="955b5-1054">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-1054">Profile</span></span>

* <span data-ttu-id="955b5-1055">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1055">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="955b5-1056">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="955b5-1056">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="955b5-1057">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1057">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="955b5-1058">Redis</span><span class="sxs-lookup"><span data-stu-id="955b5-1058">Redis</span></span>

* <span data-ttu-id="955b5-1059">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1059">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="955b5-1060">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="955b5-1060">Deprecated `redis list-all`.</span></span> <span data-ttu-id="955b5-1061">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1061">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="955b5-1062">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1062">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="955b5-1063">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="955b5-1063">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="955b5-1064">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-1064">Role</span></span>

* <span data-ttu-id="955b5-1065">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="955b5-1065">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1066">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1066">Storage</span></span>

* <span data-ttu-id="955b5-1067">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="955b5-1067">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="955b5-1068">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="955b5-1068">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="955b5-1069">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="955b5-1069">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="955b5-1070">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="955b5-1070">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="955b5-1071">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="955b5-1071">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1072">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1072">VM</span></span>

* <span data-ttu-id="955b5-1073">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="955b5-1073">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="955b5-1074">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="955b5-1074">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="955b5-1075">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="955b5-1075">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="955b5-1076">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1076">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="955b5-1077">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="955b5-1077">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="955b5-1078">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="955b5-1078">Added write accelerator support</span></span>
* <span data-ttu-id="955b5-1079">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1079">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="955b5-1080">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="955b5-1080">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="955b5-1081">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="955b5-1081">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="955b5-1082">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1082">April 10, 2018</span></span>

<span data-ttu-id="955b5-1083">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="955b5-1083">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-1084">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-1084">ACR</span></span>

* <span data-ttu-id="955b5-1085">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="955b5-1085">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1086">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1086">ACS</span></span>

* <span data-ttu-id="955b5-1087">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="955b5-1087">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1088">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1088">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="955b5-1090">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="955b5-1090">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="955b5-1091">Batch AI</span><span class="sxs-lookup"><span data-stu-id="955b5-1091">BatchAI</span></span>

* <span data-ttu-id="955b5-1092">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="955b5-1092">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="955b5-1093">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="955b5-1093">Job level mounting</span></span>
  - <span data-ttu-id="955b5-1094">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1094">Environment variables with secret values</span></span>
  - <span data-ttu-id="955b5-1095">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="955b5-1095">Performance counters settings</span></span>
  - <span data-ttu-id="955b5-1096">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="955b5-1096">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="955b5-1097">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1097">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="955b5-1098">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="955b5-1098">Usage and limits reporting</span></span>
  - <span data-ttu-id="955b5-1099">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1099">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="955b5-1100">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1100">Support for custom images</span></span>
  - <span data-ttu-id="955b5-1101">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="955b5-1101">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="955b5-1102">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="955b5-1102">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="955b5-1103">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1103">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="955b5-1104">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="955b5-1104">National clouds are supported</span></span>
* <span data-ttu-id="955b5-1105">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="955b5-1105">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="955b5-1106">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="955b5-1106">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="955b5-1107">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="955b5-1107">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="955b5-1108">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="955b5-1108">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="955b5-1109">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="955b5-1109">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="955b5-1110">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="955b5-1110">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="955b5-1111">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1111">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="955b5-1112">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="955b5-1112">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="955b5-1113">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="955b5-1113">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="955b5-1114">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1114">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="955b5-1115">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="955b5-1115">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="955b5-1116">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1116">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="955b5-1117">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1117">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="955b5-1118">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="955b5-1118">Billing</span></span>

* <span data-ttu-id="955b5-1119">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="955b5-1119">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="955b5-1120">Потребление</span><span class="sxs-lookup"><span data-stu-id="955b5-1120">Consumption</span></span>

* <span data-ttu-id="955b5-1121">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1121">Added `marketplace` commands</span></span>
* <span data-ttu-id="955b5-1122">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1122">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="955b5-1123">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1123">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="955b5-1124">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1124">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="955b5-1125">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1125">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="955b5-1126">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1126">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="955b5-1127">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-1127">Container</span></span>

* <span data-ttu-id="955b5-1128">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1128">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="955b5-1129">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="955b5-1129">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="955b5-1130">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="955b5-1130">Extension</span></span>

* <span data-ttu-id="955b5-1131">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="955b5-1131">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-1132">Interactive</span><span class="sxs-lookup"><span data-stu-id="955b5-1132">Interactive</span></span>

* <span data-ttu-id="955b5-1133">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="955b5-1133">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="955b5-1134">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="955b5-1134">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="955b5-1135">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1135">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1136">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1136">Network</span></span>

* <span data-ttu-id="955b5-1137">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1137">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="955b5-1138">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1138">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="955b5-1139">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="955b5-1139">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="955b5-1140">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="955b5-1140">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="955b5-1141">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="955b5-1141">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="955b5-1142">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1142">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="955b5-1143">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1143">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="955b5-1144">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="955b5-1144">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="955b5-1145">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-1145">Profile</span></span>

* <span data-ttu-id="955b5-1146">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1146">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="955b5-1147">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1147">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="955b5-1148">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="955b5-1148">RDBMS</span></span>

* <span data-ttu-id="955b5-1149">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1149">Added `georestore` command</span></span>
* <span data-ttu-id="955b5-1150">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="955b5-1150">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1151">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1151">Resource</span></span>

* <span data-ttu-id="955b5-1152">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1152">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="955b5-1153">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1153">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-1154">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-1154">SQL</span></span>

* <span data-ttu-id="955b5-1155">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1155">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1156">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1156">Storage</span></span>

* <span data-ttu-id="955b5-1157">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="955b5-1157">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1158">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1158">VM</span></span>

* <span data-ttu-id="955b5-1159">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="955b5-1159">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="955b5-1160">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="955b5-1160">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="955b5-1162">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1162">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="955b5-1163">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="955b5-1163">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="955b5-1164">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="955b5-1164">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="955b5-1165">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="955b5-1165">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="955b5-1166">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1166">March 27, 2018</span></span>

<span data-ttu-id="955b5-1167">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="955b5-1167">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="955b5-1168">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-1168">Core</span></span>

* <span data-ttu-id="955b5-1169">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="955b5-1169">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1170">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1170">ACS</span></span>

* <span data-ttu-id="955b5-1171">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="955b5-1171">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1172">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1172">Appservice</span></span>

* <span data-ttu-id="955b5-1173">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1173">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="955b5-1174">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1174">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="955b5-1175">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="955b5-1175">Backup</span></span>

* <span data-ttu-id="955b5-1176">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1176">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="955b5-1177">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="955b5-1177">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="955b5-1178">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="955b5-1178">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="955b5-1179">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1179">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="955b5-1180">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-1180">Container</span></span>

* <span data-ttu-id="955b5-1181">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1181">Added `container exec` command.</span></span> <span data-ttu-id="955b5-1182">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1182">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="955b5-1183">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1183">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="955b5-1184">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="955b5-1184">Extension</span></span>

* <span data-ttu-id="955b5-1185">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="955b5-1185">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="955b5-1186">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1186">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="955b5-1187">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-1187">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-1188">Interactive</span><span class="sxs-lookup"><span data-stu-id="955b5-1188">Interactive</span></span>

* <span data-ttu-id="955b5-1189">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="955b5-1189">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="955b5-1190">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1190">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="955b5-1191">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="955b5-1191">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="955b5-1192">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="955b5-1192">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="955b5-1193">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="955b5-1193">Lab</span></span>

* <span data-ttu-id="955b5-1194">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1194">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-1195">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-1195">Monitor</span></span>

* <span data-ttu-id="955b5-1196">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="955b5-1196">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="955b5-1197">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="955b5-1197">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="955b5-1198">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="955b5-1198">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1199">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1199">Network</span></span>

* <span data-ttu-id="955b5-1200">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="955b5-1200">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="955b5-1201">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-1201">Profile</span></span>

* <span data-ttu-id="955b5-1202">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1202">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="955b5-1203">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="955b5-1203">RDBMS</span></span>

* <span data-ttu-id="955b5-1204">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="955b5-1204">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1205">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1205">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="955b5-1207">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-1207">Role</span></span>

* <span data-ttu-id="955b5-1208">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1208">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="955b5-1209">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="955b5-1209">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="955b5-1210">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="955b5-1210">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="955b5-1211">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1211">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="955b5-1212">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1212">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1213">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1213">Storage</span></span>

* <span data-ttu-id="955b5-1214">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="955b5-1214">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="955b5-1215">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="955b5-1215">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1216">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1216">VM</span></span>

* <span data-ttu-id="955b5-1217">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1217">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="955b5-1218">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1218">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="955b5-1219">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="955b5-1219">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="955b5-1220">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="955b5-1220">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="955b5-1221">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1221">March 13, 2018</span></span>

<span data-ttu-id="955b5-1222">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="955b5-1222">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-1223">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-1223">ACR</span></span>

* <span data-ttu-id="955b5-1224">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1224">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="955b5-1225">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="955b5-1225">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="955b5-1226">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="955b5-1226">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1227">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1227">ACS</span></span>

* <span data-ttu-id="955b5-1228">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="955b5-1228">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="955b5-1229">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="955b5-1229">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="955b5-1230">Помощник</span><span class="sxs-lookup"><span data-stu-id="955b5-1230">Advisor</span></span>

* <span data-ttu-id="955b5-1231">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1231">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="955b5-1232">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1232">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="955b5-1233">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1233">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="955b5-1234">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1234">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="955b5-1235">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1235">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1236">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1236">Appservice</span></span>

* <span data-ttu-id="955b5-1237">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="955b5-1237">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="955b5-1238">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1238">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="955b5-1239">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="955b5-1239">Eventhubs</span></span>

* <span data-ttu-id="955b5-1240">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="955b5-1240">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="955b5-1241">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="955b5-1241">Extension</span></span>

* <span data-ttu-id="955b5-1242">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="955b5-1242">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-1243">Interactive</span><span class="sxs-lookup"><span data-stu-id="955b5-1243">Interactive</span></span>

* <span data-ttu-id="955b5-1244">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="955b5-1244">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="955b5-1245">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="955b5-1245">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="955b5-1246">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="955b5-1246">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="955b5-1247">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="955b5-1247">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-1248">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-1248">Monitor</span></span>

* <span data-ttu-id="955b5-1249">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="955b5-1249">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="955b5-1250">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1250">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="955b5-1251">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1251">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="955b5-1252">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1252">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1253">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1253">Network</span></span>

* <span data-ttu-id="955b5-1254">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1254">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="955b5-1255">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="955b5-1255">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="955b5-1256">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1256">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="955b5-1257">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1257">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="955b5-1258">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-1258">Profile</span></span>

* <span data-ttu-id="955b5-1259">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="955b5-1259">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="955b5-1260">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1260">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="955b5-1261">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="955b5-1261">RDBMS</span></span>

* <span data-ttu-id="955b5-1262">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="955b5-1262">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="955b5-1263">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-1263">Service Bus</span></span>

* <span data-ttu-id="955b5-1264">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="955b5-1264">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1265">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1265">Storage</span></span>

* <span data-ttu-id="955b5-1266">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="955b5-1266">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="955b5-1267">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="955b5-1267">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1268">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1268">VM</span></span>

* <span data-ttu-id="955b5-1269">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="955b5-1269">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="955b5-1270">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="955b5-1270">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="955b5-1271">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1271">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="955b5-1272">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="955b5-1272">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="955b5-1273">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="955b5-1273">February 27, 2018</span></span>

<span data-ttu-id="955b5-1274">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="955b5-1274">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="955b5-1275">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-1275">Core</span></span>

* <span data-ttu-id="955b5-1276">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="955b5-1276">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="955b5-1277">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="955b5-1277">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="955b5-1278">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1278">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1279">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1279">ACS</span></span>

* <span data-ttu-id="955b5-1280">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-1280">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="955b5-1281">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="955b5-1281">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="955b5-1282">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1282">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="955b5-1283">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1283">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1284">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1284">Appservice</span></span>

* <span data-ttu-id="955b5-1285">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="955b5-1285">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="955b5-1286">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="955b5-1286">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="955b5-1287">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="955b5-1287">Cognitive Services</span></span>

* <span data-ttu-id="955b5-1288">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="955b5-1288">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="955b5-1289">Потребление</span><span class="sxs-lookup"><span data-stu-id="955b5-1289">Consumption</span></span>

* <span data-ttu-id="955b5-1290">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="955b5-1290">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="955b5-1291">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="955b5-1291">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="955b5-1292">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-1292">Container</span></span>

* <span data-ttu-id="955b5-1293">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="955b5-1293">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1294">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1294">Network</span></span>

* <span data-ttu-id="955b5-1295">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1295">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1296">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1296">Resource</span></span>

* <span data-ttu-id="955b5-1297">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="955b5-1297">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="955b5-1298">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-1298">Role</span></span>

* <span data-ttu-id="955b5-1299">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-1299">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-1300">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-1300">SQL</span></span>

* <span data-ttu-id="955b5-1301">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1301">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1302">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1302">Storage</span></span>

* <span data-ttu-id="955b5-1303">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1303">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1304">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1304">VM</span></span>

* <span data-ttu-id="955b5-1305">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="955b5-1305">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="955b5-1306">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1306">February 13, 2018</span></span>

<span data-ttu-id="955b5-1307">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="955b5-1307">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="955b5-1308">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-1308">Core</span></span>

* <span data-ttu-id="955b5-1309">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="955b5-1309">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1310">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1310">ACS</span></span>

* <span data-ttu-id="955b5-1311">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="955b5-1311">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="955b5-1312">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1312">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="955b5-1313">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="955b5-1313">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="955b5-1314">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="955b5-1314">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="955b5-1315">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="955b5-1315">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="955b5-1316">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1316">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="955b5-1317">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="955b5-1317">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="955b5-1318">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1318">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1319">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1319">Appservice</span></span>

* <span data-ttu-id="955b5-1320">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="955b5-1320">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="955b5-1321">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1321">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="955b5-1322">CDN</span><span class="sxs-lookup"><span data-stu-id="955b5-1322">CDN</span></span>

* <span data-ttu-id="955b5-1323">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1323">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="955b5-1324">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-1324">Container</span></span>

* <span data-ttu-id="955b5-1325">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="955b5-1325">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="955b5-1326">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1326">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="955b5-1327">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="955b5-1327">CosmosDB</span></span>

* <span data-ttu-id="955b5-1328">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1328">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="955b5-1329">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="955b5-1329">Extension</span></span>

* <span data-ttu-id="955b5-1330">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1330">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="955b5-1331">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1331">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="955b5-1332">Отзыв</span><span class="sxs-lookup"><span data-stu-id="955b5-1332">Feedback</span></span>

* <span data-ttu-id="955b5-1333">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="955b5-1333">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-1334">Interactive</span><span class="sxs-lookup"><span data-stu-id="955b5-1334">Interactive</span></span>

* <span data-ttu-id="955b5-1335">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="955b5-1335">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="955b5-1336">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1336">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="955b5-1337">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="955b5-1337">IoT</span></span>

* <span data-ttu-id="955b5-1338">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="955b5-1338">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="955b5-1339">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="955b5-1339">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="955b5-1340">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1340">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="955b5-1341">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="955b5-1341">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-1342">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-1342">Monitor</span></span>

* <span data-ttu-id="955b5-1343">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1343">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1344">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1344">Network</span></span>

* <span data-ttu-id="955b5-1345">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="955b5-1345">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="955b5-1346">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-1346">Profile</span></span>

* <span data-ttu-id="955b5-1347">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="955b5-1347">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1348">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1348">Resource</span></span>

* <span data-ttu-id="955b5-1349">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1349">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="955b5-1350">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-1350">Role</span></span>

* <span data-ttu-id="955b5-1351">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="955b5-1351">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-1352">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-1352">SQL</span></span>

* <span data-ttu-id="955b5-1353">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1353">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="955b5-1354">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1354">Added `sql db rename`</span></span>
* <span data-ttu-id="955b5-1355">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="955b5-1355">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1356">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1356">Storage</span></span>

* <span data-ttu-id="955b5-1357">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="955b5-1357">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1358">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1358">VM</span></span>

* <span data-ttu-id="955b5-1359">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="955b5-1359">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="955b5-1360">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="955b5-1360">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="955b5-1361">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="955b5-1361">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="955b5-1362">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1362">January 31, 2018</span></span>

<span data-ttu-id="955b5-1363">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="955b5-1363">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="955b5-1364">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-1364">Core</span></span>

* <span data-ttu-id="955b5-1365">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="955b5-1365">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="955b5-1366">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="955b5-1366">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="955b5-1367">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="955b5-1367">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="955b5-1368">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="955b5-1368">Use `--verbose` to see</span></span>
* <span data-ttu-id="955b5-1369">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="955b5-1369">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1370">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1370">ACS</span></span>

* <span data-ttu-id="955b5-1371">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1371">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="955b5-1372">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1372">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1373">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1373">Appservice</span></span>

* <span data-ttu-id="955b5-1374">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="955b5-1374">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="955b5-1375">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="955b5-1375">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="955b5-1376">CDN</span><span class="sxs-lookup"><span data-stu-id="955b5-1376">CDN</span></span>

* <span data-ttu-id="955b5-1377">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1377">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="955b5-1378">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="955b5-1378">CosmosDB</span></span>

* <span data-ttu-id="955b5-1379">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="955b5-1379">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-1380">Interactive</span><span class="sxs-lookup"><span data-stu-id="955b5-1380">Interactive</span></span>

* <span data-ttu-id="955b5-1381">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="955b5-1381">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1382">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1382">Network</span></span>

* <span data-ttu-id="955b5-1383">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1383">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="955b5-1384">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-1384">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="955b5-1385">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1385">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="955b5-1386">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1386">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="955b5-1387">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1387">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="955b5-1388">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="955b5-1388">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="955b5-1389">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="955b5-1389">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="955b5-1390">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="955b5-1390">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="955b5-1391">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1391">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="955b5-1392">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1392">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="955b5-1393">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-1393">Profile</span></span>

* <span data-ttu-id="955b5-1394">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="955b5-1394">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1395">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1395">Resource</span></span>

* <span data-ttu-id="955b5-1396">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="955b5-1396">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1397">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1397">Storage</span></span>

* <span data-ttu-id="955b5-1398">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="955b5-1398">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="955b5-1399">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="955b5-1399">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="955b5-1400">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1400">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="955b5-1401">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1401">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="955b5-1402">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="955b5-1402">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1403">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1403">VM</span></span>

* <span data-ttu-id="955b5-1404">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="955b5-1404">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="955b5-1405">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1405">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="955b5-1406">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="955b5-1406">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="955b5-1407">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1407">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="955b5-1408">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1408">January 17, 2018</span></span>

<span data-ttu-id="955b5-1409">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="955b5-1409">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-1410">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-1410">ACR</span></span>

* <span data-ttu-id="955b5-1411">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="955b5-1411">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="955b5-1412">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="955b5-1412">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1413">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1413">ACS</span></span>

* <span data-ttu-id="955b5-1414">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1414">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="955b5-1415">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-1415">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1416">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1416">Appservice</span></span>

* <span data-ttu-id="955b5-1417">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="955b5-1417">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="955b5-1418">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1418">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="955b5-1419">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1419">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="955b5-1420">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="955b5-1420">Backup</span></span>

* <span data-ttu-id="955b5-1421">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="955b5-1421">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="955b5-1422">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="955b5-1422">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="955b5-1423">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="955b5-1423">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="955b5-1424">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="955b5-1424">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="955b5-1425">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="955b5-1425">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="955b5-1426">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-1426">Batch</span></span>

* <span data-ttu-id="955b5-1427">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="955b5-1427">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="955b5-1428">Облако</span><span class="sxs-lookup"><span data-stu-id="955b5-1428">Cloud</span></span>

* <span data-ttu-id="955b5-1429">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="955b5-1429">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="955b5-1430">Потребление</span><span class="sxs-lookup"><span data-stu-id="955b5-1430">Consumption</span></span>

* <span data-ttu-id="955b5-1431">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1431">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="955b5-1432">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-1432">Event Grid</span></span>

* <span data-ttu-id="955b5-1433">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1433">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="955b5-1434">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1434">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="955b5-1435">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1435">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="955b5-1436">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1436">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="955b5-1437">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1437">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="955b5-1438">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1438">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="955b5-1439">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1439">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="955b5-1440">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1440">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-1441">Interactive</span><span class="sxs-lookup"><span data-stu-id="955b5-1441">Interactive</span></span>

* <span data-ttu-id="955b5-1442">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="955b5-1442">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="955b5-1443">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="955b5-1443">Fixed errors on startup</span></span>
* <span data-ttu-id="955b5-1444">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="955b5-1444">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="955b5-1445">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="955b5-1445">IoT</span></span>

* <span data-ttu-id="955b5-1446">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="955b5-1446">Added support for device provisioning service</span></span>
* <span data-ttu-id="955b5-1447">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="955b5-1447">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="955b5-1448">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="955b5-1448">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-1449">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-1449">Monitor</span></span>

* <span data-ttu-id="955b5-1450">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="955b5-1450">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="955b5-1451">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1451">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="955b5-1452">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="955b5-1452">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1453">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1453">Network</span></span>

* <span data-ttu-id="955b5-1454">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="955b5-1454">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="955b5-1455">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="955b5-1455">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="955b5-1456">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-1456">Profile</span></span>

* <span data-ttu-id="955b5-1457">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="955b5-1457">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="955b5-1458">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-1458">Role</span></span>

* <span data-ttu-id="955b5-1459">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1459">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="955b5-1460">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="955b5-1460">Service Fabric</span></span>

* <span data-ttu-id="955b5-1461">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="955b5-1461">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="955b5-1462">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="955b5-1462">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1463">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1463">VM</span></span>

* <span data-ttu-id="955b5-1464">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1464">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="955b5-1465">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="955b5-1465">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="955b5-1466">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1466">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="955b5-1467">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="955b5-1467">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="955b5-1468">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="955b5-1468">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="955b5-1469">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1469">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="955b5-1470">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1470">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="955b5-1471">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1471">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="955b5-1472">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1472">December 19, 2017</span></span>

<span data-ttu-id="955b5-1473">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="955b5-1473">Version 2.0.23</span></span>

* <span data-ttu-id="955b5-1474">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="955b5-1474">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="955b5-1475">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-1475">Container</span></span>

* <span data-ttu-id="955b5-1476">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1476">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1477">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1477">Network</span></span>

* <span data-ttu-id="955b5-1478">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="955b5-1478">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="955b5-1479">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="955b5-1479">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1480">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1480">Storage</span></span>

* <span data-ttu-id="955b5-1481">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="955b5-1481">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1482">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1482">VM</span></span>

* <span data-ttu-id="955b5-1483">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="955b5-1483">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="955b5-1484">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1484">December 5, 2017</span></span>

<span data-ttu-id="955b5-1485">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="955b5-1485">Version 2.0.22</span></span>

* <span data-ttu-id="955b5-1486">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1486">Removed `az component` commands.</span></span> <span data-ttu-id="955b5-1487">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1487">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="955b5-1488">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-1488">Core</span></span>
* <span data-ttu-id="955b5-1489">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="955b5-1489">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="955b5-1490">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="955b5-1490">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1491">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1491">ACS</span></span>

* <span data-ttu-id="955b5-1492">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1492">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="955b5-1493">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1493">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="955b5-1494">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="955b5-1494">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="955b5-1495">Помощник</span><span class="sxs-lookup"><span data-stu-id="955b5-1495">Advisor</span></span>

* <span data-ttu-id="955b5-1496">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="955b5-1496">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1497">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1497">Appservice</span></span>

* <span data-ttu-id="955b5-1498">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1498">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="955b5-1499">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="955b5-1499">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="955b5-1500">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1500">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="955b5-1501">Потребление</span><span class="sxs-lookup"><span data-stu-id="955b5-1501">Consumption</span></span>

* <span data-ttu-id="955b5-1502">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="955b5-1502">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="955b5-1503">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-1503">Container</span></span>

* <span data-ttu-id="955b5-1504">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="955b5-1504">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-1505">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-1505">Monitor</span></span>

* <span data-ttu-id="955b5-1506">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="955b5-1506">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1507">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1507">Resource</span></span>

* <span data-ttu-id="955b5-1508">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="955b5-1508">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="955b5-1509">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-1509">Role</span></span>

* <span data-ttu-id="955b5-1510">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1510">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="955b5-1511">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="955b5-1511">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="955b5-1512">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1512">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-1513">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-1513">SQL</span></span>

* <span data-ttu-id="955b5-1514">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1514">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="955b5-1515">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1515">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1516">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1516">VM</span></span>

* <span data-ttu-id="955b5-1517">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1517">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="955b5-1518">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1518">November 14, 2017</span></span>

<span data-ttu-id="955b5-1519">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="955b5-1519">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-1520">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-1520">ACR</span></span>

* <span data-ttu-id="955b5-1521">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="955b5-1521">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="955b5-1522">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1522">ACS</span></span>

* <span data-ttu-id="955b5-1523">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="955b5-1523">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="955b5-1524">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="955b5-1524">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="955b5-1525">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1525">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="955b5-1526">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="955b5-1526">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="955b5-1527">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="955b5-1527">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1528">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1528">Appservice</span></span>

* <span data-ttu-id="955b5-1529">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="955b5-1529">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="955b5-1530">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1530">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="955b5-1531">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1531">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="955b5-1532">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1532">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="955b5-1533">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="955b5-1533">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="955b5-1534">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="955b5-1534">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="955b5-1535">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-1535">Batch</span></span>

* <span data-ttu-id="955b5-1536">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1536">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="955b5-1537">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="955b5-1537">Batchai</span></span>

* <span data-ttu-id="955b5-1538">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1538">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="955b5-1539">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1539">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="955b5-1540">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1540">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="955b5-1541">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1541">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="955b5-1542">Облако</span><span class="sxs-lookup"><span data-stu-id="955b5-1542">Cloud</span></span>

* <span data-ttu-id="955b5-1543">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="955b5-1543">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="955b5-1544">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-1544">Container</span></span>

* <span data-ttu-id="955b5-1545">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1545">Added support to open multiple ports</span></span>
* <span data-ttu-id="955b5-1546">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1546">Added container group restart policy</span></span>
* <span data-ttu-id="955b5-1547">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="955b5-1547">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="955b5-1548">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="955b5-1548">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="955b5-1549">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="955b5-1549">Data Lake Analytics</span></span>

* <span data-ttu-id="955b5-1550">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="955b5-1550">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="955b5-1551">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="955b5-1551">Data Lake Store</span></span>

* <span data-ttu-id="955b5-1552">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="955b5-1552">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="955b5-1553">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="955b5-1553">Extension</span></span>

* <span data-ttu-id="955b5-1554">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="955b5-1554">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="955b5-1555">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="955b5-1555">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="955b5-1556">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="955b5-1556">IoT</span></span>

* <span data-ttu-id="955b5-1557">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1557">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-1558">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-1558">Monitor</span></span>

* <span data-ttu-id="955b5-1559">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1559">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1560">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1560">Network</span></span>

* <span data-ttu-id="955b5-1561">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="955b5-1561">Added support for CAA DNS records</span></span>
* <span data-ttu-id="955b5-1562">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1562">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="955b5-1563">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="955b5-1563">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="955b5-1564">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1564">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="955b5-1565">Резервирование</span><span class="sxs-lookup"><span data-stu-id="955b5-1565">Reservations</span></span>

* <span data-ttu-id="955b5-1566">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="955b5-1566">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1567">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1567">Resource</span></span>

* <span data-ttu-id="955b5-1568">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1568">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-1569">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-1569">SQL</span></span>

* <span data-ttu-id="955b5-1570">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1570">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1571">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1571">Storage</span></span>

* <span data-ttu-id="955b5-1572">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-1572">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="955b5-1573">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="955b5-1573">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="955b5-1574">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1574">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="955b5-1575">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1575">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="955b5-1576">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1576">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="955b5-1577">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1577">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="955b5-1578">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1578">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1579">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1579">VM</span></span>

* <span data-ttu-id="955b5-1580">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1580">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="955b5-1581">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1581">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="955b5-1582">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1582">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="955b5-1583">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1583">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="955b5-1584">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="955b5-1584">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="955b5-1585">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1585">October 24, 2017</span></span>

<span data-ttu-id="955b5-1586">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="955b5-1586">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="955b5-1587">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-1587">Core</span></span>

* <span data-ttu-id="955b5-1588">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="955b5-1588">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-1589">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-1589">ACR</span></span>

* <span data-ttu-id="955b5-1590">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="955b5-1590">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="955b5-1591">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="955b5-1591">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="955b5-1592">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="955b5-1592">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1593">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1593">ACS</span></span>

* <span data-ttu-id="955b5-1594">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="955b5-1594">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="955b5-1595">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="955b5-1595">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1596">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1596">Appservice</span></span>

* <span data-ttu-id="955b5-1597">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="955b5-1597">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="955b5-1598">Компонент</span><span class="sxs-lookup"><span data-stu-id="955b5-1598">Component</span></span>

* <span data-ttu-id="955b5-1599">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="955b5-1599">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-1600">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-1600">Monitor</span></span>

* <span data-ttu-id="955b5-1601">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1601">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1602">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1602">Resource</span></span>

* <span data-ttu-id="955b5-1603">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="955b5-1603">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="955b5-1604">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="955b5-1604">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1605">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1605">VM</span></span>

* <span data-ttu-id="955b5-1606">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="955b5-1606">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="955b5-1607">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1607">October 9, 2017</span></span>

<span data-ttu-id="955b5-1608">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="955b5-1608">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="955b5-1609">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-1609">Core</span></span>

* <span data-ttu-id="955b5-1610">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="955b5-1610">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1611">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1611">Appservice</span></span>

* <span data-ttu-id="955b5-1612">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1612">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="955b5-1613">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-1613">Batch</span></span>

* <span data-ttu-id="955b5-1614">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="955b5-1614">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="955b5-1615">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="955b5-1615">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="955b5-1616">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-1616">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="955b5-1617">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1617">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="955b5-1618">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="955b5-1618">Batchai</span></span>

* <span data-ttu-id="955b5-1619">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="955b5-1619">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="955b5-1620">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="955b5-1620">Keyvault</span></span>

* <span data-ttu-id="955b5-1621">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="955b5-1621">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="955b5-1622">(#4448)</span><span class="sxs-lookup"><span data-stu-id="955b5-1622">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="955b5-1623">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1623">Network</span></span>

* <span data-ttu-id="955b5-1624">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="955b5-1624">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="955b5-1625">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="955b5-1625">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1626">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1626">Resource</span></span>

* <span data-ttu-id="955b5-1627">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1627">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="955b5-1628">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="955b5-1628">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="955b5-1629">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="955b5-1629">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="955b5-1630">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="955b5-1630">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-1631">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-1631">Sql</span></span>

* <span data-ttu-id="955b5-1632">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="955b5-1632">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="955b5-1633">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="955b5-1633">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="955b5-1634">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="955b5-1634">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1635">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1635">Storage</span></span>

* <span data-ttu-id="955b5-1636">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1636">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1637">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="955b5-1637">Vm</span></span>

* <span data-ttu-id="955b5-1638">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1638">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="955b5-1639">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1639">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="955b5-1640">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1640">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="955b5-1641">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1641">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="955b5-1642">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="955b5-1642">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="955b5-1643">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1643">September 22, 2017</span></span>

<span data-ttu-id="955b5-1644">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="955b5-1644">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1645">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1645">Resource</span></span>

* <span data-ttu-id="955b5-1646">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="955b5-1646">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="955b5-1647">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="955b5-1647">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="955b5-1648">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="955b5-1648">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="955b5-1649">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1649">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1650">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1650">Network</span></span>

* <span data-ttu-id="955b5-1651">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="955b5-1651">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="955b5-1652">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="955b5-1652">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="955b5-1653">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="955b5-1653">Added `asg` application security group commands</span></span>
* <span data-ttu-id="955b5-1654">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="955b5-1654">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="955b5-1655">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="955b5-1655">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="955b5-1656">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="955b5-1656">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="955b5-1657">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1657">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1658">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1658">Storage</span></span>

* <span data-ttu-id="955b5-1659">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="955b5-1659">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="955b5-1660">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="955b5-1660">Eventgrid</span></span>

* <span data-ttu-id="955b5-1661">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="955b5-1661">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-1662">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-1662">SQL</span></span>

* <span data-ttu-id="955b5-1663">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="955b5-1663">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="955b5-1664">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="955b5-1664">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="955b5-1665">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="955b5-1665">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="955b5-1666">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="955b5-1666">Keyvault</span></span>

* <span data-ttu-id="955b5-1667">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="955b5-1667">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1668">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1668">VM</span></span>

* <span data-ttu-id="955b5-1669">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="955b5-1669">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="955b5-1670">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="955b5-1670">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="955b5-1671">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="955b5-1671">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="955b5-1672">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="955b5-1672">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="955b5-1673">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="955b5-1673">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="955b5-1674">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="955b5-1674">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1675">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1675">ACS</span></span>

* <span data-ttu-id="955b5-1676">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="955b5-1676">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1677">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1677">Appservice</span></span>

* <span data-ttu-id="955b5-1678">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="955b5-1678">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="955b5-1679">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="955b5-1679">Backup</span></span>

* <span data-ttu-id="955b5-1680">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="955b5-1680">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="955b5-1681">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1681">September 11, 2017</span></span>

<span data-ttu-id="955b5-1682">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="955b5-1682">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="955b5-1683">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-1683">Core</span></span>

* <span data-ttu-id="955b5-1684">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="955b5-1684">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="955b5-1685">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="955b5-1685">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1686">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1686">Acs</span></span>

* <span data-ttu-id="955b5-1687">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1687">Added `acs list-locations` command</span></span>
* <span data-ttu-id="955b5-1688">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-1688">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1689">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1689">Appservice</span></span>

* <span data-ttu-id="955b5-1690">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="955b5-1690">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="955b5-1691">CDN</span><span class="sxs-lookup"><span data-stu-id="955b5-1691">CDN</span></span>

* <span data-ttu-id="955b5-1692">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1692">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="955b5-1693">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="955b5-1693">Extension</span></span>

* <span data-ttu-id="955b5-1694">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="955b5-1694">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="955b5-1695">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="955b5-1695">Keyvault</span></span>

* <span data-ttu-id="955b5-1696">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1696">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1697">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1697">Network</span></span>

* <span data-ttu-id="955b5-1698">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1698">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="955b5-1699">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1699">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="955b5-1700">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1700">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="955b5-1701">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1701">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="955b5-1702">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1702">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1703">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1703">Resource</span></span>

* <span data-ttu-id="955b5-1704">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1704">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="955b5-1705">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1705">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="955b5-1706">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1706">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="955b5-1707">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="955b5-1707">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-1708">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-1708">SQL</span></span>

* <span data-ttu-id="955b5-1709">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1709">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1710">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1710">VM</span></span>

* <span data-ttu-id="955b5-1711">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="955b5-1711">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="955b5-1712">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="955b5-1712">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="955b5-1713">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1713">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="955b5-1714">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="955b5-1714">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="955b5-1715">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="955b5-1715">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="955b5-1716">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1716">August 31, 2017</span></span>

<span data-ttu-id="955b5-1717">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="955b5-1717">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="955b5-1718">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="955b5-1718">Keyvault</span></span>

* <span data-ttu-id="955b5-1719">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1719">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="955b5-1720">Sf</span><span class="sxs-lookup"><span data-stu-id="955b5-1720">Sf</span></span>

* <span data-ttu-id="955b5-1721">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="955b5-1721">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1722">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1722">Storage</span></span>

* <span data-ttu-id="955b5-1723">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="955b5-1723">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="955b5-1724">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="955b5-1724">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="955b5-1725">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1725">August 28, 2017</span></span>

<span data-ttu-id="955b5-1726">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="955b5-1726">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="955b5-1727">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="955b5-1727">CLI</span></span>

* <span data-ttu-id="955b5-1728">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="955b5-1728">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1729">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1729">ACS</span></span>

* <span data-ttu-id="955b5-1730">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="955b5-1730">Corrected preview regions</span></span>
* <span data-ttu-id="955b5-1731">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1731">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="955b5-1732">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="955b5-1732">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1733">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1733">Appservice</span></span>

* <span data-ttu-id="955b5-1734">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1734">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="955b5-1735">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1735">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="955b5-1736">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1736">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="955b5-1737">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="955b5-1737">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="955b5-1738">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="955b5-1738">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="955b5-1739">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="955b5-1739">IoT</span></span>

* <span data-ttu-id="955b5-1740">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="955b5-1740">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1741">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1741">Network</span></span>

* <span data-ttu-id="955b5-1742">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1742">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="955b5-1743">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1743">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="955b5-1744">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1744">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="955b5-1745">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1745">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="955b5-1746">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1746">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="955b5-1747">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-1747">Profile</span></span>

* <span data-ttu-id="955b5-1748">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="955b5-1748">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="955b5-1749">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="955b5-1749">Service Fabric</span></span>

* <span data-ttu-id="955b5-1750">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="955b5-1750">Preview release</span></span>
* <span data-ttu-id="955b5-1751">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="955b5-1751">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="955b5-1752">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="955b5-1752">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="955b5-1753">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1753">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1754">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1754">Storage</span></span>

* <span data-ttu-id="955b5-1755">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="955b5-1755">Enabled setting blob tier</span></span>
* <span data-ttu-id="955b5-1756">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-1756">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="955b5-1757">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1757">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="955b5-1758">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="955b5-1758">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="955b5-1759">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1759">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="955b5-1760">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1760">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1761">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1761">VM</span></span>

* <span data-ttu-id="955b5-1762">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1762">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="955b5-1763">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1763">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="955b5-1764">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="955b5-1764">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="955b5-1765">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="955b5-1765">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="955b5-1766">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="955b5-1766">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="955b5-1767">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1767">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="955b5-1768">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1768">August 15, 2017</span></span>

<span data-ttu-id="955b5-1769">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="955b5-1769">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1770">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1770">ACS</span></span>

* <span data-ttu-id="955b5-1771">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="955b5-1771">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1772">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1772">Appservice</span></span>

* <span data-ttu-id="955b5-1773">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="955b5-1773">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="955b5-1774">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-1774">Event Grid</span></span>

* <span data-ttu-id="955b5-1775">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="955b5-1775">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="955b5-1776">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1776">August 11, 2017</span></span>

<span data-ttu-id="955b5-1777">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="955b5-1777">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1778">ACS</span></span>

* <span data-ttu-id="955b5-1779">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="955b5-1779">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="955b5-1780">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-1780">Batch</span></span>

* <span data-ttu-id="955b5-1781">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="955b5-1781">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="955b5-1782">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="955b5-1782">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="955b5-1783">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1783">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="955b5-1784">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="955b5-1784">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="955b5-1785">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="955b5-1785">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="955b5-1786">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="955b5-1786">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="955b5-1787">Компонент</span><span class="sxs-lookup"><span data-stu-id="955b5-1787">Component</span></span>

* <span data-ttu-id="955b5-1788">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="955b5-1788">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="955b5-1789">Контейнер</span><span class="sxs-lookup"><span data-stu-id="955b5-1789">Container</span></span>

* <span data-ttu-id="955b5-1790">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="955b5-1790">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="955b5-1791">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="955b5-1791">Data Lake Store</span></span>

* <span data-ttu-id="955b5-1792">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="955b5-1792">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="955b5-1793">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-1793">Event Grid</span></span>

* <span data-ttu-id="955b5-1794">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="955b5-1794">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1795">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1795">Network</span></span>

* <span data-ttu-id="955b5-1796">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="955b5-1796">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="955b5-1797">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1797">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="955b5-1798">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1798">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="955b5-1799">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1799">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="955b5-1800">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-1800">Profile</span></span>

* <span data-ttu-id="955b5-1801">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="955b5-1801">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1802">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1802">Storage</span></span>

* <span data-ttu-id="955b5-1803">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="955b5-1803">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1804">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1804">VM</span></span>

* <span data-ttu-id="955b5-1805">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="955b5-1805">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="955b5-1806">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1806">Exposed `list-skus` command</span></span>
* <span data-ttu-id="955b5-1807">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="955b5-1807">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="955b5-1808">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="955b5-1808">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="955b5-1809">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="955b5-1809">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="955b5-1810">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1810">July 28, 2017</span></span>

<span data-ttu-id="955b5-1811">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="955b5-1811">Version 2.0.12</span></span>

* <span data-ttu-id="955b5-1812">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1812">Added container commands</span></span>
* <span data-ttu-id="955b5-1813">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1813">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="955b5-1814">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-1814">Core</span></span>

* <span data-ttu-id="955b5-1815">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="955b5-1815">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="955b5-1816">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="955b5-1816">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="955b5-1817">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="955b5-1817">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="955b5-1818">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="955b5-1818">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="955b5-1819">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="955b5-1819">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="955b5-1820">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="955b5-1820">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="955b5-1821">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="955b5-1821">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="955b5-1822">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="955b5-1822">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="955b5-1823">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="955b5-1823">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="955b5-1824">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="955b5-1824">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="955b5-1825">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="955b5-1825">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="955b5-1826">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="955b5-1826">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="955b5-1827">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="955b5-1827">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="955b5-1828">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="955b5-1828">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="955b5-1829">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="955b5-1829">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="955b5-1830">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="955b5-1830">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="955b5-1831">ACR</span><span class="sxs-lookup"><span data-stu-id="955b5-1831">ACR</span></span>

* <span data-ttu-id="955b5-1832">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1832">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="955b5-1833">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="955b5-1833">Support SKU update for managed registries</span></span>
* <span data-ttu-id="955b5-1834">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="955b5-1834">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="955b5-1835">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="955b5-1835">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="955b5-1836">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="955b5-1836">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="955b5-1837">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="955b5-1837">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-1838">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-1838">ACS</span></span>

* <span data-ttu-id="955b5-1839">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="955b5-1839">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-1840">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="955b5-1840">Appservice</span></span>

* <span data-ttu-id="955b5-1841">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="955b5-1841">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="955b5-1842">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="955b5-1842">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="955b5-1843">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1843">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="955b5-1844">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="955b5-1844">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="955b5-1845">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="955b5-1845">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="955b5-1846">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="955b5-1846">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="955b5-1847">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="955b5-1847">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="955b5-1848">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="955b5-1848">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="955b5-1849">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="955b5-1849">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="955b5-1850">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1850">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="955b5-1851">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="955b5-1851">Batch</span></span>

* <span data-ttu-id="955b5-1852">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="955b5-1852">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="955b5-1853">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1853">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="955b5-1854">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1854">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="955b5-1855">CDN</span><span class="sxs-lookup"><span data-stu-id="955b5-1855">CDN</span></span>

* <span data-ttu-id="955b5-1856">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="955b5-1856">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="955b5-1857">Облако</span><span class="sxs-lookup"><span data-stu-id="955b5-1857">Cloud</span></span>

* <span data-ttu-id="955b5-1858">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="955b5-1858">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="955b5-1859">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="955b5-1859">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="955b5-1860">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="955b5-1860">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="955b5-1861">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="955b5-1861">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="955b5-1862">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1862">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="955b5-1863">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="955b5-1863">CosmosDB</span></span>

* <span data-ttu-id="955b5-1864">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="955b5-1864">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="955b5-1865">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="955b5-1865">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="955b5-1866">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="955b5-1866">Data Lake Analytics</span></span>

* <span data-ttu-id="955b5-1867">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1867">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="955b5-1868">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1868">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="955b5-1869">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1869">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="955b5-1870">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="955b5-1870">Data Lake Store</span></span>

* <span data-ttu-id="955b5-1871">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1871">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="955b5-1872">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="955b5-1872">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="955b5-1873">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1873">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="955b5-1874">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="955b5-1874">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="955b5-1875">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="955b5-1875">Interactive</span></span>

* <span data-ttu-id="955b5-1876">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="955b5-1876">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="955b5-1877">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="955b5-1877">Increased test coverage</span></span>
* <span data-ttu-id="955b5-1878">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="955b5-1878">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="955b5-1879">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="955b5-1879">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="955b5-1880">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="955b5-1880">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="955b5-1881">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="955b5-1881">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="955b5-1882">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="955b5-1882">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="955b5-1883">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1883">Added `--progress` flag</span></span>
* <span data-ttu-id="955b5-1884">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1884">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="955b5-1885">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="955b5-1885">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="955b5-1886">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="955b5-1886">IoT</span></span>

* <span data-ttu-id="955b5-1887">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="955b5-1887">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="955b5-1888">(3934).</span><span class="sxs-lookup"><span data-stu-id="955b5-1888">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="955b5-1889">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="955b5-1889">Key vault</span></span>

* <span data-ttu-id="955b5-1890">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="955b5-1890">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="955b5-1891">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1891">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="955b5-1892">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="955b5-1892">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="955b5-1893">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="955b5-1893">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="955b5-1894">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1894">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="955b5-1895">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="955b5-1895">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="955b5-1896">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="955b5-1896">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="955b5-1897">(3307).</span><span class="sxs-lookup"><span data-stu-id="955b5-1897">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="955b5-1898">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="955b5-1898">Lab</span></span>

* <span data-ttu-id="955b5-1899">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1899">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="955b5-1900">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1900">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-1901">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-1901">Monitor</span></span>

* <span data-ttu-id="955b5-1902">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="955b5-1902">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="955b5-1903">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1903">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="955b5-1904">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1904">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="955b5-1905">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1905">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="955b5-1906">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1906">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="955b5-1907">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="955b5-1907">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="955b5-1908">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="955b5-1908">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="955b5-1909">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="955b5-1909">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="955b5-1910">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="955b5-1910">`location` no longer required</span></span>
  * <span data-ttu-id="955b5-1911">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="955b5-1911">Add name and ID support for target</span></span>
  * <span data-ttu-id="955b5-1912">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="955b5-1912">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="955b5-1913">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="955b5-1913">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="955b5-1914">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="955b5-1914">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="955b5-1915">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="955b5-1915">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="955b5-1916">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1916">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="955b5-1917">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1917">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="955b5-1918">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-1918">Network</span></span>

* <span data-ttu-id="955b5-1919">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1919">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="955b5-1920">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1920">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="955b5-1921">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="955b5-1921">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="955b5-1922">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1922">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="955b5-1923">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1923">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="955b5-1924">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1924">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="955b5-1925">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1925">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="955b5-1926">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1926">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="955b5-1927">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1927">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="955b5-1928">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1928">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="955b5-1929">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1929">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="955b5-1930">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1930">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="955b5-1931">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1931">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="955b5-1932">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1932">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="955b5-1933">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1933">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="955b5-1934">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1934">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="955b5-1935">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="955b5-1935">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="955b5-1936">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1936">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="955b5-1937">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1937">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="955b5-1938">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1938">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="955b5-1939">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1939">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="955b5-1940">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1940">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="955b5-1941">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1941">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="955b5-1942">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="955b5-1942">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="955b5-1943">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="955b5-1943">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="955b5-1944">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="955b5-1944">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="955b5-1945">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="955b5-1945">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="955b5-1946">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-1946">Profile</span></span>

* <span data-ttu-id="955b5-1947">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="955b5-1947">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="955b5-1948">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="955b5-1948">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="955b5-1949">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="955b5-1949">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="955b5-1950">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="955b5-1950">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="955b5-1951">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="955b5-1951">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="955b5-1952">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="955b5-1952">RDBMS</span></span>

* <span data-ttu-id="955b5-1953">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="955b5-1953">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="955b5-1954">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="955b5-1954">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="955b5-1955">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="955b5-1955">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="955b5-1956">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="955b5-1956">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-1957">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-1957">Resource</span></span>

* <span data-ttu-id="955b5-1958">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1958">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="955b5-1959">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1959">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="955b5-1960">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1960">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="955b5-1961">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1961">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="955b5-1962">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="955b5-1962">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="955b5-1963">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1963">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="955b5-1964">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="955b5-1964">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="955b5-1965">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1965">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="955b5-1966">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-1966">Role</span></span>

* <span data-ttu-id="955b5-1967">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="955b5-1967">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="955b5-1968">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="955b5-1968">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="955b5-1969">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="955b5-1969">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="955b5-1970">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="955b5-1970">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="955b5-1971">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1971">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="955b5-1972">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="955b5-1972">Service Fabric</span></span>
* <span data-ttu-id="955b5-1973">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="955b5-1973">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="955b5-1974">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="955b5-1974">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="955b5-1975">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="955b5-1975">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-1976">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-1976">SQL</span></span>

* <span data-ttu-id="955b5-1977">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1977">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="955b5-1978">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1978">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="955b5-1979">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1979">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-1980">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-1980">Storage</span></span>

* <span data-ttu-id="955b5-1981">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="955b5-1981">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="955b5-1982">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="955b5-1982">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="955b5-1983">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="955b5-1983">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="955b5-1984">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="955b5-1984">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="955b5-1985">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="955b5-1985">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="955b5-1986">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="955b5-1986">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-1987">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-1987">VM</span></span>

* <span data-ttu-id="955b5-1988">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="955b5-1988">Support configuring nsg</span></span>
* <span data-ttu-id="955b5-1989">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="955b5-1989">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="955b5-1990">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="955b5-1990">Support managed service identities</span></span>
* <span data-ttu-id="955b5-1991">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="955b5-1991">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="955b5-1992">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="955b5-1992">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="955b5-1993">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-1993">May 10, 2017</span></span>

<span data-ttu-id="955b5-1994">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="955b5-1994">Version 2.0.6</span></span>

* <span data-ttu-id="955b5-1995">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="955b5-1995">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="955b5-1996">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="955b5-1996">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="955b5-1997">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="955b5-1997">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="955b5-1998">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="955b5-1998">Include Cognitive Services module</span></span>
* <span data-ttu-id="955b5-1999">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="955b5-1999">Include Service Fabric module</span></span>
* <span data-ttu-id="955b5-2000">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="955b5-2000">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="955b5-2001">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="955b5-2001">Add support for CDN commands</span></span>
* <span data-ttu-id="955b5-2002">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="955b5-2002">Remove Container module</span></span>
* <span data-ttu-id="955b5-2003">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2003">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="955b5-2004">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2004">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="955b5-2005">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-2005">Core</span></span>

* <span data-ttu-id="955b5-2006">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="955b5-2006">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="955b5-2007">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2007">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="955b5-2008">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2008">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="955b5-2009">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2009">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="955b5-2010">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2010">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="955b5-2011">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2011">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="955b5-2012">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2012">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="955b5-2013">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2013">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="955b5-2014">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2014">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="955b5-2015">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="955b5-2015">core: Improved performance</span></span>
* <span data-ttu-id="955b5-2016">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="955b5-2016">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="955b5-2017">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="955b5-2017">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-2018">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-2018">ACS</span></span>

* <span data-ttu-id="955b5-2019">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="955b5-2019">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="955b5-2020">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="955b5-2020">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="955b5-2021">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="955b5-2021">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="955b5-2022">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2022">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-2023">AppService</span><span class="sxs-lookup"><span data-stu-id="955b5-2023">AppService</span></span>

* <span data-ttu-id="955b5-2024">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="955b5-2024">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="955b5-2025">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="955b5-2025">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="955b5-2026">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="955b5-2026">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="955b5-2027">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="955b5-2027">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="955b5-2028">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="955b5-2028">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="955b5-2029">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2029">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="955b5-2030">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="955b5-2030">support slot swap with preview</span></span>
* <span data-ttu-id="955b5-2031">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2031">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="955b5-2032">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2032">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="955b5-2033">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="955b5-2033">CosmosDB</span></span>

* <span data-ttu-id="955b5-2034">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="955b5-2034">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="955b5-2035">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="955b5-2035">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="955b5-2036">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="955b5-2036">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="955b5-2037">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="955b5-2037">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="955b5-2038">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="955b5-2038">Data Lake Analytics</span></span>

* <span data-ttu-id="955b5-2039">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="955b5-2039">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="955b5-2040">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="955b5-2040">Add support for new catalog item type: package.</span></span> <span data-ttu-id="955b5-2041">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="955b5-2041">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="955b5-2042">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="955b5-2042">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="955b5-2043">Таблица</span><span class="sxs-lookup"><span data-stu-id="955b5-2043">Table</span></span>
  * <span data-ttu-id="955b5-2044">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="955b5-2044">Table valued function</span></span>
  * <span data-ttu-id="955b5-2045">Просмотр</span><span class="sxs-lookup"><span data-stu-id="955b5-2045">View</span></span>
  * <span data-ttu-id="955b5-2046">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="955b5-2046">Table Statistics.</span></span> <span data-ttu-id="955b5-2047">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="955b5-2047">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="955b5-2048">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="955b5-2048">Data Lake Store</span></span>

* <span data-ttu-id="955b5-2049">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="955b5-2049">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="955b5-2050">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2050">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="955b5-2051">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="955b5-2051">missed help for access show.</span></span> <span data-ttu-id="955b5-2052">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="955b5-2052">adding it.</span></span> <span data-ttu-id="955b5-2053">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="955b5-2053">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="955b5-2054">Поиск</span><span class="sxs-lookup"><span data-stu-id="955b5-2054">Find</span></span>

* <span data-ttu-id="955b5-2055">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="955b5-2055">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="955b5-2056">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="955b5-2056">KeyVault</span></span>

* <span data-ttu-id="955b5-2057">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="955b5-2057">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="955b5-2058">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="955b5-2058">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="955b5-2059">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="955b5-2059">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="955b5-2060">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="955b5-2060">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="955b5-2061">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2061">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="955b5-2062">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="955b5-2062">Lab</span></span>

* <span data-ttu-id="955b5-2063">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="955b5-2063">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="955b5-2064">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="955b5-2064">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="955b5-2065">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="955b5-2065">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="955b5-2066">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="955b5-2066">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="955b5-2067">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="955b5-2067">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="955b5-2068">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="955b5-2068">Monitor</span></span>

* <span data-ttu-id="955b5-2069">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2069">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="955b5-2070">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2070">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="955b5-2071">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-2071">Network</span></span>

* <span data-ttu-id="955b5-2072">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="955b5-2072">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="955b5-2073">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-2073">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="955b5-2074">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="955b5-2074">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="955b5-2075">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="955b5-2075">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="955b5-2076">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="955b5-2076">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="955b5-2077">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="955b5-2077">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="955b5-2078">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="955b5-2078">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="955b5-2079">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="955b5-2079">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="955b5-2080">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="955b5-2080">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="955b5-2081">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="955b5-2081">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="955b5-2082">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="955b5-2082">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="955b5-2083">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-2083">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="955b5-2084">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="955b5-2084">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="955b5-2085">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="955b5-2085">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="955b5-2086">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="955b5-2086">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="955b5-2087">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="955b5-2087">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="955b5-2088">Профиль</span><span class="sxs-lookup"><span data-stu-id="955b5-2088">Profile</span></span>

* <span data-ttu-id="955b5-2089">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2089">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="955b5-2090">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2090">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="955b5-2091">Redis</span><span class="sxs-lookup"><span data-stu-id="955b5-2091">Redis</span></span>

* <span data-ttu-id="955b5-2092">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="955b5-2092">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="955b5-2093">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="955b5-2093">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="955b5-2094">Ресурс</span><span class="sxs-lookup"><span data-stu-id="955b5-2094">Resource</span></span>

* <span data-ttu-id="955b5-2095">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2095">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="955b5-2096">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2096">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="955b5-2097">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2097">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="955b5-2098">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="955b5-2098">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="955b5-2099">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="955b5-2099">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="955b5-2100">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="955b5-2100">Add docs for az lock update.</span></span> <span data-ttu-id="955b5-2101">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="955b5-2101">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="955b5-2102">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="955b5-2102">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="955b5-2103">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="955b5-2103">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="955b5-2104">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="955b5-2104">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="955b5-2105">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="955b5-2105">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="955b5-2106">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2106">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="955b5-2107">Роль</span><span class="sxs-lookup"><span data-stu-id="955b5-2107">Role</span></span>

* <span data-ttu-id="955b5-2108">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2108">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="955b5-2109">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2109">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="955b5-2110">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2110">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="955b5-2111">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="955b5-2111">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="955b5-2112">SQL</span><span class="sxs-lookup"><span data-stu-id="955b5-2112">SQL</span></span>

* <span data-ttu-id="955b5-2113">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="955b5-2113">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="955b5-2114">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2114">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="955b5-2115">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-2115">Storage</span></span>

* <span data-ttu-id="955b5-2116">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="955b5-2116">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="955b5-2117">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="955b5-2117">Add support for incremental blob copy</span></span>
* <span data-ttu-id="955b5-2118">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="955b5-2118">Add support for large block blob upload</span></span>
* <span data-ttu-id="955b5-2119">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="955b5-2119">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-2120">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-2120">VM</span></span>

* <span data-ttu-id="955b5-2121">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="955b5-2121">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="955b5-2122">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="955b5-2122">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="955b5-2123">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="955b5-2123">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="955b5-2124">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="955b5-2124">az vm/vmss disk</span></span>
  3. <span data-ttu-id="955b5-2125">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="955b5-2125">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="955b5-2126">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="955b5-2126">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="955b5-2127">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2127">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="955b5-2128">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-2128">April 3, 2017</span></span>

<span data-ttu-id="955b5-2129">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="955b5-2129">Version 2.0.2</span></span>

<span data-ttu-id="955b5-2130">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="955b5-2130">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="955b5-2131">Core</span><span class="sxs-lookup"><span data-stu-id="955b5-2131">Core</span></span>

* <span data-ttu-id="955b5-2132">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-2132">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="955b5-2133">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2133">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="955b5-2134">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2134">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="955b5-2135">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2135">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="955b5-2136">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2136">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="955b5-2137">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="955b5-2137">Add prompting for missing template parameters.</span></span> <span data-ttu-id="955b5-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2138">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="955b5-2139">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="955b5-2139">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="955b5-2140">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="955b5-2140">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="955b5-2141">ACS</span><span class="sxs-lookup"><span data-stu-id="955b5-2141">ACS</span></span>

* <span data-ttu-id="955b5-2142">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2142">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="955b5-2143">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="955b5-2143">Add support for ssh key password prompting.</span></span> <span data-ttu-id="955b5-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2144">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="955b5-2145">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="955b5-2145">Add support for windows clusters.</span></span> <span data-ttu-id="955b5-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2146">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="955b5-2147">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="955b5-2147">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="955b5-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2148">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="955b5-2149">AppService</span><span class="sxs-lookup"><span data-stu-id="955b5-2149">AppService</span></span>

* <span data-ttu-id="955b5-2150">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2150">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="955b5-2151">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2151">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="955b5-2152">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2152">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="955b5-2153">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2153">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="955b5-2154">Data Lake</span><span class="sxs-lookup"><span data-stu-id="955b5-2154">DataLake</span></span>

* <span data-ttu-id="955b5-2155">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="955b5-2155">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="955b5-2156">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="955b5-2156">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="955b5-2157">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="955b5-2157">DocuemntDB</span></span>

* <span data-ttu-id="955b5-2158">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2158">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="955b5-2159">ВМ</span><span class="sxs-lookup"><span data-stu-id="955b5-2159">VM</span></span>

* <span data-ttu-id="955b5-2160">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2160">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="955b5-2161">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2161">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="955b5-2162">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2162">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="955b5-2163">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2163">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="955b5-2164">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2164">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="955b5-2165">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2165">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="955b5-2166">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="955b5-2166">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="955b5-2167">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="955b5-2167">February 27, 2017</span></span>

<span data-ttu-id="955b5-2168">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="955b5-2168">Version 2.0.0</span></span>

<span data-ttu-id="955b5-2169">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="955b5-2169">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="955b5-2170">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="955b5-2170">Container Service (acs)</span></span>
- <span data-ttu-id="955b5-2171">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="955b5-2171">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="955b5-2172">Сеть</span><span class="sxs-lookup"><span data-stu-id="955b5-2172">Networking</span></span>
- <span data-ttu-id="955b5-2173">Хранилище</span><span class="sxs-lookup"><span data-stu-id="955b5-2173">Storage</span></span>

<span data-ttu-id="955b5-2174">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="955b5-2174">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="955b5-2175">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="955b5-2175">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="955b5-2176">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="955b5-2176">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="955b5-2177">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="955b5-2177">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="955b5-2178">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="955b5-2178">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="955b5-2179">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="955b5-2179">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="955b5-2180">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="955b5-2180">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="955b5-2181">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="955b5-2181">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="955b5-2182">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="955b5-2182">Provide feedback from the command line with the `az feedback` command</span></span>

