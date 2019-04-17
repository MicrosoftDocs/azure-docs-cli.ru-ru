---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 04/09/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: df665565130322504c4794462098980b1064a6c7
ms.sourcegitcommit: c6dff58438d256647d4aa29a53eef4bf93a0cd24
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "59480003"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="e73ef-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="e73ef-103">Azure CLI release notes</span></span>
## <a name="april-9-2019"></a><span data-ttu-id="e73ef-104">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-104">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-105">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-105">Core</span></span>
* <span data-ttu-id="e73ef-106">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="e73ef-106">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-107">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-107">ACR</span></span>
* <span data-ttu-id="e73ef-108">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="e73ef-108">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="e73ef-109">AMS</span><span class="sxs-lookup"><span data-stu-id="e73ef-109">AMS</span></span>
* [<span data-ttu-id="e73ef-110">УСТАРЕЛО</span><span class="sxs-lookup"><span data-stu-id="e73ef-110">DEPRECATED</span></span>]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [<span data-ttu-id="e73ef-111">КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ</span><span class="sxs-lookup"><span data-stu-id="e73ef-111">BREAKING CHANGE</span></span>]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="e73ef-112">Добавлена поддержка новых параметров шифрования в</span><span class="sxs-lookup"><span data-stu-id="e73ef-112">Added new encryption parameters support in</span></span> `ams streaming-policy create`
* <span data-ttu-id="e73ef-113">Добавлен новый параметр `--filters` для командлета</span><span class="sxs-lookup"><span data-stu-id="e73ef-113">Added new paramter `--filters` to</span></span> `ams streaming-locator create`

### <a name="appservice"></a><span data-ttu-id="e73ef-114">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-114">AppService</span></span>
* <span data-ttu-id="e73ef-115">Добавлена поддержка параметра `--logs` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-115">Added `--logs` support to</span></span> `webapp up`
* <span data-ttu-id="e73ef-116">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-116">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="e73ef-117">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-117">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="e73ef-118">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="e73ef-118">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="e73ef-119">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="e73ef-119">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="e73ef-120">Добавлена возможность переключать план для приложения-функции с помощью</span><span class="sxs-lookup"><span data-stu-id="e73ef-120">Added ability to switch a plan underneath a function app using</span></span> `functionapp update --plan`
* <span data-ttu-id="e73ef-121">Добавлена поддержка параметров масштабирования плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="e73ef-121">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="e73ef-122">CDN</span><span class="sxs-lookup"><span data-stu-id="e73ef-122">CDN</span></span>
* <span data-ttu-id="e73ef-123">Добавлена поддержка `Microsoft_Standard` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-123">Added support for `Microsoft_Standard` and</span></span> `Standard_ChinaCdn`

### <a name="feedback"></a><span data-ttu-id="e73ef-124">Отзыв</span><span class="sxs-lookup"><span data-stu-id="e73ef-124">Feedback</span></span>
* <span data-ttu-id="e73ef-125">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-125">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="e73ef-126">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-126">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="e73ef-127">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="e73ef-127">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-128">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-128">Monitor</span></span>
* <span data-ttu-id="e73ef-129">Исправлена проблема, из-за которой у count было недопустимое значение в</span><span class="sxs-lookup"><span data-stu-id="e73ef-129">Fixed issue where "count" was not a permitted value with</span></span> `metrics alert [create|update]` 

### <a name="network"></a><span data-ttu-id="e73ef-130">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-130">Network</span></span>
* <span data-ttu-id="e73ef-131">Исправлен формат таблицы, которая не отображалась с помощью</span><span class="sxs-lookup"><span data-stu-id="e73ef-131">Fixed table format not displaying with</span></span> `vnet-gateway list-bgp-peer-status`
* <span data-ttu-id="e73ef-132">Команды `list-request-headers` и `list-response-headers` добавлены в</span><span class="sxs-lookup"><span data-stu-id="e73ef-132">Added `list-request-headers` and `list-response-headers` commands to</span></span> `application-gateway rewrite-rule`
* <span data-ttu-id="e73ef-133">Команда `list-server-variables` добавлена в</span><span class="sxs-lookup"><span data-stu-id="e73ef-133">Added `list-server-variables` command to</span></span> `application-gateway rewrite-rule condition`
* <span data-ttu-id="e73ef-134">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута</span><span class="sxs-lookup"><span data-stu-id="e73ef-134">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception</span></span> `express-route port update`

### <a name="privatedns"></a><span data-ttu-id="e73ef-135">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="e73ef-135">PrivateDNS</span></span>
* <span data-ttu-id="e73ef-136">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-136">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-137">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-137">Resource</span></span>
* <span data-ttu-id="e73ef-138">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="e73ef-138">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-139">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-139">Role</span></span>
* <span data-ttu-id="e73ef-140">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="e73ef-140">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="e73ef-141">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="e73ef-141">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-142">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-142">SQL</span></span>
* <span data-ttu-id="e73ef-143">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="e73ef-143">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-144">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-144">Storage</span></span>
* <span data-ttu-id="e73ef-145">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Удален результат</span><span class="sxs-lookup"><span data-stu-id="e73ef-145">[BREAKING CHANGE] Removed result of</span></span> `storage blob delete`
* <span data-ttu-id="e73ef-146">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-146">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="e73ef-147">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="e73ef-147">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="e73ef-148">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="e73ef-148">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="e73ef-149">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-149">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="e73ef-150">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-150">Core</span></span>
* <span data-ttu-id="e73ef-151">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-151">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="e73ef-152">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="e73ef-152">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="e73ef-153">Облако</span><span class="sxs-lookup"><span data-stu-id="e73ef-153">Cloud</span></span>
* <span data-ttu-id="e73ef-154">Исправлена ошибка с сообщением о том, что подписка не найдена, в</span><span class="sxs-lookup"><span data-stu-id="e73ef-154">Fixed a 'subscription not found' error in</span></span> `cloud set`

### <a name="acr"></a><span data-ttu-id="e73ef-155">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-155">ACR</span></span>
* <span data-ttu-id="e73ef-156">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-156">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="e73ef-157">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-157">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="e73ef-158">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="e73ef-158">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="e73ef-159">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-159">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-160">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-160">AppService</span></span>
* <span data-ttu-id="e73ef-161">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="e73ef-161">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="e73ef-162">Исправлена ошибка, из-за которой не работали слоты для</span><span class="sxs-lookup"><span data-stu-id="e73ef-162">Fixed bug where slots didn't work for</span></span> `[webapp|functionapp] config ssl bind`

### <a name="bot-service"></a><span data-ttu-id="e73ef-163">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="e73ef-163">BOT Service</span></span>
* <span data-ttu-id="e73ef-164">Добавлена команда `bot prepare-deploy` для подготовки к развертыванию ботов с помощью</span><span class="sxs-lookup"><span data-stu-id="e73ef-164">Added `bot prepare-deploy` to prepare for deploying bots via</span></span> `webapp`
* <span data-ttu-id="e73ef-165">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="e73ef-165">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="e73ef-166">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-166">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="e73ef-167">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="e73ef-167">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="e73ef-168">CDN</span><span class="sxs-lookup"><span data-stu-id="e73ef-168">CDN</span></span>
* <span data-ttu-id="e73ef-169">Добавлена поддержка `--no-wait` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-169">Added support for `--no-wait` to</span></span> `cdn endpoint [create|update|start|stop|delete|load|purge]`  
* <span data-ttu-id="e73ef-170">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-170">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="e73ef-171">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-171">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="e73ef-172">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="e73ef-172">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e73ef-173">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="e73ef-173">Cosmosdb</span></span>
* <span data-ttu-id="e73ef-174">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="e73ef-174">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="e73ef-175">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="e73ef-175">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="e73ef-176">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-176">Interactive</span></span>
* <span data-ttu-id="e73ef-177">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="e73ef-177">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-178">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-178">Monitor</span></span>
* <span data-ttu-id="e73ef-179">Внесено изменение, разрешающее использовать значение измерения `*` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-179">Changed to allow dimension value `*` for</span></span> `monitor metrics alert [create|update]`

### <a name="network"></a><span data-ttu-id="e73ef-180">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-180">Network</span></span>
* <span data-ttu-id="e73ef-181">Добавлена группа команд `rewrite-rule` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-181">Added `rewrite-rule` command group to</span></span> `application-gateway`

### <a name="profile"></a><span data-ttu-id="e73ef-182">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-182">Profile</span></span>
* <span data-ttu-id="e73ef-183">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для</span><span class="sxs-lookup"><span data-stu-id="e73ef-183">Added tenant level account support for managed service identity to</span></span> `login`

### <a name="postgres"></a><span data-ttu-id="e73ef-184">Postgres</span><span class="sxs-lookup"><span data-stu-id="e73ef-184">Postgres</span></span> 
* <span data-ttu-id="e73ef-185">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-185">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="e73ef-186">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-186">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-187">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-187">Resource</span></span>
* <span data-ttu-id="e73ef-188">Улучшены табличные выходные данные для</span><span class="sxs-lookup"><span data-stu-id="e73ef-188">Improved table output for</span></span> `deployment [create|list|show]`
* <span data-ttu-id="e73ef-189">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="e73ef-189">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="e73ef-190">График</span><span class="sxs-lookup"><span data-stu-id="e73ef-190">Graph</span></span>
* <span data-ttu-id="e73ef-191">Добавлена поддержка `--end-date` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-191">Added support for `--end-date` to</span></span> `ad [app|sp] credential reset`
* <span data-ttu-id="e73ef-192">Добавлена поддержка разрешений для</span><span class="sxs-lookup"><span data-stu-id="e73ef-192">Added support to add permissions with</span></span> `ad app permission add`
* <span data-ttu-id="e73ef-193">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-193">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="e73ef-194">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="e73ef-194">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="e73ef-195">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="e73ef-195">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-196">storage</span><span class="sxs-lookup"><span data-stu-id="e73ef-196">storage</span></span>
* <span data-ttu-id="e73ef-197">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="e73ef-197">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="e73ef-198">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="e73ef-198">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="e73ef-199">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="e73ef-199">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="e73ef-200">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="e73ef-200">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-201">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-201">VM</span></span>
* <span data-ttu-id="e73ef-202">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-202">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="e73ef-203">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-203">March 12, 2019</span></span>

<span data-ttu-id="e73ef-204">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="e73ef-204">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-205">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-205">Core</span></span>

* <span data-ttu-id="e73ef-206">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="e73ef-206">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-207">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-207">ACR</span></span>

* <span data-ttu-id="e73ef-208">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-208">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-209">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-209">ACS</span></span>

* <span data-ttu-id="e73ef-210">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="e73ef-210">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="e73ef-211">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-211">AppService</span></span>

* <span data-ttu-id="e73ef-212">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="e73ef-212">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="e73ef-213">Удалена ошибочная инструкция вывода для</span><span class="sxs-lookup"><span data-stu-id="e73ef-213">Removed erroneous print statement for</span></span> `webapp auth update`
* <span data-ttu-id="e73ef-214">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="e73ef-214">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="e73ef-215">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="e73ef-215">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="e73ef-216">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="e73ef-216">Botservice</span></span>

* <span data-ttu-id="e73ef-217">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="e73ef-217">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="e73ef-218">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="e73ef-218">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="e73ef-219">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце</span><span class="sxs-lookup"><span data-stu-id="e73ef-219">Removed single quotes from `bot publish` command output at end of</span></span> `bot create`
* <span data-ttu-id="e73ef-220">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="e73ef-220">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-221">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-221">Container</span></span>

* <span data-ttu-id="e73ef-222">Добавлен аргумент `--no-wait` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-222">Added `--no-wait` argument to</span></span> `container [start|restart]`

### <a name="eventhub"></a><span data-ttu-id="e73ef-223">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="e73ef-223">EventHub</span></span>

* <span data-ttu-id="e73ef-224">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="e73ef-224">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="e73ef-225">Поиск</span><span class="sxs-lookup"><span data-stu-id="e73ef-225">Find</span></span>

* <span data-ttu-id="e73ef-226">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="e73ef-226">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e73ef-227">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e73ef-227">HDInsight</span></span>

* <span data-ttu-id="e73ef-228">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-228">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-229">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-229">Network</span></span>

* <span data-ttu-id="e73ef-230">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-230">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="e73ef-231">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e73ef-231">Rdbms</span></span>

* <span data-ttu-id="e73ef-232">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-232">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-233">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-233">Role</span></span>

* <span data-ttu-id="e73ef-234">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-234">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="e73ef-235">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="e73ef-235">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e73ef-236">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e73ef-236">Service Fabric</span></span>

* <span data-ttu-id="e73ef-237">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="e73ef-237">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="e73ef-238">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-238">February 26, 2019</span></span>

<span data-ttu-id="e73ef-239">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="e73ef-239">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-240">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-240">Core</span></span>

* <span data-ttu-id="e73ef-241">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="e73ef-241">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-242">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-242">ACR</span></span>

* <span data-ttu-id="e73ef-243">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-243">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="e73ef-244">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="e73ef-244">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-245">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-245">ACS</span></span>

* <span data-ttu-id="e73ef-246">Добавлен параметр `--listen-address` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-246">Added `--listen-address` option to</span></span> `aks port-forward`

### <a name="appservice"></a><span data-ttu-id="e73ef-247">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-247">AppService</span></span>

* <span data-ttu-id="e73ef-248">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-248">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="e73ef-249">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-249">Batch</span></span>
* <span data-ttu-id="e73ef-250">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-250">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="e73ef-251">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-251">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="e73ef-252">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-252">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="e73ef-253">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-253">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="e73ef-254">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="e73ef-254">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="e73ef-255">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e73ef-255">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e73ef-256">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e73ef-256">CosmosDB</span></span>

* <span data-ttu-id="e73ef-257">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="e73ef-257">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="e73ef-258">Kusto</span><span class="sxs-lookup"><span data-stu-id="e73ef-258">Kusto</span></span>

* <span data-ttu-id="e73ef-259">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="e73ef-259">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-260">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-260">Network</span></span>

* <span data-ttu-id="e73ef-261">Добавлен аргумент `--express-route-gateway-bypass` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-261">Added `--express-route-gateway-bypass` argument to</span></span> `vpn-connection [create|update]`
* <span data-ttu-id="e73ef-262">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-262">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="e73ef-263">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-263">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="e73ef-264">Добавлен аргумент `--legacy-mode` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-264">Added argument `--legacy-mode` to</span></span> `express-route peering [create|update]` 
* <span data-ttu-id="e73ef-265">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-265">Added arguments `--allow-classic-operations` and `--express-route-port` to</span></span> `express-route [create|update]`
* <span data-ttu-id="e73ef-266">Добавлен аргумент `--gateway-default-site` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-266">Added `--gateway-default-site` argument to</span></span> `vnet-gateway [create|update]`
* <span data-ttu-id="e73ef-267">Добавлены команды `ipsec-policy` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-267">Added `ipsec-policy` commands to</span></span> `vnet-gateway`

### <a name="resource"></a><span data-ttu-id="e73ef-268">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-268">Resource</span></span>

* <span data-ttu-id="e73ef-269">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="e73ef-269">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="e73ef-270">Добавлена поддержка файла параметров на основе URI для</span><span class="sxs-lookup"><span data-stu-id="e73ef-270">Added support for URI-based parameters file to</span></span> `policy assignment create`
* <span data-ttu-id="e73ef-271">Добавлена поддержка определений и параметров на основе URI для</span><span class="sxs-lookup"><span data-stu-id="e73ef-271">Added support for URI-based parameters and definitions to</span></span> `policy set-definition update`
* <span data-ttu-id="e73ef-272">Исправлена обработка параметров и правил для</span><span class="sxs-lookup"><span data-stu-id="e73ef-272">Fixed handling of parameters and rules for</span></span> `policy definition update`
* <span data-ttu-id="e73ef-273">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-273">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-274">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-274">Role</span></span>

* <span data-ttu-id="e73ef-275">Добавлена поддержка ролей приложений для</span><span class="sxs-lookup"><span data-stu-id="e73ef-275">Added support for app roles to</span></span> `ad app [create|update]`

### <a name="vm"></a><span data-ttu-id="e73ef-276">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-276">VM</span></span>

* <span data-ttu-id="e73ef-277">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="e73ef-277">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="e73ef-278">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-278">February 12, 2019</span></span>

<span data-ttu-id="e73ef-279">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="e73ef-279">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-280">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-280">Core</span></span>

* `az --version` <span data-ttu-id="e73ef-281">теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="e73ef-281">now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="e73ef-282">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="e73ef-282">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-283">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-283">ACR</span></span>
* <span data-ttu-id="e73ef-284">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-284">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="e73ef-285">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Удалены параметры `--tag` и `--manifest` из</span><span class="sxs-lookup"><span data-stu-id="e73ef-285">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from</span></span> `acr repository delete`

### <a name="acs"></a><span data-ttu-id="e73ef-286">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-286">ACS</span></span>
* <span data-ttu-id="e73ef-287">Теперь имена без учета регистра поддерживаются в</span><span class="sxs-lookup"><span data-stu-id="e73ef-287">Added support for case-insensitive names to</span></span> `aks [enable-addons|disable-addons]`
* <span data-ttu-id="e73ef-288">Добавлена поддержка операции обновления Azure Active Directory с помощью</span><span class="sxs-lookup"><span data-stu-id="e73ef-288">Added support for Azure Active Directory updating operation using</span></span> `aks update-credentials --reset-aad`
* <span data-ttu-id="e73ef-289">Добавлено пояснение, что значение `--output` игнорируется для</span><span class="sxs-lookup"><span data-stu-id="e73ef-289">Added clarification that `--output` is ignored for</span></span> `aks get-credentials`

### <a name="ams"></a><span data-ttu-id="e73ef-290">AMS</span><span class="sxs-lookup"><span data-stu-id="e73ef-290">AMS</span></span>
* <span data-ttu-id="e73ef-291">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-291">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="e73ef-292">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-292">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-293">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-293">Appservice</span></span>
* <span data-ttu-id="e73ef-294">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="e73ef-294">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="e73ef-295">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="e73ef-295">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="e73ef-296">Улучшена справка для</span><span class="sxs-lookup"><span data-stu-id="e73ef-296">Improved help for</span></span> `appservice-plan-update`
* <span data-ttu-id="e73ef-297">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="e73ef-297">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="e73ef-298">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-298">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="e73ef-299">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="e73ef-299">Botservice</span></span>
* <span data-ttu-id="e73ef-300">Улучшен пользовательский интерфейс для</span><span class="sxs-lookup"><span data-stu-id="e73ef-300">Improved UX for</span></span> `bot publish`
* <span data-ttu-id="e73ef-301">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции</span><span class="sxs-lookup"><span data-stu-id="e73ef-301">Added warning for timeouts when running `npm install` during</span></span> `az bot publish`
* <span data-ttu-id="e73ef-302">Удален недопустимый символ `.` из значения `--name` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-302">Removed invalid char `.` from `--name`  in</span></span> `az bot create`
* <span data-ttu-id="e73ef-303">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="e73ef-303">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="e73ef-304">[УСТАРЕЛО] Аргумент `--proj-name` не поддерживается. Вместо него теперь используется</span><span class="sxs-lookup"><span data-stu-id="e73ef-304">[DEPRECATED] Deprecated `--proj-name` argument in favor of</span></span> `--proj-file-path`
* <span data-ttu-id="e73ef-305">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="e73ef-305">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="e73ef-306">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-306">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="e73ef-307">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="e73ef-307">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="e73ef-308">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="e73ef-308">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="e73ef-309">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="e73ef-309">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="e73ef-310">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e73ef-310">Key Vault</span></span>
* <span data-ttu-id="e73ef-311">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании</span><span class="sxs-lookup"><span data-stu-id="e73ef-311">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using</span></span> `--id`

### <a name="monitor"></a><span data-ttu-id="e73ef-312">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-312">Monitor</span></span>
* <span data-ttu-id="e73ef-313">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения</span><span class="sxs-lookup"><span data-stu-id="e73ef-313">Changed `monitor metrics alert [create|update]` to allow dimension value</span></span> `*`

### <a name="network"></a><span data-ttu-id="e73ef-314">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-314">Network</span></span>
* <span data-ttu-id="e73ef-315">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="e73ef-315">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="e73ef-316">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-316">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="e73ef-317">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="e73ef-317">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="e73ef-318">Добавлены аргументы `--idle-timeout` и `--floating-ip` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-318">Added `--idle-timeout` and `--floating-ip` to</span></span> `lb inbound-nat-pool [create|update]`

### <a name="policy-insights"></a><span data-ttu-id="e73ef-319">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="e73ef-319">Policy Insights</span></span>
* <span data-ttu-id="e73ef-320">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-320">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="e73ef-321">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="e73ef-321">RDBMS</span></span>
* <span data-ttu-id="e73ef-322">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="e73ef-322">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="e73ef-323">Redis</span><span class="sxs-lookup"><span data-stu-id="e73ef-323">Redis</span></span>
* <span data-ttu-id="e73ef-324">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="e73ef-324">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="e73ef-325">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="e73ef-325">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="e73ef-326">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="e73ef-326">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="e73ef-327">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="e73ef-327">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="e73ef-328">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-328">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="e73ef-329">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="e73ef-329">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="e73ef-330">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e73ef-330">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-331">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-331">Role</span></span>
* <span data-ttu-id="e73ef-332">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-332">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="e73ef-333">ВМ SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-333">SQL VM</span></span>
* <span data-ttu-id="e73ef-334">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-334">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-335">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-335">VM</span></span>
* <span data-ttu-id="e73ef-336">С параметром `vm list-skus` теперь можно использовать `--all` вместо</span><span class="sxs-lookup"><span data-stu-id="e73ef-336">Changed `vm list-skus` to allow use of `--all` in place of</span></span> `--all true`
* <span data-ttu-id="e73ef-337">Добавлено</span><span class="sxs-lookup"><span data-stu-id="e73ef-337">Added</span></span> `vmss run-command [invoke | list | show]`
* <span data-ttu-id="e73ef-338">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="e73ef-338">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="e73ef-339">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-339">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="e73ef-340">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-340">January 31, 2019</span></span>

<span data-ttu-id="e73ef-341">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="e73ef-341">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-342">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-342">Core</span></span>

* <span data-ttu-id="e73ef-343">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="e73ef-343">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="e73ef-344">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-344">January 28, 2019</span></span>

<span data-ttu-id="e73ef-345">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="e73ef-345">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-346">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-346">ACR</span></span>
* <span data-ttu-id="e73ef-347">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-347">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-348">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-348">ACS</span></span>
* <span data-ttu-id="e73ef-349">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-349">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="e73ef-350">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="e73ef-350">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="e73ef-351">Добавлена поддержка операции обновления субъекта-службы с помощью</span><span class="sxs-lookup"><span data-stu-id="e73ef-351">Added support for service principal updates operation with</span></span> `aks update-credentials -reset-service-principal`

### <a name="ams"></a><span data-ttu-id="e73ef-352">AMS</span><span class="sxs-lookup"><span data-stu-id="e73ef-352">AMS</span></span>
* <span data-ttu-id="e73ef-353">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Команда `ams asset get-streaming-locators` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-353">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to</span></span> `ams asset list-streaming-locators`
* <span data-ttu-id="e73ef-354">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Команда `ams streaming-locator get-content-keys` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-354">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to</span></span> `ams streaming-locator list-content-keys`

### <a name="appservice"></a><span data-ttu-id="e73ef-355">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-355">Appservice</span></span>
* <span data-ttu-id="e73ef-356">Добавлена поддержка аналитики приложений для</span><span class="sxs-lookup"><span data-stu-id="e73ef-356">Added support for app insights on</span></span> `functionapp create`
* <span data-ttu-id="e73ef-357">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="e73ef-357">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="e73ef-358">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="e73ef-358">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-359">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-359">Container</span></span>
* <span data-ttu-id="e73ef-360">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-360">Added `container start` command</span></span>
* <span data-ttu-id="e73ef-361">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-361">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e73ef-362">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="e73ef-362">EventGrid</span></span>
* <span data-ttu-id="e73ef-363">Добавлен параметр `--deadletter-endpoint` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-363">Added `--deadletter-endpoint` parameter to</span></span> `event-subscription [create|update]`
* <span data-ttu-id="e73ef-364">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-364">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="e73ef-365">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="e73ef-365">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="e73ef-366">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="e73ef-366">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="e73ef-367">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="e73ef-367">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e73ef-368">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e73ef-368">HDInsight</span></span>
* <span data-ttu-id="e73ef-369">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Параметры `--virtual-network` и `--subnet-name` удалены из</span><span class="sxs-lookup"><span data-stu-id="e73ef-369">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from</span></span> `hdinsight [application] create`
* <span data-ttu-id="e73ef-370">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-370">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="e73ef-371">Добавлены параметры `--vnet-name` и `--subnet-name` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-371">Added `--vnet-name` and `--subnet-name` parameters to</span></span> `hdinsight create`
* <span data-ttu-id="e73ef-372">Добавлена поддержка Корпоративного пакета безопасности и шифрования дисков для</span><span class="sxs-lookup"><span data-stu-id="e73ef-372">Added support for Enterprise Security Package and disk encryption to</span></span> `hdinsight create` 
* <span data-ttu-id="e73ef-373">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-373">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="e73ef-374">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-374">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="e73ef-375">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="e73ef-375">IoT</span></span>
* <span data-ttu-id="e73ef-376">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="e73ef-376">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="e73ef-377">Kusto</span><span class="sxs-lookup"><span data-stu-id="e73ef-377">Kusto</span></span>
* <span data-ttu-id="e73ef-378">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="e73ef-378">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-379">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-379">Monitor</span></span>
* <span data-ttu-id="e73ef-380">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="e73ef-380">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="e73ef-381">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-381">Profile</span></span>
* <span data-ttu-id="e73ef-382">Теперь можно использовать учетную запись уровня клиента для управляемого удостоверения службы при операции</span><span class="sxs-lookup"><span data-stu-id="e73ef-382">Enable tenant level account for managed service identity for</span></span> `login`

### <a name="network"></a><span data-ttu-id="e73ef-383">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-383">Network</span></span>
* <span data-ttu-id="e73ef-384">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-384">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="e73ef-385">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="e73ef-385">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-386">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-386">Resource</span></span>
* <span data-ttu-id="e73ef-387">Добавлена поддержка файла параметров URI для</span><span class="sxs-lookup"><span data-stu-id="e73ef-387">Added support for URI parameters file to</span></span> `group deployment create`
* <span data-ttu-id="e73ef-388">Добавлена поддержка управляемого удостоверения для</span><span class="sxs-lookup"><span data-stu-id="e73ef-388">Added support for managed identity to</span></span> `policy assignment [create|list|show]`

### <a name="sql-virtual-machine"></a><span data-ttu-id="e73ef-389">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-389">SQL Virtual Machine</span></span>
* <span data-ttu-id="e73ef-390">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="e73ef-390">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-391">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-391">Storage</span></span>
* <span data-ttu-id="e73ef-392">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="e73ef-392">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="e73ef-393">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="e73ef-393">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-394">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-394">VM</span></span>
* <span data-ttu-id="e73ef-395">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="e73ef-395">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="e73ef-396">Добавлен флаг `--force` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-396">Added `--force` flag to</span></span> `vm encryption enable`

## <a name="january-15-2019"></a><span data-ttu-id="e73ef-397">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-397">January 15, 2019</span></span>

<span data-ttu-id="e73ef-398">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="e73ef-398">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-399">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-399">ACR</span></span>
* <span data-ttu-id="e73ef-400">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="e73ef-400">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="e73ef-401">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="e73ef-401">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="e73ef-402">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="e73ef-402">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="e73ef-403">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-403">ACS</span></span>
* <span data-ttu-id="e73ef-404">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="e73ef-404">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-405">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-405">Appservice</span></span>
* <span data-ttu-id="e73ef-406">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-406">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="e73ef-407">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="e73ef-407">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="e73ef-408">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="e73ef-408">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="e73ef-409">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-409">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="e73ef-410">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="e73ef-410">Botservice</span></span>
* <span data-ttu-id="e73ef-411">Добавлены обновления состояния развертывания для</span><span class="sxs-lookup"><span data-stu-id="e73ef-411">Added deployment status updates to</span></span> `bot create`

### <a name="configure"></a><span data-ttu-id="e73ef-412">Настройка</span><span class="sxs-lookup"><span data-stu-id="e73ef-412">Configure</span></span>
* <span data-ttu-id="e73ef-413">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-413">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e73ef-414">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e73ef-414">CosmosDB</span></span>
* <span data-ttu-id="e73ef-415">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="e73ef-415">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e73ef-416">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e73ef-416">HDInsight</span></span>
* <span data-ttu-id="e73ef-417">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="e73ef-417">Added commands for managing applications</span></span>
* <span data-ttu-id="e73ef-418">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-418">Added commands for managing script actions</span></span>
* <span data-ttu-id="e73ef-419">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="e73ef-419">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="e73ef-420">Добавлена поддержка регионального использования списка для</span><span class="sxs-lookup"><span data-stu-id="e73ef-420">Added support to list regional usage to</span></span> `hdinsight list-usage`
* <span data-ttu-id="e73ef-421">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Тип кластера по умолчанию удален из</span><span class="sxs-lookup"><span data-stu-id="e73ef-421">[BREAKING CHANGE] Removed default cluster type from</span></span> `hdinsight create`

### <a name="network"></a><span data-ttu-id="e73ef-422">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-422">Network</span></span>
* <span data-ttu-id="e73ef-423">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-423">Added `--custom-headers` and `--status-code-ranges` arguments to</span></span> `traffic-manager profile [create|update]`
* <span data-ttu-id="e73ef-424">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="e73ef-424">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="e73ef-425">Добавлены аргументы `--custom-headers` и `--subnets` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-425">Added `--custom-headers` and `--subnets` arguments to</span></span> `traffic-manager endpoint [create|update]`  
* <span data-ttu-id="e73ef-426">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-426">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-427">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-427">Role</span></span>
* <span data-ttu-id="e73ef-428">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e73ef-428">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="e73ef-429">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="e73ef-429">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="e73ef-430">Безопасность</span><span class="sxs-lookup"><span data-stu-id="e73ef-430">Security</span></span>
* <span data-ttu-id="e73ef-431">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="e73ef-431">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-432">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-432">Storage</span></span>
* <span data-ttu-id="e73ef-433">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="e73ef-433">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="e73ef-434">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-434">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="e73ef-435">Добавлен параметр `--marker` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-435">Added `--marker` parameter to</span></span> `storage [blob|file|container|share] list`
* <span data-ttu-id="e73ef-436">Добавлена отметка журнала для следующей страницы в STDERR для</span><span class="sxs-lookup"><span data-stu-id="e73ef-436">Added log marker for next page to STDERR for</span></span> `storage [blob|file|container|share] list` 
* <span data-ttu-id="e73ef-437">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-437">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-438">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-438">VM</span></span>
* <span data-ttu-id="e73ef-439">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-439">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="e73ef-440">Добавлена поддержка перекрестных ссылок на образы клиента для</span><span class="sxs-lookup"><span data-stu-id="e73ef-440">Added support for cross tenant image referencing to</span></span> `[vm|vmss] create`
* <span data-ttu-id="e73ef-441">Исправлена ошибка конфигурации по умолчанию в</span><span class="sxs-lookup"><span data-stu-id="e73ef-441">Fixed bug with default configuration in</span></span> `vm diagnostics get-default-config --windows-os`
* <span data-ttu-id="e73ef-442">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-442">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="e73ef-443">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-443">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="e73ef-444">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="e73ef-444">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="e73ef-445">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-445">December 20, 2018</span></span>

<span data-ttu-id="e73ef-446">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="e73ef-446">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="e73ef-447">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-447">Appservice</span></span>
* <span data-ttu-id="e73ef-448">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="e73ef-448">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="e73ef-449">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="e73ef-449">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="e73ef-450">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="e73ef-450">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="e73ef-451">IoT Central</span><span class="sxs-lookup"><span data-stu-id="e73ef-451">IoTCentral</span></span>
* <span data-ttu-id="e73ef-452">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="e73ef-452">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-453">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-453">Role</span></span>
* <span data-ttu-id="e73ef-454">[Критическое изменение] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-454">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-455">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-455">SQL</span></span>
* <span data-ttu-id="e73ef-456">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="e73ef-456">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-457">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-457">VM</span></span>
* <span data-ttu-id="e73ef-458">Добавлен параметр `---os-type` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-458">Added `---os-type` parameter to</span></span> `disk create`

## <a name="december-18-2018"></a><span data-ttu-id="e73ef-459">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-459">December 18, 2018</span></span>

<span data-ttu-id="e73ef-460">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="e73ef-460">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="e73ef-461">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-461">ACR</span></span>
* <span data-ttu-id="e73ef-462">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-462">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="e73ef-463">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="e73ef-463">Condensed the table layout for task list</span></span>
* <span data-ttu-id="e73ef-464">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="e73ef-464">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-465">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-465">ACS</span></span>
* <span data-ttu-id="e73ef-466">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-466">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="e73ef-467">Из аргументов AAD удалено "(PREVIEW)" для</span><span class="sxs-lookup"><span data-stu-id="e73ef-467">Removed "(PREVIEW)" from AAD arguments to</span></span> `aks create`
* <span data-ttu-id="e73ef-468">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="e73ef-468">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="e73ef-469">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-469">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="e73ef-470">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-470">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="e73ef-471">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-471">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-472">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-472">Appservice</span></span>
* <span data-ttu-id="e73ef-473">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-473">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="e73ef-474">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="e73ef-474">Botservice</span></span>
* <span data-ttu-id="e73ef-475">Добавлена поддержка анализа файла `.bot` при вызове</span><span class="sxs-lookup"><span data-stu-id="e73ef-475">Added support for `.bot` file parsing when calling</span></span> `bot show`
* <span data-ttu-id="e73ef-476">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="e73ef-476">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="e73ef-477">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="e73ef-477">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="e73ef-478">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="e73ef-478">Reduced Kudu network calls</span></span>
* <span data-ttu-id="e73ef-479">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-479">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="e73ef-480">Потребление</span><span class="sxs-lookup"><span data-stu-id="e73ef-480">Consumption</span></span>
* <span data-ttu-id="e73ef-481">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-481">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e73ef-482">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e73ef-482">CosmosDB</span></span>
* <span data-ttu-id="e73ef-483">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="e73ef-483">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="e73ef-484">Карты</span><span class="sxs-lookup"><span data-stu-id="e73ef-484">Maps</span></span>
* <span data-ttu-id="e73ef-485">Добавлена поддержка номера SKU S1 для</span><span class="sxs-lookup"><span data-stu-id="e73ef-485">Added support for the S1 SKU to</span></span> `maps account [create|update]`

### <a name="network"></a><span data-ttu-id="e73ef-486">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-486">Network</span></span>
* <span data-ttu-id="e73ef-487">Добавлена поддержка аргументов `--format` и `--log-version` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-487">Added support for `--format` and `--log-version` to</span></span> `watcher flow-log configure`
* <span data-ttu-id="e73ef-488">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="e73ef-488">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-489">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-489">Resource</span></span>
* <span data-ttu-id="e73ef-490">Исправлена обработка параметра области для групп управления в</span><span class="sxs-lookup"><span data-stu-id="e73ef-490">Fixed handling of scope parameter for management groups in</span></span> `policy assignment [create|list|delete|show|update]` 
* <span data-ttu-id="e73ef-491">Добавлена новая команда</span><span class="sxs-lookup"><span data-stu-id="e73ef-491">Added new command</span></span> `resource wait`

### <a name="storage"></a><span data-ttu-id="e73ef-492">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-492">Storage</span></span>
*  <span data-ttu-id="e73ef-493">Добавлена возможность обновления версии схемы журнала для служб хранилища в</span><span class="sxs-lookup"><span data-stu-id="e73ef-493">Added ability to update log schema version for storage services in</span></span> `storage logging update`

### <a name="vm"></a><span data-ttu-id="e73ef-494">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-494">VM</span></span>
* <span data-ttu-id="e73ef-495">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-495">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="e73ef-496">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-496">December 4, 2018</span></span>

<span data-ttu-id="e73ef-497">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="e73ef-497">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="e73ef-498">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-498">Core</span></span>
* <span data-ttu-id="e73ef-499">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-499">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="e73ef-500">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="e73ef-500">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-501">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-501">Appservice</span></span>
* <span data-ttu-id="e73ef-502">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-502">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="e73ef-503">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="e73ef-503">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-504">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-504">Network</span></span>
* <span data-ttu-id="e73ef-505">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="e73ef-505">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-506">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-506">Role</span></span>
* <span data-ttu-id="e73ef-507">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-507">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="e73ef-508">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-508">VM</span></span>
* <span data-ttu-id="e73ef-509">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e73ef-509">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="e73ef-510">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="e73ef-510">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="e73ef-511">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="e73ef-511">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="e73ef-512">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="e73ef-512">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="e73ef-513">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-513">November 20, 2018</span></span>

<span data-ttu-id="e73ef-514">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="e73ef-514">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="e73ef-515">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-515">Core</span></span>
* <span data-ttu-id="e73ef-516">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="e73ef-516">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-517">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-517">ACR</span></span>
* <span data-ttu-id="e73ef-518">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="e73ef-518">Added context token to task step</span></span>
* <span data-ttu-id="e73ef-519">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="e73ef-519">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="e73ef-520">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-520">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-521">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-521">Appservice</span></span>
* <span data-ttu-id="e73ef-522">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-522">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="e73ef-523">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-523">Updated the default `node_version`.</span></span> <span data-ttu-id="e73ef-524">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-524">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="e73ef-525">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="e73ef-525">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="e73ef-526">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="e73ef-526">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="e73ef-527">IotCentral</span><span class="sxs-lookup"><span data-stu-id="e73ef-527">IotCentral</span></span>
* <span data-ttu-id="e73ef-528">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="e73ef-528">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="e73ef-529">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="e73ef-529">KeyVault</span></span>
* <span data-ttu-id="e73ef-530">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="e73ef-530">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-531">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-531">Network</span></span>
* <span data-ttu-id="e73ef-532">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-532">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="e73ef-533">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-533">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="e73ef-534">Добавлен параметр `--zones` для поддержки зоны доступности в</span><span class="sxs-lookup"><span data-stu-id="e73ef-534">Added `--zones` for availability zone support to</span></span> `application-gateway create` 
* <span data-ttu-id="e73ef-535">Добавлены аргументы `--file-upload-limit`, `--max-request-body-size` и `--request-body-check` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-535">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to</span></span> `application-gateway waf-config set`

### <a name="rdbms"></a><span data-ttu-id="e73ef-536">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e73ef-536">Rdbms</span></span>
* <span data-ttu-id="e73ef-537">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="e73ef-537">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="e73ef-538">RBAC:</span><span class="sxs-lookup"><span data-stu-id="e73ef-538">Rbac</span></span>
* <span data-ttu-id="e73ef-539">Исправлена проблема при попытке обновления неизменяемых учетных данных в</span><span class="sxs-lookup"><span data-stu-id="e73ef-539">Fixed an issue with attempting to update immutable credentials in</span></span> `ad app update`
* <span data-ttu-id="e73ef-540">Добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем, в выходные данные</span><span class="sxs-lookup"><span data-stu-id="e73ef-540">Added output warnings to communicate breaking changes in the near future for</span></span> `ad [app|sp] list` 

### <a name="storage"></a><span data-ttu-id="e73ef-541">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-541">Storage</span></span>
* <span data-ttu-id="e73ef-542">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="e73ef-542">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="e73ef-543">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-543">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="e73ef-544">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="e73ef-544">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="e73ef-545">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-545">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-546">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-546">VM</span></span>
* <span data-ttu-id="e73ef-547">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="e73ef-547">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="e73ef-548">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры</span><span class="sxs-lookup"><span data-stu-id="e73ef-548">Changed version name parameters to `sig image-version` to be</span></span> `--image-version -e`
* <span data-ttu-id="e73ef-549">Аргумент `--image-version-name` в команде `sig image-version` больше не поддерживается. Он заменен на</span><span class="sxs-lookup"><span data-stu-id="e73ef-549">Deprecated `sig image-version` argument `--image-version-name`, replaced by</span></span> `--image-version`
* <span data-ttu-id="e73ef-550">Добавлена поддержка для использования локального диска с ОС в</span><span class="sxs-lookup"><span data-stu-id="e73ef-550">Added support to use local OS disk to</span></span> `[vm|vmss] create --ephemeral-os-disk`
* <span data-ttu-id="e73ef-551">Добавлена поддержка `--no-wait` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-551">Added support for `--no-wait` to</span></span> `snapshot create/update`
* <span data-ttu-id="e73ef-552">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-552">Added `snapshot wait` command</span></span>
* <span data-ttu-id="e73ef-553">Добавлена поддержка для использования имени экземпляра в</span><span class="sxs-lookup"><span data-stu-id="e73ef-553">Added support for using instance name with</span></span> `[vm|vmss] extension set --extension-instance-name`

## <a name="november-6-2018"></a><span data-ttu-id="e73ef-554">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-554">November 6, 2018</span></span>

<span data-ttu-id="e73ef-555">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="e73ef-555">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-556">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-556">Core</span></span>
* <span data-ttu-id="e73ef-557">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="e73ef-557">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-558">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-558">ACR</span></span>
* <span data-ttu-id="e73ef-559">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="e73ef-559">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="e73ef-560">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="e73ef-560">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-561">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-561">ACS</span></span>
* <span data-ttu-id="e73ef-562">[Критическое изменение] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-562">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="e73ef-563">Помощник</span><span class="sxs-lookup"><span data-stu-id="e73ef-563">Advisor</span></span>
* <span data-ttu-id="e73ef-564">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="e73ef-564">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="e73ef-565">AMS</span><span class="sxs-lookup"><span data-stu-id="e73ef-565">AMS</span></span>
* <span data-ttu-id="e73ef-566">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="e73ef-566">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="e73ef-567">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="e73ef-567">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="e73ef-568">Добавлена поддержка параметров шифрования в</span><span class="sxs-lookup"><span data-stu-id="e73ef-568">Added encryption parameters support to</span></span> `ams streaming-policy create`
* <span data-ttu-id="e73ef-569">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="e73ef-569">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="e73ef-570">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-570">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="e73ef-571">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-571">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="e73ef-572">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-572">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="e73ef-573">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Команда `ams streaming locator` заменена на</span><span class="sxs-lookup"><span data-stu-id="e73ef-573">[BREAKING CHANGE] Replaced `ams streaming locator` command with</span></span> `ams streaming-locator`
* <span data-ttu-id="e73ef-574">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Обновлен аргумент `--content-keys` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-574">[BREAKING CHANGE] Updated `--content-keys` argument of</span></span> `ams streaming locator`
* <span data-ttu-id="e73ef-575">[Критическое изменение] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-575">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="e73ef-576">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Команда `ams streaming policy` заменена на</span><span class="sxs-lookup"><span data-stu-id="e73ef-576">[BREAKING CHANGE] Replaced `ams streaming policy` command with</span></span> `ams streaming-policy`
* <span data-ttu-id="e73ef-577">[Критическое изменение] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-577">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="e73ef-578">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="e73ef-578">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="e73ef-579">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="e73ef-579">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="e73ef-580">[Критическое изменение] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-580">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="e73ef-581">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="e73ef-581">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="e73ef-582">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="e73ef-582">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-583">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-583">AppService</span></span>
* <span data-ttu-id="e73ef-584">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="e73ef-584">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="e73ef-585">Настройка</span><span class="sxs-lookup"><span data-stu-id="e73ef-585">Configure</span></span>
* <span data-ttu-id="e73ef-586">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="e73ef-586">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-587">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-587">Container</span></span>
* <span data-ttu-id="e73ef-588">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="e73ef-588">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="e73ef-589">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="e73ef-589">EventHub</span></span>
* <span data-ttu-id="e73ef-590">Добавлен флаг `--enable-kafka` для поддержки Kafka в</span><span class="sxs-lookup"><span data-stu-id="e73ef-590">Added `--enable-kafka` flag to support Kafka in</span></span> `eventhub namespace [create|update]`

### <a name="interactive"></a><span data-ttu-id="e73ef-591">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-591">Interactive</span></span>
* <span data-ttu-id="e73ef-592">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="e73ef-592">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-593">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-593">Monitor</span></span>
* <span data-ttu-id="e73ef-594">Добавлена поддержка имен метрик, которые включают символы косой черты (/) и точки (.), в параметр `--condition` команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-594">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in</span></span> `monitor metrics alert [create|update]`

### <a name="network"></a><span data-ttu-id="e73ef-595">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-595">Network</span></span>
* <span data-ttu-id="e73ef-596">Имена команд `network interface-endpoint` больше не поддерживаются. Вместо них следует использовать</span><span class="sxs-lookup"><span data-stu-id="e73ef-596">Deprecated `network interface-endpoint` command names in favor of</span></span> `network private-endpoint`
* <span data-ttu-id="e73ef-597">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="e73ef-597">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="e73ef-598">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде</span><span class="sxs-lookup"><span data-stu-id="e73ef-598">Fixed issue where `--ip-tags` did not work correctly with</span></span> `public-ip create` 

### <a name="profile"></a><span data-ttu-id="e73ef-599">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-599">Profile</span></span>
* <span data-ttu-id="e73ef-600">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-600">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="e73ef-601">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="e73ef-601">RDBMS</span></span>
* <span data-ttu-id="e73ef-602">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="e73ef-602">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-603">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-603">Resource</span></span>
* <span data-ttu-id="e73ef-604">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-604">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-605">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-605">Role</span></span>
* <span data-ttu-id="e73ef-606">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-606">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="e73ef-607">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-607">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="e73ef-608">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="e73ef-608">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-609">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-609">Storage</span></span>
* <span data-ttu-id="e73ef-610">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-610">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-611">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-611">VM</span></span>
* <span data-ttu-id="e73ef-612">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="e73ef-612">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="e73ef-613">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="e73ef-613">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="e73ef-614">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="e73ef-614">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="e73ef-615">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="e73ef-615">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="e73ef-616">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="e73ef-616">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="e73ef-617">Улучшена проверка аргументов команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-617">Improved argument validation for</span></span> `vm create --image`

## <a name="october-23-2018"></a><span data-ttu-id="e73ef-618">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-618">October 23, 2018</span></span>

<span data-ttu-id="e73ef-619">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="e73ef-619">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-620">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-620">Core</span></span>
* <span data-ttu-id="e73ef-621">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием</span><span class="sxs-lookup"><span data-stu-id="e73ef-621">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in</span></span> `--ids`
* <span data-ttu-id="e73ef-622">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании</span><span class="sxs-lookup"><span data-stu-id="e73ef-622">Added explicit warnings when parameters would be ignored by use of</span></span> `--ids`

### <a name="acr"></a><span data-ttu-id="e73ef-623">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-623">ACR</span></span>
* <span data-ttu-id="e73ef-624">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="e73ef-624">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="e73ef-625">CDN</span><span class="sxs-lookup"><span data-stu-id="e73ef-625">CDN</span></span>
* <span data-ttu-id="e73ef-626">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-626">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="e73ef-627">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="e73ef-627">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-628">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-628">Container</span></span>
* <span data-ttu-id="e73ef-629">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="e73ef-629">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="e73ef-630">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="e73ef-630">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="e73ef-631">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-631">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="e73ef-632">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-632">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="e73ef-633">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-633">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="e73ef-634">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="e73ef-634">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="e73ef-635">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-635">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e73ef-636">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e73ef-636">CosmosDB</span></span>
* <span data-ttu-id="e73ef-637">Добавлена поддержка `--enable-multiple-write-locations` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-637">Added `--enable-multiple-write-locations` support to</span></span> `cosmosdb create`

### <a name="interactive"></a><span data-ttu-id="e73ef-638">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-638">Interactive</span></span>
* <span data-ttu-id="e73ef-639">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-639">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="e73ef-640">IoT Central</span><span class="sxs-lookup"><span data-stu-id="e73ef-640">IoT Central</span></span>
* <span data-ttu-id="e73ef-641">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="e73ef-641">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="e73ef-642">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="e73ef-642">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-643">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-643">Monitor</span></span>
* <span data-ttu-id="e73ef-644">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="e73ef-644">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="e73ef-645">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-645">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="e73ef-646">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="e73ef-646">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="e73ef-647">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="e73ef-647">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="e73ef-648">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра</span><span class="sxs-lookup"><span data-stu-id="e73ef-648">Added `--namespace` as alias for deprecated option</span></span> `--resource-provider`
  * <span data-ttu-id="e73ef-649">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="e73ef-649">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="e73ef-650">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="e73ef-650">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="e73ef-651">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="e73ef-651">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="e73ef-652">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="e73ef-652">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="e73ef-653">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-653">Improved validation for `--event-hub` and `--event-hub-rule` arguments to</span></span> `monitor diagnostic-settings create`

### <a name="network"></a><span data-ttu-id="e73ef-654">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-654">Network</span></span>
* <span data-ttu-id="e73ef-655">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="e73ef-655">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="e73ef-656">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="e73ef-656">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="e73ef-657">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="e73ef-657">ServiceBus</span></span>
* <span data-ttu-id="e73ef-658">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="e73ef-658">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-659">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-659">SQL</span></span>
* <span data-ttu-id="e73ef-660">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="e73ef-660">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-661">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-661">Storage</span></span>
* <span data-ttu-id="e73ef-662">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-662">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="e73ef-663">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="e73ef-663">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-664">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-664">VM</span></span>
* <span data-ttu-id="e73ef-665">Для режима кэширования диска принудительно применяется значение `None` для виртуальных машин серии Lv или Lv2 в</span><span class="sxs-lookup"><span data-stu-id="e73ef-665">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in</span></span> `[vm|vmss] create`
* <span data-ttu-id="e73ef-666">Обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя в</span><span class="sxs-lookup"><span data-stu-id="e73ef-666">Updated supported size list supporting networking accelerator for</span></span> `vm create`
* <span data-ttu-id="e73ef-667">Добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра" для</span><span class="sxs-lookup"><span data-stu-id="e73ef-667">Added strong typed arguments for ultrassd iops and mbps configs for</span></span> `disk create`

## <a name="october-16-2018"></a><span data-ttu-id="e73ef-668">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-668">October 16, 2018</span></span>

<span data-ttu-id="e73ef-669">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="e73ef-669">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-670">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-670">VM</span></span>
* <span data-ttu-id="e73ef-671">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-671">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="e73ef-672">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-672">October 9, 2018</span></span>

<span data-ttu-id="e73ef-673">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="e73ef-673">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-674">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-674">Core</span></span>
* <span data-ttu-id="e73ef-675">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="e73ef-675">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-676">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-676">ACR</span></span>
* <span data-ttu-id="e73ef-677">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="e73ef-677">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-678">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-678">ACS</span></span>
* <span data-ttu-id="e73ef-679">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="e73ef-679">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="e73ef-680">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="e73ef-680">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="e73ef-681">Изменена команда `aks create`, которая больше не требует</span><span class="sxs-lookup"><span data-stu-id="e73ef-681">Changed `aks create` to no longer require</span></span> `--aad-tenant-id`
* <span data-ttu-id="e73ef-682">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-682">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-683">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-683">Container</span></span>
* <span data-ttu-id="e73ef-684">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-684">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="e73ef-685">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="e73ef-685">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="e73ef-686">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="e73ef-686">Event Hub</span></span>
* <span data-ttu-id="e73ef-687">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-687">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="e73ef-688">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="e73ef-688">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="e73ef-689">расширения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-689">Extensions</span></span>
* <span data-ttu-id="e73ef-690">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="e73ef-690">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="e73ef-691">HDInsight</span><span class="sxs-lookup"><span data-stu-id="e73ef-691">HDInsight</span></span>
* <span data-ttu-id="e73ef-692">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="e73ef-692">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="e73ef-693">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="e73ef-693">IoT</span></span>
* <span data-ttu-id="e73ef-694">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-694">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="e73ef-695">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="e73ef-695">KeyVault</span></span>
* <span data-ttu-id="e73ef-696">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="e73ef-696">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-697">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-697">Network</span></span>
* <span data-ttu-id="e73ef-698">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-698">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="e73ef-699">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="e73ef-699">See #6052</span></span>
* <span data-ttu-id="e73ef-700">Больше не поддерживается `--remote-vnet-id` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-700">Deprecated `--remote-vnet-id` for</span></span> `network vnet peering create`
* <span data-ttu-id="e73ef-701">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="e73ef-701">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="e73ef-702">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром</span><span class="sxs-lookup"><span data-stu-id="e73ef-702">Added support for multiple subnet prefixes to `network vnet create` with</span></span> `--subnet-prefixes`
* <span data-ttu-id="e73ef-703">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром</span><span class="sxs-lookup"><span data-stu-id="e73ef-703">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with</span></span> `--address-prefixes`
* <span data-ttu-id="e73ef-704">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-704">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="e73ef-705">Добавлен вспомогательный аргумент `--service-endpoint-policy` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-705">Added `--service-endpoint-policy` convenience argument to</span></span> `network vnet subnet update`

### <a name="role"></a><span data-ttu-id="e73ef-706">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-706">Role</span></span>
* <span data-ttu-id="e73ef-707">Добавлена поддержка для списка владельцев приложения Azure AD в команду</span><span class="sxs-lookup"><span data-stu-id="e73ef-707">Added support for listing Azure AD app owners to</span></span> `ad app owner`
* <span data-ttu-id="e73ef-708">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду</span><span class="sxs-lookup"><span data-stu-id="e73ef-708">Added support for listing Azure AD service principal owners to</span></span> `ad sp owner`
* <span data-ttu-id="e73ef-709">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-709">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="e73ef-710">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="e73ef-710">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="e73ef-711">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-711">Service Bus</span></span>
* <span data-ttu-id="e73ef-712">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="e73ef-712">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-713">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-713">VM</span></span>
* <span data-ttu-id="e73ef-714">Исправлено пустое поле `accessSas` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-714">Fixed empty `accessSas` field in</span></span> `disk grant-access`
* <span data-ttu-id="e73ef-715">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-715">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="e73ef-716">Исправлены команды обновления для</span><span class="sxs-lookup"><span data-stu-id="e73ef-716">Fixed update commands for</span></span> `sig`
* <span data-ttu-id="e73ef-717">Добавлена поддержка `--no-wait` для управления версиями образов в</span><span class="sxs-lookup"><span data-stu-id="e73ef-717">Added `--no-wait` support for managing image versions in</span></span> `sig`
* <span data-ttu-id="e73ef-718">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="e73ef-718">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="e73ef-719">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="e73ef-719">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="e73ef-720">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-720">September 21, 2018</span></span>

<span data-ttu-id="e73ef-721">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="e73ef-721">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-722">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-722">ACR</span></span>
* <span data-ttu-id="e73ef-723">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="e73ef-723">Added ACR Task commands</span></span>
* <span data-ttu-id="e73ef-724">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="e73ef-724">Added quick run command</span></span>
* <span data-ttu-id="e73ef-725">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-725">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="e73ef-726">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="e73ef-726">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="e73ef-727">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="e73ef-727">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="e73ef-728">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-728">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-729">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-729">ACS</span></span>
* <span data-ttu-id="e73ef-730">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-730">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="e73ef-731">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-731">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-732">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-732">AppService</span></span>

* <span data-ttu-id="e73ef-733">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="e73ef-733">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="e73ef-734">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="e73ef-734">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="e73ef-735">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-735">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="e73ef-736">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="e73ef-736">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="e73ef-737">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-737">Batch</span></span>
* <span data-ttu-id="e73ef-738">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="e73ef-738">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="e73ef-739">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-739">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="e73ef-740">Добавлен параметр `--max-tasks-per-node-option` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-740">Added `--max-tasks-per-node-option` to</span></span> `batch pool create`
* <span data-ttu-id="e73ef-741">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="e73ef-741">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e73ef-742">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="e73ef-742">Batch AI</span></span> 
* <span data-ttu-id="e73ef-743">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-743">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e73ef-744">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e73ef-744">Cognitive Services</span></span>
* <span data-ttu-id="e73ef-745">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-745">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="e73ef-746">Добавлена команда</span><span class="sxs-lookup"><span data-stu-id="e73ef-746">Added command</span></span> `cognitiveservices account list-usage`
* <span data-ttu-id="e73ef-747">Добавлена команда</span><span class="sxs-lookup"><span data-stu-id="e73ef-747">Added command</span></span> `cognitiveservices account list-kinds`
* <span data-ttu-id="e73ef-748">Добавлена команда</span><span class="sxs-lookup"><span data-stu-id="e73ef-748">Added command</span></span> `cognitiveservices account list`
* <span data-ttu-id="e73ef-749">Не рекомендуется</span><span class="sxs-lookup"><span data-stu-id="e73ef-749">Deprecated</span></span> `cognitiveservices list`
* <span data-ttu-id="e73ef-750">Изменен параметр `--name`, который теперь является необязательным для</span><span class="sxs-lookup"><span data-stu-id="e73ef-750">Changed `--name` to be optional for</span></span> `cognitiveservices account list-skus`

### <a name="container"></a><span data-ttu-id="e73ef-751">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-751">Container</span></span>
* <span data-ttu-id="e73ef-752">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-752">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="e73ef-753">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="e73ef-753">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="e73ef-754">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="e73ef-754">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="e73ef-755">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-755">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="e73ef-756">Data Lake</span><span class="sxs-lookup"><span data-stu-id="e73ef-756">Datalake</span></span>
* <span data-ttu-id="e73ef-757">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="e73ef-757">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="e73ef-758">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="e73ef-758">Interactive Shell</span></span>
* <span data-ttu-id="e73ef-759">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-759">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="e73ef-760">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-760">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="e73ef-761">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="e73ef-761">IoT</span></span>
* <span data-ttu-id="e73ef-762">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-762">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="e73ef-763">Key Vault</span><span class="sxs-lookup"><span data-stu-id="e73ef-763">Key Vault</span></span>
* <span data-ttu-id="e73ef-764">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="e73ef-764">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-765">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-765">Network</span></span>
* <span data-ttu-id="e73ef-766">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-766">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="e73ef-767">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-767">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="e73ef-768">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="e73ef-768">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="e73ef-769">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-769">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="e73ef-770">Добавлен параметр `--enable-tcp-reset` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-770">Add `--enable-tcp-reset` to</span></span> `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`
* <span data-ttu-id="e73ef-771">Добавлен параметр `--disable-outbound-snat` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-771">Add `--disable-outbound-snat` to</span></span> `network lb rule create/update`
* <span data-ttu-id="e73ef-772">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="e73ef-772">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="e73ef-773">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-773">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="e73ef-774">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-774">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* `network express-route create/update`<span data-ttu-id="e73ef-775">: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-775">: Add `--allow-global-reach` flag</span></span>
* `network vnet subnet create/update`<span data-ttu-id="e73ef-776">: Добавлена поддержка</span><span class="sxs-lookup"><span data-stu-id="e73ef-776">: Add support for</span></span> `--delegation`
* <span data-ttu-id="e73ef-777">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-777">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="e73ef-778">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-778">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="e73ef-779">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="e73ef-779">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* `dns record-set * create/update`<span data-ttu-id="e73ef-780">: Добавлена поддержка</span><span class="sxs-lookup"><span data-stu-id="e73ef-780">: Add support for</span></span> `--target-resource`
* <span data-ttu-id="e73ef-781">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="e73ef-781">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="e73ef-782">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="e73ef-782">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="e73ef-783">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="e73ef-783">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="e73ef-784">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="e73ef-784">RDBMS</span></span>
* <span data-ttu-id="e73ef-785">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="e73ef-785">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="e73ef-786">резервирование.</span><span class="sxs-lookup"><span data-stu-id="e73ef-786">Reservation</span></span>
* <span data-ttu-id="e73ef-787">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-787">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="e73ef-788">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="e73ef-788">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="e73ef-789">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="e73ef-789">Manage App</span></span>
* <span data-ttu-id="e73ef-790">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="e73ef-790">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="e73ef-791">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="e73ef-791">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-792">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-792">Role</span></span>
* <span data-ttu-id="e73ef-793">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="e73ef-793">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="e73ef-794">SignalR</span><span class="sxs-lookup"><span data-stu-id="e73ef-794">SignalR</span></span>
* <span data-ttu-id="e73ef-795">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="e73ef-795">First release</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-796">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-796">Storage</span></span>
* <span data-ttu-id="e73ef-797">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="e73ef-797">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="e73ef-798">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="e73ef-798">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-799">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-799">VM</span></span>
* <span data-ttu-id="e73ef-800">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="e73ef-800">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="e73ef-801">Добавлена поддержка общей коллекции изображений с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-801">Added support for shared image gallery through</span></span> `az sig`

## <a name="august-28-2018"></a><span data-ttu-id="e73ef-802">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-802">August 28, 2018</span></span>

<span data-ttu-id="e73ef-803">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="e73ef-803">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-804">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-804">Core</span></span>

* <span data-ttu-id="e73ef-805">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="e73ef-805">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="e73ef-806">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e73ef-806">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-807">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-807">ACR</span></span>

* <span data-ttu-id="e73ef-808">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="e73ef-808">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="e73ef-809">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-809">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-810">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-810">ACS</span></span>

* <span data-ttu-id="e73ef-811">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-811">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="e73ef-812">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="e73ef-812">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-813">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-813">AppService</span></span>

* <span data-ttu-id="e73ef-814">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="e73ef-814">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="e73ef-815">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="e73ef-815">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="e73ef-816">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e73ef-816">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="e73ef-817">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="e73ef-817">Backup</span></span>

* <span data-ttu-id="e73ef-818">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e73ef-818">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="e73ef-819">Служба Bot Service</span><span class="sxs-lookup"><span data-stu-id="e73ef-819">Bot Service</span></span>

* <span data-ttu-id="e73ef-820">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="e73ef-820">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e73ef-821">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e73ef-821">Cognitive Services</span></span>

* <span data-ttu-id="e73ef-822">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="e73ef-822">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="e73ef-823">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="e73ef-823">IoT</span></span>

* <span data-ttu-id="e73ef-824">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-824">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-825">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-825">Monitor</span></span>

* <span data-ttu-id="e73ef-826">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="e73ef-826">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="e73ef-827">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-827">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-828">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-828">Network</span></span>

* <span data-ttu-id="e73ef-829">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e73ef-829">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-830">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-830">Resource</span></span>

* <span data-ttu-id="e73ef-831">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e73ef-831">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-832">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-832">Storage</span></span>

* <span data-ttu-id="e73ef-833">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e73ef-833">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-834">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-834">VM</span></span>

* <span data-ttu-id="e73ef-835">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="e73ef-835">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="e73ef-836">Больше не поддерживается `--storage-caching` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-836">Deprecated `--storage-caching` for</span></span> `vm create`

## <a name="auguest-14-2018"></a><span data-ttu-id="e73ef-837">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-837">Auguest 14, 2018</span></span>

<span data-ttu-id="e73ef-838">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="e73ef-838">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-839">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-839">Core</span></span>

* <span data-ttu-id="e73ef-840">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-840">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="e73ef-841">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="e73ef-841">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="e73ef-842">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="e73ef-842">Telemetry</span></span>

* <span data-ttu-id="e73ef-843">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="e73ef-843">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-844">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-844">ACR</span></span>

* <span data-ttu-id="e73ef-845">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-845">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="e73ef-846">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-846">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-847">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-847">ACS</span></span>

* <span data-ttu-id="e73ef-848">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="e73ef-848">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="e73ef-849">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="e73ef-849">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="e73ef-850">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="e73ef-850">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="e73ef-851">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="e73ef-851">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="e73ef-852">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="e73ef-852">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="e73ef-853">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-853">AppService</span></span>

* <span data-ttu-id="e73ef-854">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-854">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="e73ef-855">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="e73ef-855">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="e73ef-856">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e73ef-856">BatchAI</span></span>

* <span data-ttu-id="e73ef-857">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="e73ef-857">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="e73ef-858">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-858">Container</span></span>

* <span data-ttu-id="e73ef-859">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="e73ef-859">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="e73ef-860">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="e73ef-860">IoT</span></span>

* <span data-ttu-id="e73ef-861">[Критическое изменение] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-861">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="e73ef-862">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-862">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="e73ef-863">IoT Central</span><span class="sxs-lookup"><span data-stu-id="e73ef-863">Iot Central</span></span>

* <span data-ttu-id="e73ef-864">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="e73ef-864">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e73ef-865">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="e73ef-865">KeyVault</span></span>


* <span data-ttu-id="e73ef-866">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-866">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="e73ef-867">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="e73ef-867">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="e73ef-868">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="e73ef-868">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="e73ef-869">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-869">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="e73ef-870">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-870">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="e73ef-871">Передача</span><span class="sxs-lookup"><span data-stu-id="e73ef-871">Relay</span></span>

* <span data-ttu-id="e73ef-872">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="e73ef-872">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-873">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-873">Sql</span></span>

* <span data-ttu-id="e73ef-874">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-874">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-875">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-875">Storage</span></span>

* <span data-ttu-id="e73ef-876">[Критическое изменение] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="e73ef-876">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="e73ef-877">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="e73ef-877">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="e73ef-878">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-878">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="e73ef-879">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="e73ef-879">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="e73ef-880">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="e73ef-880">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-881">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-881">VM</span></span>

* <span data-ttu-id="e73ef-882">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="e73ef-882">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="e73ef-883">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-883">July 31, 2018</span></span>

<span data-ttu-id="e73ef-884">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="e73ef-884">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-885">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-885">ACR</span></span>

* <span data-ttu-id="e73ef-886">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-886">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="e73ef-887">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-887">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-888">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-888">ACS</span></span>

* <span data-ttu-id="e73ef-889">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="e73ef-889">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="e73ef-890">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-890">Batch</span></span>

* <span data-ttu-id="e73ef-891">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="e73ef-891">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-892">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-892">Container</span></span>

* <span data-ttu-id="e73ef-893">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-893">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-894">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-894">Network</span></span>

* <span data-ttu-id="e73ef-895">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-895">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="e73ef-896">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-896">Resource</span></span>

* <span data-ttu-id="e73ef-897">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-897">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="e73ef-898">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="e73ef-898">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-899">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-899">Role</span></span>

* <span data-ttu-id="e73ef-900">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e73ef-900">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="e73ef-901">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="e73ef-901">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="e73ef-902">поиска</span><span class="sxs-lookup"><span data-stu-id="e73ef-902">Search</span></span>

* <span data-ttu-id="e73ef-903">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="e73ef-903">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="e73ef-904">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-904">Service Bus</span></span>

* <span data-ttu-id="e73ef-905">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="e73ef-905">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="e73ef-906">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="e73ef-906">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  `--enable-batched-operations` <span data-ttu-id="e73ef-907">и `--enable-dead-lettering-on-message-expiration` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-907">and `--enable-dead-lettering-on-message-expiration` in</span></span> `queue`
  *  `--dead-letter-on-filter-exceptions` <span data-ttu-id="e73ef-908">больше</span><span class="sxs-lookup"><span data-stu-id="e73ef-908">in</span></span> `subscriptions`

### <a name="storage"></a><span data-ttu-id="e73ef-909">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-909">Storage</span></span>

* <span data-ttu-id="e73ef-910">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-910">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="e73ef-911">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="e73ef-911">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-912">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-912">VM</span></span>

* <span data-ttu-id="e73ef-913">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="e73ef-913">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="e73ef-914">Добавлена поддержка</span><span class="sxs-lookup"><span data-stu-id="e73ef-914">Added support for</span></span> `StandardSSD_LRS`
* <span data-ttu-id="e73ef-915">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="e73ef-915">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="e73ef-916">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="e73ef-916">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="e73ef-917">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-917">July 18, 2018</span></span>

<span data-ttu-id="e73ef-918">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="e73ef-918">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-919">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-919">Core</span></span>

* <span data-ttu-id="e73ef-920">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="e73ef-920">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="e73ef-921">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="e73ef-921">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="e73ef-922">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="e73ef-922">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-923">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-923">ACR</span></span>

* <span data-ttu-id="e73ef-924">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="e73ef-924">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="e73ef-925">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-925">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="e73ef-926">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-926">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="e73ef-927">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="e73ef-927">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-928">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-928">ACS</span></span>

* <span data-ttu-id="e73ef-929">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="e73ef-929">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-930">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-930">AppService</span></span>

* <span data-ttu-id="e73ef-931">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="e73ef-931">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="e73ef-932">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-932">Batch</span></span>

* <span data-ttu-id="e73ef-933">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="e73ef-933">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="e73ef-934">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="e73ef-934">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e73ef-935">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="e73ef-935">Batch AI</span></span>

* <span data-ttu-id="e73ef-936">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-936">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-937">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-937">Container</span></span>

* <span data-ttu-id="e73ef-938">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="e73ef-938">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="e73ef-939">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="e73ef-939">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-940">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-940">Network</span></span>

* <span data-ttu-id="e73ef-941">Добавлена поддержка `--no-wait` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-941">Added `--no-wait` support to</span></span> `network nic [create|update|delete]` 
* <span data-ttu-id="e73ef-942">Добавлено</span><span class="sxs-lookup"><span data-stu-id="e73ef-942">Added</span></span> `network nic wait`
* <span data-ttu-id="e73ef-943">Больше не поддерживается аргумент `--ids` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-943">Deprecated `--ids` argument for</span></span> `network vnet [subnet|peering] list`
* <span data-ttu-id="e73ef-944">Добавлен флаг `--include-default`, позволяющий включать стандартные правила безопасности в выходные данные команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-944">Added `--include-default` flag to include default security rules in the output of</span></span> `network nsg rule list`  

### <a name="resource"></a><span data-ttu-id="e73ef-945">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-945">Resource</span></span>

* <span data-ttu-id="e73ef-946">Добавлена поддержка `--no-wait` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-946">Added `--no-wait` support to</span></span> `group deployment delete`
* <span data-ttu-id="e73ef-947">Добавлена поддержка `--no-wait` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-947">Added `--no-wait` support to</span></span> `deployment delete`
* <span data-ttu-id="e73ef-948">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-948">Added `deployment wait` command</span></span>
* <span data-ttu-id="e73ef-949">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="e73ef-949">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-950">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-950">SQL</span></span>

* <span data-ttu-id="e73ef-951">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-951">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="e73ef-952">Разрешена настройка сервера SQL Server по умолчанию с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-952">Allow configuring default sql server by executing</span></span> `az configure --defaults sql-server=<name>`
* <span data-ttu-id="e73ef-953">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-953">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-954">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-954">Storage</span></span>

* <span data-ttu-id="e73ef-955">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-955">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-956">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-956">VM</span></span>

* <span data-ttu-id="e73ef-957">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-957">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="e73ef-958">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-958">Added `--no-wait` support to `vm extension [set|delete]` and</span></span> `vmss extension [set|delete]`
* <span data-ttu-id="e73ef-959">Добавлено</span><span class="sxs-lookup"><span data-stu-id="e73ef-959">Added</span></span> `vm extension wait`

## <a name="july-3-2018"></a><span data-ttu-id="e73ef-960">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-960">July 3, 2018</span></span>

<span data-ttu-id="e73ef-961">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="e73ef-961">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="e73ef-962">AKS</span><span class="sxs-lookup"><span data-stu-id="e73ef-962">AKS</span></span>

* <span data-ttu-id="e73ef-963">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-963">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="e73ef-964">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-964">July 3, 2018</span></span>

<span data-ttu-id="e73ef-965">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="e73ef-965">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-966">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-966">Core</span></span>

* <span data-ttu-id="e73ef-967">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="e73ef-967">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-968">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-968">ACR</span></span>

* <span data-ttu-id="e73ef-969">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="e73ef-969">Added polling build status</span></span>
* <span data-ttu-id="e73ef-970">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="e73ef-970">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="e73ef-971">Добавлены параметры `--top` и `--orderby` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-971">Added `--top` and `--orderby` parameters for</span></span> `show-manifests`

### <a name="acs"></a><span data-ttu-id="e73ef-972">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-972">ACS</span></span>

* <span data-ttu-id="e73ef-973">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-973">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="e73ef-974">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-974">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="e73ef-975">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-975">Updated options for `aks browse` command.</span></span> <span data-ttu-id="e73ef-976">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-976">Added `--listen-port` support</span></span>
* <span data-ttu-id="e73ef-977">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-977">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="e73ef-978">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="e73ef-978">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="e73ef-979">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-979">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-980">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-980">AppService</span></span>

* <span data-ttu-id="e73ef-981">Добавлена поддержка отключения удостоверения с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-981">Added support for disabling identity via</span></span> `webapp identity remove`
* <span data-ttu-id="e73ef-982">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="e73ef-982">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="e73ef-983">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="e73ef-983">Backup</span></span>

* <span data-ttu-id="e73ef-984">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="e73ef-984">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="e73ef-985">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e73ef-985">BatchAI</span></span>

* <span data-ttu-id="e73ef-986">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-986">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="e73ef-987">Облако</span><span class="sxs-lookup"><span data-stu-id="e73ef-987">Cloud</span></span>

* <span data-ttu-id="e73ef-988">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-988">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-989">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-989">Container</span></span>

* <span data-ttu-id="e73ef-990">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-990">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="e73ef-991">Добавлены параметры Log Analytics `--log-analytics-workspace` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-991">Added Log Analytics parameters `--log-analytics-workspace` and</span></span> `--log-analytics-workspace-key`
* <span data-ttu-id="e73ef-992">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="e73ef-992">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="e73ef-993">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="e73ef-993">Extension</span></span>

* <span data-ttu-id="e73ef-994">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="e73ef-994">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-995">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-995">Network</span></span>

* <span data-ttu-id="e73ef-996">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-996">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="e73ef-997">Rdbms</span><span class="sxs-lookup"><span data-stu-id="e73ef-997">Rdbms</span></span>

* <span data-ttu-id="e73ef-998">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-998">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-999">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-999">Resource</span></span>

* <span data-ttu-id="e73ef-1000">Добавлена новая группа операций</span><span class="sxs-lookup"><span data-stu-id="e73ef-1000">Added new operation group</span></span> `deployment`

### <a name="vm"></a><span data-ttu-id="e73ef-1001">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1001">VM</span></span>

* <span data-ttu-id="e73ef-1002">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1002">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="e73ef-1003">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1003">June 25, 2018</span></span>

<span data-ttu-id="e73ef-1004">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="e73ef-1004">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="e73ef-1005">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="e73ef-1005">CLI</span></span>

* <span data-ttu-id="e73ef-1006">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1006">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="e73ef-1007">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1007">June 19, 2018</span></span>

<span data-ttu-id="e73ef-1008">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="e73ef-1008">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1009">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1009">Core</span></span>

* <span data-ttu-id="e73ef-1010">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1010">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-1011">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-1011">ACR</span></span>

* <span data-ttu-id="e73ef-1012">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1012">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="e73ef-1013">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1013">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1014">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1014">ACS</span></span>

* <span data-ttu-id="e73ef-1015">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1015">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="e73ef-1016">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1016">Added `--update` support</span></span>
* <span data-ttu-id="e73ef-1017">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1017">Changed `aks get-credentials --admin` to not eplace the user context in</span></span> `$HOME/.kube/config`
* <span data-ttu-id="e73ef-1018">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1018">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="e73ef-1019">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1019">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="e73ef-1020">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1020">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and</span></span> `aks remove-connector`
* <span data-ttu-id="e73ef-1021">Добавлены новые регионы для службы "Экземпляры контейнеров Azure" для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1021">Added new Azure Container Instance regions for</span></span> `aks install-connector`
* <span data-ttu-id="e73ef-1022">В имя выпуска и имя узла Helm добавлено нормализованное расположение для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1022">Added the normalized location into the helm release name and node name to</span></span> `aks install-connector`

### <a name="appservice"></a><span data-ttu-id="e73ef-1023">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-1023">AppService</span></span>

* <span data-ttu-id="e73ef-1024">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1024">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="e73ef-1025">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1025">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="e73ef-1026">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-1026">Batch</span></span>

* <span data-ttu-id="e73ef-1027">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1027">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e73ef-1028">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="e73ef-1028">Batch AI</span></span>

* <span data-ttu-id="e73ef-1029">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1029">Added support for workspaces.</span></span> <span data-ttu-id="e73ef-1030">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1030">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="e73ef-1031">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1031">Added support for experiments.</span></span> <span data-ttu-id="e73ef-1032">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1032">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="e73ef-1033">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1033">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="e73ef-1034">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1034">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="e73ef-1035">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1035">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="e73ef-1036">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1036">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="e73ef-1037">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1037">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="e73ef-1038">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1038">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="e73ef-1039">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1039">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="e73ef-1040">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1040">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="e73ef-1041">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1041">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="e73ef-1042">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1042">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="e73ef-1043">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1043">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="e73ef-1044">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1044">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="e73ef-1045">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1045">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="e73ef-1046">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1046">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="e73ef-1047">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="e73ef-1047">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="e73ef-1048">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="e73ef-1048">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="e73ef-1049">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="e73ef-1049">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="e73ef-1050">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="e73ef-1050">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="e73ef-1051">Карты</span><span class="sxs-lookup"><span data-stu-id="e73ef-1051">Maps</span></span>

* <span data-ttu-id="e73ef-1052">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1052">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1053">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1053">Network</span></span>

* <span data-ttu-id="e73ef-1054">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1054">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="e73ef-1055">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1055">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="e73ef-1056">№ 6502</span><span class="sxs-lookup"><span data-stu-id="e73ef-1056">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="e73ef-1057">Резервирование</span><span class="sxs-lookup"><span data-stu-id="e73ef-1057">Reservations</span></span>

* <span data-ttu-id="e73ef-1058">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Добавлен обязательный параметр `ReservedResourceType` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1058">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to</span></span> `reservations catalog show`
* <span data-ttu-id="e73ef-1059">Добавлен параметр `Location` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1059">Added parameter `Location`to</span></span> `reservations catalog show`
* <span data-ttu-id="e73ef-1060">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Удален параметр `kind` из команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1060">[BREAKING CHANGE] Removed `kind` from</span></span> `ReservationProperties`
* <span data-ttu-id="e73ef-1061">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Параметр `capabilities` переименован в `sku_properties` в команде</span><span class="sxs-lookup"><span data-stu-id="e73ef-1061">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in</span></span> `Catalog`
* <span data-ttu-id="e73ef-1062">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Удалены свойства `size` и `tier` из команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1062">[BREAKING CHANGE] Removed `size` and `tier` properties from</span></span> `Catalog`
* <span data-ttu-id="e73ef-1063">Добавлен параметр `InstanceFlexibility` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1063">Added parameter `InstanceFlexibility` to</span></span> `reservations reservation update`

### <a name="role"></a><span data-ttu-id="e73ef-1064">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1064">Role</span></span>

* <span data-ttu-id="e73ef-1065">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1065">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-1066">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-1066">SQL</span></span>

* <span data-ttu-id="e73ef-1067">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1067">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-1068">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1068">Storage</span></span>

* <span data-ttu-id="e73ef-1069">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1069">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1070">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1070">VM</span></span>

* <span data-ttu-id="e73ef-1071">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1071">Improved refine vm size check for accelerated networking support in</span></span> `vm create`
* <span data-ttu-id="e73ef-1072">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на</span><span class="sxs-lookup"><span data-stu-id="e73ef-1072">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to</span></span> `Standard_DS1_v2`
* <span data-ttu-id="e73ef-1073">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1073">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e73ef-1074">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1074">June 13, 2018</span></span>

<span data-ttu-id="e73ef-1075">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="e73ef-1075">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1076">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1076">Core</span></span>

* <span data-ttu-id="e73ef-1077">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1077">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="e73ef-1078">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1078">June 13, 2018</span></span>

<span data-ttu-id="e73ef-1079">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="e73ef-1079">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="e73ef-1080">AKS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1080">AKS</span></span>

* <span data-ttu-id="e73ef-1081">Добавлены дополнительные сетевые параметры в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1081">Added advanced networking options to</span></span> `aks create`
* <span data-ttu-id="e73ef-1082">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1082">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="e73ef-1083">Добавлен аргумент `--no-ssh-key` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1083">Added `--no-ssh-key` argument to</span></span> `aks create`
* <span data-ttu-id="e73ef-1084">Добавлен аргумент `--enable-rbac` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1084">Added `--enable-rbac` argument to</span></span> `aks create`
* <span data-ttu-id="e73ef-1085">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка аутентификации Azure Active Directory в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1085">[PREVIEW] Added support for Azure Active Directory authentication to</span></span> `aks create`

### <a name="appservice"></a><span data-ttu-id="e73ef-1086">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-1086">AppService</span></span>

* <span data-ttu-id="e73ef-1087">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1087">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e73ef-1088">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1088">June 5, 2018</span></span>

<span data-ttu-id="e73ef-1089">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="e73ef-1089">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="e73ef-1090">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-1090">Interactive</span></span>

* <span data-ttu-id="e73ef-1091">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1091">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="e73ef-1092">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1092">June 5, 2018</span></span>

<span data-ttu-id="e73ef-1093">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="e73ef-1093">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1094">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1094">Core</span></span>

* <span data-ttu-id="e73ef-1095">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1095">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="e73ef-1096">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1096">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-1097">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-1097">ACR</span></span>

* <span data-ttu-id="e73ef-1098">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1098">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="e73ef-1099">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1099">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="e73ef-1100">AKS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1100">AKS</span></span>

* <span data-ttu-id="e73ef-1101">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1101">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="e73ef-1102">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-1102">Batch</span></span>

* <span data-ttu-id="e73ef-1103">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="e73ef-1103">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="e73ef-1104">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="e73ef-1104">IOT</span></span>

* <span data-ttu-id="e73ef-1105">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="e73ef-1105">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1106">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1106">Network</span></span>

* <span data-ttu-id="e73ef-1107">Улучшена команда</span><span class="sxs-lookup"><span data-stu-id="e73ef-1107">Improved</span></span> `network vnet peering`

### <a name="policy-insights"></a><span data-ttu-id="e73ef-1108">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="e73ef-1108">Policy Insights</span></span>

* <span data-ttu-id="e73ef-1109">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="e73ef-1109">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="e73ef-1110">ARM</span><span class="sxs-lookup"><span data-stu-id="e73ef-1110">ARM</span></span>

* <span data-ttu-id="e73ef-1111">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1111">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-1112">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-1112">SQL</span></span>

* <span data-ttu-id="e73ef-1113">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1113">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="e73ef-1114">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1114">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="e73ef-1115">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1115">Storage</span></span>

* <span data-ttu-id="e73ef-1116">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1116">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1117">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1117">VM</span></span>

* <span data-ttu-id="e73ef-1118">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1118">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="e73ef-1119">Добавлен параметр `--accelerated-networking` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1119">Added `--accelerated-networking` option to</span></span> `vm create`
* <span data-ttu-id="e73ef-1120">Добавлен параметр `--tags` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1120">Added `--tags` to</span></span> `identity create`

## <a name="may-22-2018"></a><span data-ttu-id="e73ef-1121">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1121">May 22, 2018</span></span>

<span data-ttu-id="e73ef-1122">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="e73ef-1122">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1123">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1123">Core</span></span>

* <span data-ttu-id="e73ef-1124">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1124">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1125">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1125">ACS</span></span>

* <span data-ttu-id="e73ef-1126">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1126">Added new Dev-Spaces commands `aks use-dev-spaces` and</span></span> `aks remove-dev-spaces`
* <span data-ttu-id="e73ef-1127">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1127">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1128">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-1128">AppService</span></span>

* <span data-ttu-id="e73ef-1129">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1129">Improved generic update commands</span></span>
* <span data-ttu-id="e73ef-1130">Добавлена поддержка асинхронного выполнения для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1130">Added async support for</span></span> `webapp deployment source config-zip`

### <a name="container"></a><span data-ttu-id="e73ef-1131">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1131">Container</span></span>

* <span data-ttu-id="e73ef-1132">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1132">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="e73ef-1133">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1133">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e73ef-1134">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1134">Extension</span></span>

* <span data-ttu-id="e73ef-1135">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1135">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="e73ef-1136">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-1136">Interactive</span></span>

* <span data-ttu-id="e73ef-1137">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1137">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="e73ef-1138">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1138">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="e73ef-1139">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="e73ef-1139">KeyVault</span></span>

* <span data-ttu-id="e73ef-1140">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1140">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1141">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1141">Network</span></span>

* <span data-ttu-id="e73ef-1142">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="e73ef-1142">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="e73ef-1143">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="e73ef-1143">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-1144">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-1144">SQL</span></span>

* <span data-ttu-id="e73ef-1145">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1145">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="e73ef-1146">Свойство `serviceLevelObjective` переименовано в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1146">Renamed `serviceLevelObjective` property to</span></span> `currentServiceObjectiveName`
    * <span data-ttu-id="e73ef-1147">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1147">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="e73ef-1148">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1148">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="e73ef-1149">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1149">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * `requestedServiceObjectiveName`<span data-ttu-id="e73ef-1150">.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1150">.</span></span>  <span data-ttu-id="e73ef-1151">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1151">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * `edition`<span data-ttu-id="e73ef-1152">.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1152">.</span></span> <span data-ttu-id="e73ef-1153">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1153">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * `elasticPoolName`<span data-ttu-id="e73ef-1154">.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1154">.</span></span> <span data-ttu-id="e73ef-1155">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1155">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="e73ef-1156">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1156">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * `edition`<span data-ttu-id="e73ef-1157">.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1157">.</span></span> <span data-ttu-id="e73ef-1158">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1158">To update, use the `--edition` parameter</span></span>
    * `dtu`<span data-ttu-id="e73ef-1159">.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1159">.</span></span> <span data-ttu-id="e73ef-1160">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1160">To update, use the `--capacity` parameter</span></span>
    *  `databaseDtuMin`<span data-ttu-id="e73ef-1161">.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1161">.</span></span> <span data-ttu-id="e73ef-1162">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1162">To update, use the `--db-min-capacity` parameter</span></span>
    *  `databaseDtuMax`<span data-ttu-id="e73ef-1163">.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1163">.</span></span> <span data-ttu-id="e73ef-1164">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1164">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="e73ef-1165">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1165">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="e73ef-1166">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1166">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-1167">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1167">Storage</span></span>

* <span data-ttu-id="e73ef-1168">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1168">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="e73ef-1169">Устранена проблема с</span><span class="sxs-lookup"><span data-stu-id="e73ef-1169">Fixed problem with</span></span> `storage entity query`

### <a name="vm"></a><span data-ttu-id="e73ef-1170">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1170">VM</span></span>

* <span data-ttu-id="e73ef-1171">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1171">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="e73ef-1172">Такие же возможности предоставляет команда `vm update` или</span><span class="sxs-lookup"><span data-stu-id="e73ef-1172">The same support can be accessed through `vm update` or</span></span> `vm disk attach`
* <span data-ttu-id="e73ef-1173">Устранена проблема с сопоставлением образов расширения в команде</span><span class="sxs-lookup"><span data-stu-id="e73ef-1173">Fixed extension image matching in</span></span> `[vm|vmss] extension`
* <span data-ttu-id="e73ef-1174">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1174">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="e73ef-1175">Добавлен параметр `--license-type` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1175">Added `--license-type` to</span></span> `[vm|vmss] update`

## <a name="may-7-2018"></a><span data-ttu-id="e73ef-1176">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1176">May 7, 2018</span></span>

<span data-ttu-id="e73ef-1177">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="e73ef-1177">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1178">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1178">Core</span></span>

* <span data-ttu-id="e73ef-1179">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1179">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="e73ef-1180">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1180">Added limited support for positional arguments</span></span>
* <span data-ttu-id="e73ef-1181">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1181">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="e73ef-1182">№ 5591</span><span class="sxs-lookup"><span data-stu-id="e73ef-1182">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="e73ef-1183">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1183">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="e73ef-1184">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1184">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="e73ef-1185">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1185">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="e73ef-1186">Исправлена ошибка, когда пользователи вводят</span><span class="sxs-lookup"><span data-stu-id="e73ef-1186">Improved error when users type</span></span> `az ''`
* <span data-ttu-id="e73ef-1187">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1187">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-1188">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-1188">ACR</span></span>

* <span data-ttu-id="e73ef-1189">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1189">Added ACR Build commands</span></span>
* <span data-ttu-id="e73ef-1190">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1190">Improved resource not found error messages</span></span>
* <span data-ttu-id="e73ef-1191">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1191">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="e73ef-1192">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1192">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="e73ef-1193">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1193">Improved repository commands error messages</span></span>
* <span data-ttu-id="e73ef-1194">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1194">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1195">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1195">ACS</span></span>

* <span data-ttu-id="e73ef-1196">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1196">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="e73ef-1197">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1197">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="e73ef-1198">AMS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1198">AMS</span></span>

* <span data-ttu-id="e73ef-1199">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1199">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1200">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1200">Appservice</span></span>

* <span data-ttu-id="e73ef-1201">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1201">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="e73ef-1202">Удален параметр `--runtime-version` из</span><span class="sxs-lookup"><span data-stu-id="e73ef-1202">Removed `--runtime-version` from</span></span> `webapp auth update`
* <span data-ttu-id="e73ef-1203">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1203">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="e73ef-1204">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1204">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="e73ef-1205">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="e73ef-1205">Batch AI</span></span>

* <span data-ttu-id="e73ef-1206">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1206">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e73ef-1207">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e73ef-1207">Cognitive Services</span></span>

* <span data-ttu-id="e73ef-1208">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1208">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="e73ef-1209">Потребление</span><span class="sxs-lookup"><span data-stu-id="e73ef-1209">Consumption</span></span>

* <span data-ttu-id="e73ef-1210">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1210">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-1211">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1211">Container</span></span>

* <span data-ttu-id="e73ef-1212">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1212">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="e73ef-1213">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="e73ef-1213">Cosmos DB</span></span>

* <span data-ttu-id="e73ef-1214">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e73ef-1214">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="e73ef-1215">DMS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1215">DMS</span></span>

* <span data-ttu-id="e73ef-1216">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1216">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="e73ef-1217">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1217">Extension</span></span>

* <span data-ttu-id="e73ef-1218">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1218">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="e73ef-1219">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-1219">Interactive</span></span>

* <span data-ttu-id="e73ef-1220">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1220">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="e73ef-1221">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1221">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="e73ef-1222">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1222">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="e73ef-1223">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1223">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="e73ef-1224">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="e73ef-1224">Lab</span></span>

* <span data-ttu-id="e73ef-1225">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1225">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1226">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1226">Network</span></span>

* <span data-ttu-id="e73ef-1227">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1227">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="e73ef-1228">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1228">Profile</span></span>

* <span data-ttu-id="e73ef-1229">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1229">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="e73ef-1230">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1230">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="e73ef-1231">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1231">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="e73ef-1232">Redis</span><span class="sxs-lookup"><span data-stu-id="e73ef-1232">Redis</span></span>

* <span data-ttu-id="e73ef-1233">Вместо `redis patch-schedule patch-schedule show` теперь используется</span><span class="sxs-lookup"><span data-stu-id="e73ef-1233">Deprecated `redis patch-schedule patch-schedule show` in favor of</span></span> `redis patch-schedule show`
* <span data-ttu-id="e73ef-1234">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1234">Deprecated `redis list-all`.</span></span> <span data-ttu-id="e73ef-1235">Эта функция включена в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1235">This functionality has been folded into</span></span> `redis list`
* <span data-ttu-id="e73ef-1236">Вместо `redis import-method` теперь используется</span><span class="sxs-lookup"><span data-stu-id="e73ef-1236">Deprecated `redis import-method` in favor of</span></span> `redis import`
* <span data-ttu-id="e73ef-1237">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1237">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-1238">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1238">Role</span></span>

* <span data-ttu-id="e73ef-1239">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Удалено по причине устаревания:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1239">[BREAKING CHANGE] Removed deprecated</span></span> `ad sp reset-credentials`

### <a name="storage"></a><span data-ttu-id="e73ef-1240">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1240">Storage</span></span>

* <span data-ttu-id="e73ef-1241">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1241">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="e73ef-1242">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1242">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="e73ef-1243">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1243">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="e73ef-1244">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="e73ef-1244">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="e73ef-1245">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="e73ef-1245">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1246">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1246">VM</span></span>

* <span data-ttu-id="e73ef-1247">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1247">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="e73ef-1248">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1248">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="e73ef-1249">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕИЕ] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1249">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="e73ef-1250">Добавлена поддержка политики вытеснения для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1250">Added support for eviction policy to</span></span> `vmss`
* <span data-ttu-id="e73ef-1251">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1251">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="e73ef-1252">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1252">Added write accelerator support</span></span>
* <span data-ttu-id="e73ef-1253">Добавлено</span><span class="sxs-lookup"><span data-stu-id="e73ef-1253">Added</span></span> `vmss perform-maintenance`
* <span data-ttu-id="e73ef-1254">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1254">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="e73ef-1255">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1255">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="e73ef-1256">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1256">April 10, 2018</span></span>

<span data-ttu-id="e73ef-1257">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="e73ef-1257">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-1258">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-1258">ACR</span></span>

* <span data-ttu-id="e73ef-1259">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1259">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1260">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1260">ACS</span></span>

* <span data-ttu-id="e73ef-1261">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1261">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1262">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1262">Appservice</span></span>

* [<span data-ttu-id="e73ef-1263">КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1263">BREAKING CHANGE</span></span>]: Removed `assign-identity`
* <span data-ttu-id="e73ef-1264">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1264">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="e73ef-1265">Batch AI</span><span class="sxs-lookup"><span data-stu-id="e73ef-1265">BatchAI</span></span>

* <span data-ttu-id="e73ef-1266">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1266">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="e73ef-1267">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1267">Job level mounting</span></span>
  - <span data-ttu-id="e73ef-1268">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1268">Environment variables with secret values</span></span>
  - <span data-ttu-id="e73ef-1269">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="e73ef-1269">Performance counters settings</span></span>
  - <span data-ttu-id="e73ef-1270">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1270">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="e73ef-1271">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1271">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="e73ef-1272">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1272">Usage and limits reporting</span></span>
  - <span data-ttu-id="e73ef-1273">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1273">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="e73ef-1274">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1274">Support for custom images</span></span>
  - <span data-ttu-id="e73ef-1275">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1275">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="e73ef-1276">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1276">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="e73ef-1277">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1277">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="e73ef-1278">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1278">National clouds are supported</span></span>
* <span data-ttu-id="e73ef-1279">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1279">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="e73ef-1280">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1280">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="e73ef-1281">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1281">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="e73ef-1282">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1282">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="e73ef-1283">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1283">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="e73ef-1284">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1284">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="e73ef-1285">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1285">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="e73ef-1286">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1286">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="e73ef-1287">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1287">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="e73ef-1288">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1288">Added `--generate-ssh-keys` option to `cluster create` and</span></span> `file-server create`
* <span data-ttu-id="e73ef-1289">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1289">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="e73ef-1290">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1290">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="e73ef-1291">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1291">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="e73ef-1292">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="e73ef-1292">Billing</span></span>

* <span data-ttu-id="e73ef-1293">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1293">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="e73ef-1294">Потребление</span><span class="sxs-lookup"><span data-stu-id="e73ef-1294">Consumption</span></span>

* <span data-ttu-id="e73ef-1295">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1295">Added `marketplace` commands</span></span>
* <span data-ttu-id="e73ef-1296">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Команда `reservations summaries` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1296">[BREAKING CHANGE] Renamed `reservations summaries` to</span></span> `reservation summary`
* <span data-ttu-id="e73ef-1297">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Команда `reservations details` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1297">[BREAKING CHANGE] Renamed `reservations details` to</span></span> `reservation detail`
* <span data-ttu-id="e73ef-1298">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1298">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="e73ef-1299">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1299">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="e73ef-1300">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1300">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-1301">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1301">Container</span></span>

* <span data-ttu-id="e73ef-1302">Добавлены параметры подключения тома репозитория Git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1302">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and</span></span> `--gitrepo-mount-path`
* <span data-ttu-id="e73ef-1303">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1303">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="e73ef-1304">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1304">Extension</span></span>

* <span data-ttu-id="e73ef-1305">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1305">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="e73ef-1306">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-1306">Interactive</span></span>

* <span data-ttu-id="e73ef-1307">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1307">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="e73ef-1308">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1308">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="e73ef-1309">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1309">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1310">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1310">Network</span></span>

* <span data-ttu-id="e73ef-1311">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1311">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="e73ef-1312">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1312">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> [<span data-ttu-id="e73ef-1313">№ 4910</span><span class="sxs-lookup"><span data-stu-id="e73ef-1313">#4910</span></span>](https://github.com/Azure/azure-cli/issues/4910)
* <span data-ttu-id="e73ef-1314">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1314">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="e73ef-1315">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1315">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="e73ef-1316">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде</span><span class="sxs-lookup"><span data-stu-id="e73ef-1316">Fixed issue with `--disable-bgp-route-propagation` flag in</span></span> `network route-table [create|update]`
* <span data-ttu-id="e73ef-1317">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1317">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for</span></span> `network lb [create|update]`
* <span data-ttu-id="e73ef-1318">Добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035 в `network dns zone [import|export]` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1318">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and</span></span> `network dns record-set txt add-record`

### <a name="profile"></a><span data-ttu-id="e73ef-1319">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1319">Profile</span></span>

* <span data-ttu-id="e73ef-1320">Добавлена поддержка классических учетных записей Azure для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1320">Added support for Azure Classic accounts in</span></span> `account list`
* <span data-ttu-id="e73ef-1321">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1321">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="e73ef-1322">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="e73ef-1322">RDBMS</span></span>

* <span data-ttu-id="e73ef-1323">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1323">Added `georestore` command</span></span>
* <span data-ttu-id="e73ef-1324">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1324">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-1325">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-1325">Resource</span></span>

* <span data-ttu-id="e73ef-1326">Добавлена поддержка `--metadata` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1326">Added support for `--metadata` to</span></span> `policy definition create`
* <span data-ttu-id="e73ef-1327">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1327">Added support for `--metadata`, `--set`, `--add`, `--remove` to</span></span> `policy definition update`

### <a name="sql"></a><span data-ttu-id="e73ef-1328">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-1328">SQL</span></span>

* <span data-ttu-id="e73ef-1329">Добавлены команды `sql elastic-pool op list` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1329">Added `sql elastic-pool op list` and</span></span> `sql elastic-pool op cancel`

### <a name="storage"></a><span data-ttu-id="e73ef-1330">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1330">Storage</span></span>

* <span data-ttu-id="e73ef-1331">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1331">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1332">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1332">VM</span></span>

* <span data-ttu-id="e73ef-1333">Добавлена возможность настроить для платформы количество доменов сбоя в команде</span><span class="sxs-lookup"><span data-stu-id="e73ef-1333">Added support to configure platform fault domain count to</span></span> `vmss create`
* <span data-ttu-id="e73ef-1334">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1334">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [<span data-ttu-id="e73ef-1335">КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1335">BREAKING CHANGE</span></span>]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret`
* <span data-ttu-id="e73ef-1336">Добавлена поддержка номера SKU общедоступного IP-адреса для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1336">Added support for Public-IP SKU to</span></span> `vm create`
* <span data-ttu-id="e73ef-1337">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1337">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> [<span data-ttu-id="e73ef-1338">№ 5718</span><span class="sxs-lookup"><span data-stu-id="e73ef-1338">#5718</span></span>](https://github.com/Azure/azure-cli/issues/5718)
* <span data-ttu-id="e73ef-1339">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1339">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="e73ef-1340">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1340">March 27, 2018</span></span>

<span data-ttu-id="e73ef-1341">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="e73ef-1341">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1342">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1342">Core</span></span>

* <span data-ttu-id="e73ef-1343">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1343">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1344">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1344">ACS</span></span>

* <span data-ttu-id="e73ef-1345">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1345">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1346">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1346">Appservice</span></span>

* <span data-ttu-id="e73ef-1347">Добавлена поддержка только протокола HTTPS для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1347">Added HTTPS-only support to</span></span> `webapp update`
* <span data-ttu-id="e73ef-1348">Добавлена поддержка слотов для `az webapp identity [assign|show]` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1348">Added support for slots to `az webapp identity [assign|show]` and</span></span> `az functionapp identity [assign|show]`

### <a name="backup"></a><span data-ttu-id="e73ef-1349">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="e73ef-1349">Backup</span></span>

* <span data-ttu-id="e73ef-1350">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1350">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="e73ef-1351">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1351">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="e73ef-1352">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1352">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="e73ef-1353">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1353">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-1354">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1354">Container</span></span>

* <span data-ttu-id="e73ef-1355">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1355">Added `container exec` command.</span></span> <span data-ttu-id="e73ef-1356">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1356">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="e73ef-1357">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1357">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="e73ef-1358">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1358">Extension</span></span>

* <span data-ttu-id="e73ef-1359">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1359">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="e73ef-1360">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием</span><span class="sxs-lookup"><span data-stu-id="e73ef-1360">Changed `extension list-available` to show full extension data with</span></span> `--show-details`
* <span data-ttu-id="e73ef-1361">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1361">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="e73ef-1362">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-1362">Interactive</span></span>

* <span data-ttu-id="e73ef-1363">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1363">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="e73ef-1364">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1364">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="e73ef-1365">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1365">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="e73ef-1366">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1366">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="e73ef-1367">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="e73ef-1367">Lab</span></span>

* <span data-ttu-id="e73ef-1368">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1368">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-1369">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-1369">Monitor</span></span>

* <span data-ttu-id="e73ef-1370">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1370">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="e73ef-1371">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1371">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="e73ef-1372">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1372">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1373">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1373">Network</span></span>

* <span data-ttu-id="e73ef-1374">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1374">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="e73ef-1375">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1375">Profile</span></span>

* <span data-ttu-id="e73ef-1376">Добавлено предупреждение для `--identity-port` и `--msi-port` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1376">Added warning for `--identity-port` and `--msi-port` to</span></span> `login`

### <a name="rdbms"></a><span data-ttu-id="e73ef-1377">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="e73ef-1377">RDBMS</span></span>

* <span data-ttu-id="e73ef-1378">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1378">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-1379">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-1379">Resource</span></span>

* [<span data-ttu-id="e73ef-1380">КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1380">BREAKING CHANGE</span></span>]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="e73ef-1381">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1381">Role</span></span>

* <span data-ttu-id="e73ef-1382">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1382">Added support for required access configurations and native clients to</span></span> `az ad app create`
* <span data-ttu-id="e73ef-1383">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1383">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="e73ef-1384">Добавлены команды для управления учетными данными:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1384">Added credential management commands</span></span> `ad sp credential [reset|list|delete]`
* <span data-ttu-id="e73ef-1385">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1385">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="e73ef-1386">Добавлена поддержка разрешений `dataActions` и `notDataActions` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1386">Added support for `dataActions` and `notDataActions` permissions to</span></span> `role definition`

### <a name="storage"></a><span data-ttu-id="e73ef-1387">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1387">Storage</span></span>

* <span data-ttu-id="e73ef-1388">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1388">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="e73ef-1389">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1389">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1390">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1390">VM</span></span>

* <span data-ttu-id="e73ef-1391">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1391">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="e73ef-1392">Добавлена поддержка устойчивости зон для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1392">Added zone resilient support to</span></span> `vm [snapshot|image]`
* <span data-ttu-id="e73ef-1393">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1393">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="e73ef-1394">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1394">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="e73ef-1395">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1395">March 13, 2018</span></span>

<span data-ttu-id="e73ef-1396">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="e73ef-1396">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-1397">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-1397">ACR</span></span>

* <span data-ttu-id="e73ef-1398">Добавлена поддержка параметра `--image` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1398">Added support for `--image` parameter to</span></span> `repository delete`
* <span data-ttu-id="e73ef-1399">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1399">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="e73ef-1400">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1400">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1401">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1401">ACS</span></span>

* <span data-ttu-id="e73ef-1402">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1402">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="e73ef-1403">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1403">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="e73ef-1404">Помощник</span><span class="sxs-lookup"><span data-stu-id="e73ef-1404">Advisor</span></span>

* <span data-ttu-id="e73ef-1405">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Команда `advisor configuration get` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1405">[BREAKING CHANGE] Renamed `advisor configuration get` to</span></span> `advisor configuration list`
* <span data-ttu-id="e73ef-1406">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Команда `advisor configuration set` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1406">[BREAKING CHANGE] Renamed `advisor configuration set` to</span></span> `advisor configuration update`
* <span data-ttu-id="e73ef-1407">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Удалена команда</span><span class="sxs-lookup"><span data-stu-id="e73ef-1407">[BREAKING CHANGE] Removed</span></span> `advisor recommendation generate`
* <span data-ttu-id="e73ef-1408">Добавлен параметр `--refresh` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1408">Added `--refresh` parameter to</span></span> `advisor recommendation list`
* <span data-ttu-id="e73ef-1409">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1409">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1410">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1410">Appservice</span></span>

* <span data-ttu-id="e73ef-1411">Не рекомендуется</span><span class="sxs-lookup"><span data-stu-id="e73ef-1411">Deprecated</span></span> `[webapp|functionapp] assign-identity`
* <span data-ttu-id="e73ef-1412">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1412">Added managed identity commands `webapp identity [assign|show]` and</span></span> `functionapp identity [assign|show]`

### <a name="eventhubs"></a><span data-ttu-id="e73ef-1413">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="e73ef-1413">Eventhubs</span></span>

* <span data-ttu-id="e73ef-1414">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="e73ef-1414">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="e73ef-1415">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1415">Extension</span></span>

* <span data-ttu-id="e73ef-1416">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1416">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="e73ef-1417">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-1417">Interactive</span></span>

* <span data-ttu-id="e73ef-1418">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1418">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="e73ef-1419">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1419">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="e73ef-1420">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1420">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="e73ef-1421">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1421">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-1422">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-1422">Monitor</span></span>

* <span data-ttu-id="e73ef-1423">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1423">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="e73ef-1424">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1424">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="e73ef-1425">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1425">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="e73ef-1426">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1426">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1427">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1427">Network</span></span>

* <span data-ttu-id="e73ef-1428">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Удален параметр `--tags` из</span><span class="sxs-lookup"><span data-stu-id="e73ef-1428">[BREAKING CHANGE] Removed `--tags` parameter from</span></span>  `route-filter rule create`
* <span data-ttu-id="e73ef-1429">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1429">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="e73ef-1430">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1430">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="e73ef-1431">Добавлены параметры `--vnet` и `--subnet` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1431">Added `--vnet` and `--subnet` parameters to</span></span> `network watcher show-topology`

### <a name="profile"></a><span data-ttu-id="e73ef-1432">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1432">Profile</span></span>

* <span data-ttu-id="e73ef-1433">Больше не поддерживается параметр `--msi` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1433">Deprecated `--msi` parameter for</span></span> `az login`
* <span data-ttu-id="e73ef-1434">Добавлен параметр `--identity` для `az login`. Он заменяет</span><span class="sxs-lookup"><span data-stu-id="e73ef-1434">Added `--identity` parameter for `az login` to replace</span></span> `--msi`

### <a name="rdbms"></a><span data-ttu-id="e73ef-1435">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="e73ef-1435">RDBMS</span></span>

* <span data-ttu-id="e73ef-1436">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1436">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="e73ef-1437">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-1437">Service Bus</span></span>

* <span data-ttu-id="e73ef-1438">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="e73ef-1438">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-1439">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1439">Storage</span></span>

* <span data-ttu-id="e73ef-1440">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1440">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="e73ef-1441">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1441">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1442">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1442">VM</span></span>

* <span data-ttu-id="e73ef-1443">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1443">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="e73ef-1444">Больше не поддерживаются `[vm|vmss] assign-identity` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1444">Deprecated `[vm|vmss] assign-identity` and</span></span> `[vm|vmss] remove-identity`
* <span data-ttu-id="e73ef-1445">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1445">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="e73ef-1446">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1446">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="e73ef-1447">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="e73ef-1447">February 27, 2018</span></span>

<span data-ttu-id="e73ef-1448">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="e73ef-1448">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1449">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1449">Core</span></span>

* <span data-ttu-id="e73ef-1450">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1450">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="e73ef-1451">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1451">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="e73ef-1452">Добавлена функция ведения журнала HTTP в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1452">Added HTTP logging to</span></span> `--debug`

### <a name="acs"></a><span data-ttu-id="e73ef-1453">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1453">ACS</span></span>

* <span data-ttu-id="e73ef-1454">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1454">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="e73ef-1455">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1455">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="e73ef-1456">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1456">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to</span></span> `aks install-connector`
* <span data-ttu-id="e73ef-1457">Удалено уведомление об устаревании из</span><span class="sxs-lookup"><span data-stu-id="e73ef-1457">Removed deprecation notice from</span></span> `aks get-versions`

### <a name="appservice"></a><span data-ttu-id="e73ef-1458">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1458">Appservice</span></span>

* <span data-ttu-id="e73ef-1459">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="e73ef-1459">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="e73ef-1460">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1460">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="e73ef-1461">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="e73ef-1461">Cognitive Services</span></span>

* <span data-ttu-id="e73ef-1462">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1462">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="e73ef-1463">Потребление</span><span class="sxs-lookup"><span data-stu-id="e73ef-1463">Consumption</span></span>

* <span data-ttu-id="e73ef-1464">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1464">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="e73ef-1465">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1465">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-1466">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1466">Container</span></span>

* <span data-ttu-id="e73ef-1467">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1467">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1468">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1468">Network</span></span>

* <span data-ttu-id="e73ef-1469">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1469">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in</span></span> `network vnet-gateway vpn-client generate`

### <a name="resource"></a><span data-ttu-id="e73ef-1470">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-1470">Resource</span></span>

* <span data-ttu-id="e73ef-1471">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1471">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-1472">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1472">Role</span></span>

* <span data-ttu-id="e73ef-1473">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1473">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-1474">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-1474">SQL</span></span>

* <span data-ttu-id="e73ef-1475">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1475">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-1476">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1476">Storage</span></span>

* <span data-ttu-id="e73ef-1477">Включено определение пути назначения и префикса для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1477">Enabled specifying destination-path/prefix for</span></span> `storage blob [upload-batch|download-batch]`

### <a name="vm"></a><span data-ttu-id="e73ef-1478">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1478">VM</span></span>

* <span data-ttu-id="e73ef-1479">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1479">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="e73ef-1480">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1480">February 13, 2018</span></span>

<span data-ttu-id="e73ef-1481">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="e73ef-1481">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1482">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1482">Core</span></span>

* <span data-ttu-id="e73ef-1483">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1483">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1484">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1484">ACS</span></span>

* <span data-ttu-id="e73ef-1485">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1485">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="e73ef-1486">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1486">Changed `aks get-versions` to show Kubernetes versions available for</span></span> `aks create`
* <span data-ttu-id="e73ef-1487">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1487">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="e73ef-1488">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1488">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="e73ef-1489">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1489">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="e73ef-1490">Улучшена надежность при поиске панели мониторинга для группы pod для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1490">Improved reliability when locating the dashboard pod for</span></span> `az aks browse`
* <span data-ttu-id="e73ef-1491">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1491">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="e73ef-1492">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1492">Added a message to `az aks install-cli` to help get `kubectl` in</span></span> `$PATH`

### <a name="appservice"></a><span data-ttu-id="e73ef-1493">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1493">Appservice</span></span>

* <span data-ttu-id="e73ef-1494">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1494">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="e73ef-1495">Добавлена поддержка стандартных планов службы приложений с помощью</span><span class="sxs-lookup"><span data-stu-id="e73ef-1495">Added support for default app service plans through</span></span> `az configure --defaults appserviceplan=my-asp`

### <a name="cdn"></a><span data-ttu-id="e73ef-1496">CDN</span><span class="sxs-lookup"><span data-stu-id="e73ef-1496">CDN</span></span>

* <span data-ttu-id="e73ef-1497">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1497">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-1498">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1498">Container</span></span>

* <span data-ttu-id="e73ef-1499">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1499">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="e73ef-1500">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1500">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e73ef-1501">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e73ef-1501">CosmosDB</span></span>

* <span data-ttu-id="e73ef-1502">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1502">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="e73ef-1503">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1503">Extension</span></span>

* <span data-ttu-id="e73ef-1504">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1504">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="e73ef-1505">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1505">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="e73ef-1506">Отзыв</span><span class="sxs-lookup"><span data-stu-id="e73ef-1506">Feedback</span></span>

* <span data-ttu-id="e73ef-1507">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1507">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="e73ef-1508">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-1508">Interactive</span></span>

* <span data-ttu-id="e73ef-1509">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1509">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="e73ef-1510">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1510">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="e73ef-1511">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="e73ef-1511">IoT</span></span>

* <span data-ttu-id="e73ef-1512">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="e73ef-1512">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e73ef-1513">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="e73ef-1513">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="e73ef-1514">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1514">Added `--no-wait` support to `iot dps access policy [create|update]` and</span></span> `iot dps linked-hub [create|update]`
* <span data-ttu-id="e73ef-1515">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1515">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-1516">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-1516">Monitor</span></span>

* <span data-ttu-id="e73ef-1517">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1517">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1518">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1518">Network</span></span>

* <span data-ttu-id="e73ef-1519">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1519">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="e73ef-1520">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1520">Profile</span></span>

* <span data-ttu-id="e73ef-1521">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1521">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-1522">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-1522">Resource</span></span>

* <span data-ttu-id="e73ef-1523">Снова добавлена команда</span><span class="sxs-lookup"><span data-stu-id="e73ef-1523">Added back</span></span> `feature show`

### <a name="role"></a><span data-ttu-id="e73ef-1524">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1524">Role</span></span>

* <span data-ttu-id="e73ef-1525">Добавлен аргумент `--available-to-other-tenants` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1525">Added `--available-to-other-tenants` argument to</span></span> `ad app update`

### <a name="sql"></a><span data-ttu-id="e73ef-1526">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-1526">SQL</span></span>

* <span data-ttu-id="e73ef-1527">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1527">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="e73ef-1528">Добавлено</span><span class="sxs-lookup"><span data-stu-id="e73ef-1528">Added</span></span> `sql db rename`
* <span data-ttu-id="e73ef-1529">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1529">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-1530">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1530">Storage</span></span>

* <span data-ttu-id="e73ef-1531">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1531">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1532">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1532">VM</span></span>

* <span data-ttu-id="e73ef-1533">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1533">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="e73ef-1534">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1534">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="e73ef-1535">исправление</span><span class="sxs-lookup"><span data-stu-id="e73ef-1535">Fixed</span></span> `vm boot-diagnostics get-boot-log`


## <a name="january-31-2018"></a><span data-ttu-id="e73ef-1536">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1536">January 31, 2018</span></span>

<span data-ttu-id="e73ef-1537">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="e73ef-1537">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1538">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1538">Core</span></span>

* <span data-ttu-id="e73ef-1539">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1539">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="e73ef-1540">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1540">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="e73ef-1541">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1541">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="e73ef-1542">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1542">Use `--verbose` to see</span></span>
* <span data-ttu-id="e73ef-1543">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1543">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1544">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1544">ACS</span></span>

* <span data-ttu-id="e73ef-1545">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1545">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="e73ef-1546">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1546">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1547">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1547">Appservice</span></span>

* <span data-ttu-id="e73ef-1548">исправление</span><span class="sxs-lookup"><span data-stu-id="e73ef-1548">Fixed</span></span> `webapp log [tail|download]`
* <span data-ttu-id="e73ef-1549">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1549">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="e73ef-1550">CDN</span><span class="sxs-lookup"><span data-stu-id="e73ef-1550">CDN</span></span>

* <span data-ttu-id="e73ef-1551">Устранена проблема с отсутствием клиента для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1551">Fixed missing client issue with</span></span> `cdn custom-domain create`

### <a name="cosmosdb"></a><span data-ttu-id="e73ef-1552">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e73ef-1552">CosmosDB</span></span>

* <span data-ttu-id="e73ef-1553">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1553">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="e73ef-1554">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-1554">Interactive</span></span>

* <span data-ttu-id="e73ef-1555">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1555">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1556">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1556">Network</span></span>

* <span data-ttu-id="e73ef-1557">Добавлена защита `--cert-password` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1557">Added protection for `--cert-password` to</span></span> `application-gateway create`
* <span data-ttu-id="e73ef-1558">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1558">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="e73ef-1559">Добавлена защита `--shared-key` и `--authorization-key` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1559">Added protection for `--shared-key` and `--authorization-key` to</span></span> `vpn-connection create`
* <span data-ttu-id="e73ef-1560">Устранена проблема с отсутствием клиента для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1560">Fixed missing client issue with</span></span> `asg create`
* <span data-ttu-id="e73ef-1561">Добавлен параметр `--file-name / -f` для экспортируемых имен в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1561">Added `--file-name / -f` parameter for exported names to</span></span> `dns zone export`
* <span data-ttu-id="e73ef-1562">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1562">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="e73ef-1563">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1563">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="e73ef-1564">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1564">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="e73ef-1565">Исправлена проблема, когда некоторые записи импортировались дважды с помощью</span><span class="sxs-lookup"><span data-stu-id="e73ef-1565">Fixed issue where certain records were imported twice with</span></span> `dns zone import`
* <span data-ttu-id="e73ef-1566">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1566">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="e73ef-1567">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1567">Profile</span></span>

* <span data-ttu-id="e73ef-1568">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1568">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-1569">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-1569">Resource</span></span>

* <span data-ttu-id="e73ef-1570">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1570">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-1571">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1571">Storage</span></span>

* <span data-ttu-id="e73ef-1572">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1572">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="e73ef-1573">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1573">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="e73ef-1574">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с</span><span class="sxs-lookup"><span data-stu-id="e73ef-1574">Fixed bug preventing "-n" arg option with</span></span> `storage account check-name`
* <span data-ttu-id="e73ef-1575">Добавлен столбец snapshot в табличные выходные данные для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1575">Added 'snapshot' column to table output for</span></span> `blob [list|show]`
* <span data-ttu-id="e73ef-1576">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1576">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1577">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1577">VM</span></span>

* <span data-ttu-id="e73ef-1578">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1578">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="e73ef-1579">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1579">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="e73ef-1580">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1580">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="e73ef-1581">Добавлена защита `--admin-password` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1581">Added protection for `--admin-password` to</span></span> `[vm|vmss] create`


## <a name="january-17-2018"></a><span data-ttu-id="e73ef-1582">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1582">January 17, 2018</span></span>

<span data-ttu-id="e73ef-1583">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="e73ef-1583">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-1584">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-1584">ACR</span></span>

* <span data-ttu-id="e73ef-1585">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1585">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="e73ef-1586">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1586">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1587">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1587">ACS</span></span>

* <span data-ttu-id="e73ef-1588">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1588">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="e73ef-1589">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1589">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1590">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1590">Appservice</span></span>

* <span data-ttu-id="e73ef-1591">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1591">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="e73ef-1592">Добавлена поддержка для пользовательских URL-адресов в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1592">Added support for custom URLs to</span></span> `browse`
* <span data-ttu-id="e73ef-1593">Исправлена поддержка слотов для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1593">Fixed slot support for</span></span> `log tail`

### <a name="backup"></a><span data-ttu-id="e73ef-1594">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="e73ef-1594">Backup</span></span>

* <span data-ttu-id="e73ef-1595">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1595">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="e73ef-1596">Добавлены варианты учетной записи хранения в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1596">Added storage account options to</span></span> `backup restore restore-disks`
* <span data-ttu-id="e73ef-1597">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1597">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="e73ef-1598">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1598">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="e73ef-1599">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1599">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="e73ef-1600">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-1600">Batch</span></span>

* <span data-ttu-id="e73ef-1601">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1601">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="e73ef-1602">Облако</span><span class="sxs-lookup"><span data-stu-id="e73ef-1602">Cloud</span></span>

* <span data-ttu-id="e73ef-1603">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1603">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="e73ef-1604">Потребление</span><span class="sxs-lookup"><span data-stu-id="e73ef-1604">Consumption</span></span>

* <span data-ttu-id="e73ef-1605">Добавлены новые команды для резервирования: `consumption reservations summaries` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1605">Added new commands for reservations: `consumption reservations summaries` and</span></span> `consumption reservations details`

### <a name="event-grid"></a><span data-ttu-id="e73ef-1606">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-1606">Event Grid</span></span>

* <span data-ttu-id="e73ef-1607">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Команды `az eventgrid topic event-subscription` перемещены в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1607">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to</span></span> `eventgrid event-subscription`
* <span data-ttu-id="e73ef-1608">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Команды `az eventgrid resource event-subscription` перемещены в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1608">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to</span></span> `eventgrid event-subscription`
* <span data-ttu-id="e73ef-1609">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1609">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="e73ef-1610">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1610">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="e73ef-1611">Добавлена команда</span><span class="sxs-lookup"><span data-stu-id="e73ef-1611">Added command</span></span> `eventgrid topic update`
* <span data-ttu-id="e73ef-1612">Добавлена команда</span><span class="sxs-lookup"><span data-stu-id="e73ef-1612">Added command</span></span> `eventgrid event-subscription update`
* <span data-ttu-id="e73ef-1613">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1613">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="e73ef-1614">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1614">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="e73ef-1615">Interactive</span><span class="sxs-lookup"><span data-stu-id="e73ef-1615">Interactive</span></span>

* <span data-ttu-id="e73ef-1616">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1616">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="e73ef-1617">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1617">Fixed errors on startup</span></span>
* <span data-ttu-id="e73ef-1618">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1618">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="e73ef-1619">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="e73ef-1619">IoT</span></span>

* <span data-ttu-id="e73ef-1620">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1620">Added support for device provisioning service</span></span>
* <span data-ttu-id="e73ef-1621">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1621">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="e73ef-1622">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1622">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-1623">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-1623">Monitor</span></span>

* <span data-ttu-id="e73ef-1624">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1624">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="e73ef-1625">Теперь параметр `--name` является обязательным для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1625">The `--name` parameter is now required for</span></span> `az monitor diagnostic-settings create`
* <span data-ttu-id="e73ef-1626">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1626">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1627">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1627">Network</span></span>

* <span data-ttu-id="e73ef-1628">Устранена проблема при попытке входа в активный режим и режим ожидания или выхода из них, связанная с</span><span class="sxs-lookup"><span data-stu-id="e73ef-1628">Fixed issue when trying to change to/from active-standby mode with</span></span> `vnet-gateway update`
* <span data-ttu-id="e73ef-1629">Добавлена поддержка HTTP2 в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1629">Added support for HTTP2 to</span></span> `application-gateway [create|update]`

### <a name="profile"></a><span data-ttu-id="e73ef-1630">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1630">Profile</span></span>

* <span data-ttu-id="e73ef-1631">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1631">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-1632">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1632">Role</span></span>

* <span data-ttu-id="e73ef-1633">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1633">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e73ef-1634">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e73ef-1634">Service Fabric</span></span>

* <span data-ttu-id="e73ef-1635">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1635">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="e73ef-1636">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1636">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1637">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1637">VM</span></span>

* <span data-ttu-id="e73ef-1638">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1638">[PREVIEW] Cross-zone support for</span></span> `vmss`
* <span data-ttu-id="e73ef-1639">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="e73ef-1639">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="e73ef-1640">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1640">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="e73ef-1641">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1641">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="e73ef-1642">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1642">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="e73ef-1643">Добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1643">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to</span></span> `[vm|vmss] create`
* <span data-ttu-id="e73ef-1644">Устранены проблемы с</span><span class="sxs-lookup"><span data-stu-id="e73ef-1644">Fixed error issues with</span></span> `[vm|vmss] create`
* <span data-ttu-id="e73ef-1645">Устранена проблема чрезмерного использования ресурсов из-за</span><span class="sxs-lookup"><span data-stu-id="e73ef-1645">Fixed excessive resource usage caused by</span></span> `vm image list --all`

## <a name="december-19-2017"></a><span data-ttu-id="e73ef-1646">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1646">December 19, 2017</span></span>

<span data-ttu-id="e73ef-1647">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="e73ef-1647">Version 2.0.23</span></span>

* <span data-ttu-id="e73ef-1648">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1648">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-1649">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1649">Container</span></span>

* <span data-ttu-id="e73ef-1650">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1650">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1651">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1651">Network</span></span>

* <span data-ttu-id="e73ef-1652">Добавлен аргумент `--disable-bgp-route-propagation` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1652">Added `--disable-bgp-route-propagation` argument to</span></span> `route-table [create|update]`
* <span data-ttu-id="e73ef-1653">Добавлен аргумент `--ip-tags` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1653">Added `--ip-tags` argument to</span></span> `public-ip [create|update]`

### <a name="storage"></a><span data-ttu-id="e73ef-1654">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1654">Storage</span></span>

* <span data-ttu-id="e73ef-1655">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1655">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1656">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1656">VM</span></span>

* <span data-ttu-id="e73ef-1657">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1657">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="e73ef-1658">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1658">December 5, 2017</span></span>

<span data-ttu-id="e73ef-1659">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="e73ef-1659">Version 2.0.22</span></span>

* <span data-ttu-id="e73ef-1660">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1660">Removed `az component` commands.</span></span> <span data-ttu-id="e73ef-1661">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1661">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1662">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1662">Core</span></span>
* <span data-ttu-id="e73ef-1663">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1663">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="e73ef-1664">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1664">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1665">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1665">ACS</span></span>

* <span data-ttu-id="e73ef-1666">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1666">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="e73ef-1667">Улучшены сообщения об ошибках для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1667">Improved error reporting for</span></span> `acs create`
* <span data-ttu-id="e73ef-1668">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1668">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="e73ef-1669">Помощник</span><span class="sxs-lookup"><span data-stu-id="e73ef-1669">Advisor</span></span>

* <span data-ttu-id="e73ef-1670">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="e73ef-1670">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1671">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1671">Appservice</span></span>

* <span data-ttu-id="e73ef-1672">Добавлена возможность создания имени сертификата с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1672">Fixed cert name generation with</span></span> `webapp config ssl upload`
* <span data-ttu-id="e73ef-1673">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1673">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="e73ef-1674">Добавлено значение по умолчанию для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1674">Added default value for</span></span> `WEBSITE_NODE_DEFAULT_VERSION`

### <a name="consumption"></a><span data-ttu-id="e73ef-1675">Потребление</span><span class="sxs-lookup"><span data-stu-id="e73ef-1675">Consumption</span></span>

* <span data-ttu-id="e73ef-1676">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1676">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-1677">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1677">Container</span></span>

* <span data-ttu-id="e73ef-1678">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1678">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-1679">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-1679">Monitor</span></span>

* <span data-ttu-id="e73ef-1680">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1680">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-1681">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-1681">Resource</span></span>

* <span data-ttu-id="e73ef-1682">Добавлен аргумент `--include-response-body` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1682">Added `--include-response-body` argument to</span></span> `resource show`

### <a name="role"></a><span data-ttu-id="e73ef-1683">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1683">Role</span></span>

* <span data-ttu-id="e73ef-1684">Добавлено отображение стандартных назначений "классических" администраторов для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1684">Added display of default assignments for "classic" administraors to</span></span> `role assignment list`
* <span data-ttu-id="e73ef-1685">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1685">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="e73ef-1686">Улучшены сообщения об ошибках для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1686">Improved error reporting for</span></span> `ad sp create-for-rbac`

### <a name="sql"></a><span data-ttu-id="e73ef-1687">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-1687">SQL</span></span>

* <span data-ttu-id="e73ef-1688">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1688">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="e73ef-1689">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1689">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1690">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1690">VM</span></span>

* <span data-ttu-id="e73ef-1691">Добавлены сведения о зонах для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1691">Added zone information to</span></span> `az vm list-skus`


## <a name="november-14-2017"></a><span data-ttu-id="e73ef-1692">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1692">November 14, 2017</span></span>

<span data-ttu-id="e73ef-1693">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="e73ef-1693">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-1694">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-1694">ACR</span></span>

* <span data-ttu-id="e73ef-1695">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1695">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="e73ef-1696">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1696">ACS</span></span>

* <span data-ttu-id="e73ef-1697">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1697">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="e73ef-1698">Больше не поддерживается параметр `--orchestrator-release` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1698">Deprecated `--orchestrator-release` option for</span></span> `acs create`
* <span data-ttu-id="e73ef-1699">Изменен размер виртуальной машины по умолчанию для AKS на</span><span class="sxs-lookup"><span data-stu-id="e73ef-1699">Changed default VM size for AKS to</span></span> `Standard_D1_v2`
* <span data-ttu-id="e73ef-1700">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1700">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="e73ef-1701">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1701">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1702">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1702">Appservice</span></span>

* <span data-ttu-id="e73ef-1703">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1703">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="e73ef-1704">Добавлен параметр `--docker-container-logging` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1704">Added `--docker-container-logging` option to</span></span> `az webapp log config`
* <span data-ttu-id="e73ef-1705">Удален параметр `storage` из параметра `--web-server-logging` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1705">Removed the `storage` option from the parameter `--web-server-logging` of</span></span> `az webapp log config`
* <span data-ttu-id="e73ef-1706">Улучшены сообщения об ошибках для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1706">Improved error messages for</span></span> `deployment user set`
* <span data-ttu-id="e73ef-1707">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="e73ef-1707">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="e73ef-1708">исправление</span><span class="sxs-lookup"><span data-stu-id="e73ef-1708">Fixed</span></span> `list-locations`

### <a name="batch"></a><span data-ttu-id="e73ef-1709">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-1709">Batch</span></span>

* <span data-ttu-id="e73ef-1710">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1710">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="e73ef-1711">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="e73ef-1711">Batchai</span></span>

* <span data-ttu-id="e73ef-1712">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1712">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="e73ef-1713">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1713">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="e73ef-1714">Исправлена документация по командам `job list-files` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1714">Fixed documentation for `job list-files` and</span></span> `job stream-file`
* <span data-ttu-id="e73ef-1715">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1715">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="e73ef-1716">Облако</span><span class="sxs-lookup"><span data-stu-id="e73ef-1716">Cloud</span></span>

* <span data-ttu-id="e73ef-1717">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1717">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-1718">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1718">Container</span></span>

* <span data-ttu-id="e73ef-1719">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1719">Added support to open multiple ports</span></span>
* <span data-ttu-id="e73ef-1720">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1720">Added container group restart policy</span></span>
* <span data-ttu-id="e73ef-1721">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1721">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="e73ef-1722">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1722">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e73ef-1723">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e73ef-1723">Data Lake Analytics</span></span>

* <span data-ttu-id="e73ef-1724">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1724">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e73ef-1725">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e73ef-1725">Data Lake Store</span></span>

* <span data-ttu-id="e73ef-1726">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1726">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="e73ef-1727">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1727">Extension</span></span>

* <span data-ttu-id="e73ef-1728">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1728">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="e73ef-1729">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1729">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="e73ef-1730">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="e73ef-1730">IoT</span></span>

* <span data-ttu-id="e73ef-1731">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1731">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-1732">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-1732">Monitor</span></span>

* <span data-ttu-id="e73ef-1733">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1733">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1734">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1734">Network</span></span>

* <span data-ttu-id="e73ef-1735">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1735">Added support for CAA DNS records</span></span>
* <span data-ttu-id="e73ef-1736">Исправлена проблема, из-за которой конечные точки нельзя было обновить с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1736">Fixed issue where endpoints could not be updated with</span></span> `traffic-manager profile update`
* <span data-ttu-id="e73ef-1737">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1737">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="e73ef-1738">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1738">Fixed issue where relative DNS names were incorrectly imported by</span></span> `dns zone import`

### <a name="reservations"></a><span data-ttu-id="e73ef-1739">Резервирование</span><span class="sxs-lookup"><span data-stu-id="e73ef-1739">Reservations</span></span>

* <span data-ttu-id="e73ef-1740">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="e73ef-1740">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-1741">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-1741">Resource</span></span>

* <span data-ttu-id="e73ef-1742">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1742">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-1743">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-1743">SQL</span></span>

* <span data-ttu-id="e73ef-1744">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1744">Added `--ignore-missing-vnet-service-endpoint` parameter to</span></span> `sql server vnet-rule [create|update]`

### <a name="storage"></a><span data-ttu-id="e73ef-1745">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1745">Storage</span></span>

* <span data-ttu-id="e73ef-1746">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1746">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="e73ef-1747">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1747">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="e73ef-1748">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой</span><span class="sxs-lookup"><span data-stu-id="e73ef-1748">Fixed bug that prevented using `--source-uri` with</span></span> `storage [blob|file] copy start-batch`
* <span data-ttu-id="e73ef-1749">Добавлены команды для создания стандартных масок и удаления нескольких объектов с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1749">Added commands to glob and delete multiple objects with</span></span> `storage [blob|file] delete-batch`
* <span data-ttu-id="e73ef-1750">Исправлена проблема с включением метрик с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1750">Fixed issue when enabling metrics with</span></span> `storage metrics update`
* <span data-ttu-id="e73ef-1751">Исправлена проблема с файлами размером более 200 ГБ при использовании команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1751">Fixed issue with files over 200GB when using</span></span> `storage blob upload-batch`
* <span data-ttu-id="e73ef-1752">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой</span><span class="sxs-lookup"><span data-stu-id="e73ef-1752">Fixed issue where `--bypass` and `--default-action` were ignored by</span></span> `storage account [create|update]`

### <a name="vm"></a><span data-ttu-id="e73ef-1753">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1753">VM</span></span>

* <span data-ttu-id="e73ef-1754">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1754">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="e73ef-1755">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1755">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="e73ef-1756">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1756">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="e73ef-1757">Команда `vm format-secret` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1757">Renamed `vm format-secret` to</span></span> `vm secret format`
* <span data-ttu-id="e73ef-1758">Добавлен аргумент `--encrypt format` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1758">Added `--encrypt format` argument to</span></span> `vm encryption enable`

## <a name="october-24-2017"></a><span data-ttu-id="e73ef-1759">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1759">October 24, 2017</span></span>

<span data-ttu-id="e73ef-1760">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="e73ef-1760">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1761">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1761">Core</span></span>

* <span data-ttu-id="e73ef-1762">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии</span><span class="sxs-lookup"><span data-stu-id="e73ef-1762">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version</span></span> `2016-01-01`

### <a name="acr"></a><span data-ttu-id="e73ef-1763">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-1763">ACR</span></span>

* <span data-ttu-id="e73ef-1764">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="e73ef-1764">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="e73ef-1765">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="e73ef-1765">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="e73ef-1766">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="e73ef-1766">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1767">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1767">ACS</span></span>

* <span data-ttu-id="e73ef-1768">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="e73ef-1768">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="e73ef-1769">Исправление для Kubernetes:</span><span class="sxs-lookup"><span data-stu-id="e73ef-1769">Fixed kubernetes</span></span> `get-credentials`

### <a name="appservice"></a><span data-ttu-id="e73ef-1770">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1770">Appservice</span></span>

* <span data-ttu-id="e73ef-1771">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="e73ef-1771">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="e73ef-1772">Компонент</span><span class="sxs-lookup"><span data-stu-id="e73ef-1772">Component</span></span>

* <span data-ttu-id="e73ef-1773">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="e73ef-1773">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-1774">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-1774">Monitor</span></span>

* <span data-ttu-id="e73ef-1775">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1775">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-1776">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-1776">Resource</span></span>

* <span data-ttu-id="e73ef-1777">Исправление несовместимости с самой последней версией зависимости msrest в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1777">Fixed incompatibility with most recent version of msrest dependency in</span></span> `group export`
* <span data-ttu-id="e73ef-1778">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="e73ef-1778">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1779">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1779">VM</span></span>

* <span data-ttu-id="e73ef-1780">Добавлен аргумент `--accelerated-networking` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1780">Added `--accelerated-networking` argument to</span></span> `vmss create`


## <a name="october-9-2017"></a><span data-ttu-id="e73ef-1781">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1781">October 9, 2017</span></span>

<span data-ttu-id="e73ef-1782">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="e73ef-1782">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1783">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1783">Core</span></span>

* <span data-ttu-id="e73ef-1784">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1784">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1785">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1785">Appservice</span></span>

* <span data-ttu-id="e73ef-1786">Добавлена возможность общего обновления с помощью новой команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1786">Added generic update with new command</span></span> `webapp update`

### <a name="batch"></a><span data-ttu-id="e73ef-1787">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-1787">Batch</span></span>

* <span data-ttu-id="e73ef-1788">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="e73ef-1788">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="e73ef-1789">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1789">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="e73ef-1790">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1790">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="e73ef-1791">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1791">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="e73ef-1792">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="e73ef-1792">Batchai</span></span>

* <span data-ttu-id="e73ef-1793">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="e73ef-1793">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="e73ef-1794">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="e73ef-1794">Keyvault</span></span>

* <span data-ttu-id="e73ef-1795">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1795">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="e73ef-1796">№ 4448</span><span class="sxs-lookup"><span data-stu-id="e73ef-1796">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="e73ef-1797">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1797">Network</span></span>

* <span data-ttu-id="e73ef-1798">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1798">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="e73ef-1799">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1799">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-1800">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-1800">Resource</span></span>

* <span data-ttu-id="e73ef-1801">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на</span><span class="sxs-lookup"><span data-stu-id="e73ef-1801">Added support for `--resource-group/-g` options for resource group name to</span></span> `group`
* <span data-ttu-id="e73ef-1802">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1802">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="e73ef-1803">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1803">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="e73ef-1804">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1804">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-1805">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-1805">Sql</span></span>

* <span data-ttu-id="e73ef-1806">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1806">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="e73ef-1807">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1807">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="e73ef-1808">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1808">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-1809">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1809">Storage</span></span>

* <span data-ttu-id="e73ef-1810">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1810">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1811">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="e73ef-1811">Vm</span></span>

* <span data-ttu-id="e73ef-1812">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1812">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="e73ef-1813">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1813">[PREVIEW] Added support for rolling upgrade to</span></span> `vmss create`
* <span data-ttu-id="e73ef-1814">Добавлена поддержка обновления параметров шифрования с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1814">Added support for updating encryption settings with</span></span> `vm encryption enable`
* <span data-ttu-id="e73ef-1815">Добавлен параметр `--os-disk-size-gb` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1815">Added `--os-disk-size-gb` parameter to</span></span> `vm create`
* <span data-ttu-id="e73ef-1816">Добавлен параметр `--license-type` для Windows для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1816">Added `--license-type` parameter for Windows to</span></span> `vmss create`


## <a name="september-22-2017"></a><span data-ttu-id="e73ef-1817">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1817">September 22, 2017</span></span>

<span data-ttu-id="e73ef-1818">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="e73ef-1818">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-1819">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-1819">Resource</span></span>

* <span data-ttu-id="e73ef-1820">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="e73ef-1820">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="e73ef-1821">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="e73ef-1821">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="e73ef-1822">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1822">Added support for UI definitions and templates to</span></span> `managedapp definition create`
* <span data-ttu-id="e73ef-1823">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на</span><span class="sxs-lookup"><span data-stu-id="e73ef-1823">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to</span></span> `applicationDefinitions`

### <a name="network"></a><span data-ttu-id="e73ef-1824">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1824">Network</span></span>

* <span data-ttu-id="e73ef-1825">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="e73ef-1825">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="e73ef-1826">Добавлена поддержка IPv6 (пиринг Майкрософт) для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1826">Added support for IPv6 Microsoft Peering to</span></span> `express-route`
* <span data-ttu-id="e73ef-1827">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="e73ef-1827">Added `asg` application security group commands</span></span>
* <span data-ttu-id="e73ef-1828">Добавлен аргумент `--application-security-groups` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1828">Added `--application-security-groups` argument to</span></span> `nic [create|ip-config create|ip-config update]`
* <span data-ttu-id="e73ef-1829">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1829">Added `--source-asgs` and `--destination-asgs` arguments to</span></span> `nsg rule [create|update]`
* <span data-ttu-id="e73ef-1830">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1830">Added `--ddos-protection` and `--vm-protection` arguments to</span></span> `vnet [create|update]`
* <span data-ttu-id="e73ef-1831">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1831">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-1832">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1832">Storage</span></span>

* <span data-ttu-id="e73ef-1833">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="e73ef-1833">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="e73ef-1834">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="e73ef-1834">Eventgrid</span></span>

* <span data-ttu-id="e73ef-1835">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="e73ef-1835">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-1836">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-1836">SQL</span></span>

* <span data-ttu-id="e73ef-1837">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1837">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="e73ef-1838">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="e73ef-1838">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="e73ef-1839">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1839">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and</span></span> `dw [create|update]`

### <a name="keyvault"></a><span data-ttu-id="e73ef-1840">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="e73ef-1840">Keyvault</span></span>

* <span data-ttu-id="e73ef-1841">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="e73ef-1841">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1842">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1842">VM</span></span>

* <span data-ttu-id="e73ef-1843">Добавлена поддержка зоны доступности для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1843">Added for support to availability zone to</span></span> `[vm|vmss|disk] create`
* <span data-ttu-id="e73ef-1844">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="e73ef-1844">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="e73ef-1845">Добавлен аргумент `--asgs` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1845">Added `--asgs` argument to</span></span> `vm create`
* <span data-ttu-id="e73ef-1846">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1846">Added support for running commands on VMs with</span></span> `vm run-command`
* <span data-ttu-id="e73ef-1847">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1847">[PREVIEW] Added support for VMSS disk encryption with</span></span> `vmss encryption`
* <span data-ttu-id="e73ef-1848">Добавлена поддержка обслуживания виртуальных машин с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1848">Added support for performing maintenance on VMs with</span></span> `vm perform-maintenance`

### <a name="acs"></a><span data-ttu-id="e73ef-1849">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1849">ACS</span></span>

* <span data-ttu-id="e73ef-1850">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="e73ef-1850">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1851">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1851">Appservice</span></span>

* <span data-ttu-id="e73ef-1852">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1852">Added ability to update and show authentication settings with</span></span> `webapp auth [update|show]`

### <a name="backup"></a><span data-ttu-id="e73ef-1853">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="e73ef-1853">Backup</span></span>

* <span data-ttu-id="e73ef-1854">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1854">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="e73ef-1855">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1855">September 11, 2017</span></span>

<span data-ttu-id="e73ef-1856">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="e73ef-1856">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="e73ef-1857">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1857">Core</span></span>

* <span data-ttu-id="e73ef-1858">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1858">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="e73ef-1859">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1859">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1860">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1860">Acs</span></span>

* <span data-ttu-id="e73ef-1861">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1861">Added `acs list-locations` command</span></span>
* <span data-ttu-id="e73ef-1862">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1862">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1863">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1863">Appservice</span></span>

* <span data-ttu-id="e73ef-1864">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1864">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="e73ef-1865">CDN</span><span class="sxs-lookup"><span data-stu-id="e73ef-1865">CDN</span></span>

* <span data-ttu-id="e73ef-1866">Исправлена ошибка CustomDomain is not interable (CustomDomain не пригоден к итерации) для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1866">Fixed 'CustomDomain is not interable' bug for</span></span> `cdn custom-domain create`

### <a name="extension"></a><span data-ttu-id="e73ef-1867">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1867">Extension</span></span>

* <span data-ttu-id="e73ef-1868">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="e73ef-1868">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="e73ef-1869">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="e73ef-1869">Keyvault</span></span>

* <span data-ttu-id="e73ef-1870">Исправлена проблема с зависимостью разрешений от регистра для</span><span class="sxs-lookup"><span data-stu-id="e73ef-1870">Fixed issue where permissions were case sensitive for</span></span> `keyvault set-policy`

### <a name="network"></a><span data-ttu-id="e73ef-1871">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1871">Network</span></span>

* <span data-ttu-id="e73ef-1872">Команда `vnet list-private-access-services` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1872">Renamed `vnet list-private-access-services` to</span></span> `vnet list-endpoint-services`
* <span data-ttu-id="e73ef-1873">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1873">Renamed `--private-access-services` argument to `--service-endpoints` for</span></span> `vnet subnet create/update`
* <span data-ttu-id="e73ef-1874">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах</span><span class="sxs-lookup"><span data-stu-id="e73ef-1874">Added support for multiple IP ranges and port ranges to</span></span> `nsg rule create/update`
* <span data-ttu-id="e73ef-1875">Добавлена поддержка номера SKU в команде</span><span class="sxs-lookup"><span data-stu-id="e73ef-1875">Added support for SKU to</span></span> `lb create`
* <span data-ttu-id="e73ef-1876">Добавлена поддержка номера SKU в команде</span><span class="sxs-lookup"><span data-stu-id="e73ef-1876">Added support for SKU to</span></span> `public-ip create`

### <a name="resource"></a><span data-ttu-id="e73ef-1877">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-1877">Resource</span></span>

* <span data-ttu-id="e73ef-1878">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-1878">Allow passing in resource policy parameter definitions in `policy definition create`, and</span></span> `policy definition update`
* <span data-ttu-id="e73ef-1879">Разрешена передача значений параметров для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-1879">Allow passing in parameter values for</span></span> `policy assignment create`
* <span data-ttu-id="e73ef-1880">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1880">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="e73ef-1881">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1881">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-1882">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-1882">SQL</span></span>

* <span data-ttu-id="e73ef-1883">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1883">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1884">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1884">VM</span></span>

* <span data-ttu-id="e73ef-1885">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1885">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="e73ef-1886">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1886">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="e73ef-1887">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1887">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="e73ef-1888">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1888">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="e73ef-1889">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1889">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="e73ef-1890">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1890">August 31, 2017</span></span>

<span data-ttu-id="e73ef-1891">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="e73ef-1891">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="e73ef-1892">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="e73ef-1892">Keyvault</span></span>

* <span data-ttu-id="e73ef-1893">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью</span><span class="sxs-lookup"><span data-stu-id="e73ef-1893">Fixed bug when trying to automatically resolve secret encoding with</span></span> `secret download`

### <a name="sf"></a><span data-ttu-id="e73ef-1894">Sf</span><span class="sxs-lookup"><span data-stu-id="e73ef-1894">Sf</span></span>

* <span data-ttu-id="e73ef-1895">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1895">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-1896">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1896">Storage</span></span>

* <span data-ttu-id="e73ef-1897">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1897">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="e73ef-1898">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1898">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="e73ef-1899">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1899">August 28, 2017</span></span>

<span data-ttu-id="e73ef-1900">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="e73ef-1900">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="e73ef-1901">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="e73ef-1901">CLI</span></span>

* <span data-ttu-id="e73ef-1902">Добавлено юридическое примечание в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1902">Added legal note to</span></span> `--version`

### <a name="acs"></a><span data-ttu-id="e73ef-1903">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1903">ACS</span></span>

* <span data-ttu-id="e73ef-1904">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1904">Corrected preview regions</span></span>
* <span data-ttu-id="e73ef-1905">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1905">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="e73ef-1906">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1906">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1907">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1907">Appservice</span></span>

* <span data-ttu-id="e73ef-1908">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Исправлены несоответствия в выходных данных</span><span class="sxs-lookup"><span data-stu-id="e73ef-1908">[BREAKING CHANGE] Fixed inconsistencies in the output of</span></span> `az webapp config appsettings [delete|set]`
* <span data-ttu-id="e73ef-1909">Добавлен новый псевдоним `-i` в команду</span><span class="sxs-lookup"><span data-stu-id="e73ef-1909">Added a new alias of `-i` for</span></span> `az webapp config container set --docker-custom-image-name`
* <span data-ttu-id="e73ef-1910">Предоставлено</span><span class="sxs-lookup"><span data-stu-id="e73ef-1910">Exposed</span></span> `az webapp log show`
* <span data-ttu-id="e73ef-1911">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1911">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="e73ef-1912">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1912">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="e73ef-1913">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="e73ef-1913">IoT</span></span>

* <span data-ttu-id="e73ef-1914">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1914">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1915">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1915">Network</span></span>

* <span data-ttu-id="e73ef-1916">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Команда `vnet list-private-access-services` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1916">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to</span></span> `vnet list-endpoint-services`
* <span data-ttu-id="e73ef-1917">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Параметр `--private-access-services` переименован в `--service-endpoints` в командах</span><span class="sxs-lookup"><span data-stu-id="e73ef-1917">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for</span></span> `vnet subnet [create|update]`
* <span data-ttu-id="e73ef-1918">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах</span><span class="sxs-lookup"><span data-stu-id="e73ef-1918">Added support for multiple IP and port ranges to</span></span> `nsg rule [create|update]`
* <span data-ttu-id="e73ef-1919">Добавлена поддержка номера SKU в команде</span><span class="sxs-lookup"><span data-stu-id="e73ef-1919">Added support for SKU to</span></span> `lb create`
* <span data-ttu-id="e73ef-1920">Добавлена поддержка номера SKU в команде</span><span class="sxs-lookup"><span data-stu-id="e73ef-1920">Added support for SKU to</span></span> `public-ip create`

### <a name="profile"></a><span data-ttu-id="e73ef-1921">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1921">Profile</span></span>

* <span data-ttu-id="e73ef-1922">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1922">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e73ef-1923">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e73ef-1923">Service Fabric</span></span>

* <span data-ttu-id="e73ef-1924">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1924">Preview release</span></span>
* <span data-ttu-id="e73ef-1925">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1925">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="e73ef-1926">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1926">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="e73ef-1927">Добавлена поддержка пустого значения</span><span class="sxs-lookup"><span data-stu-id="e73ef-1927">Added support for empty</span></span> `registry_cred`

### <a name="storage"></a><span data-ttu-id="e73ef-1928">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1928">Storage</span></span>

* <span data-ttu-id="e73ef-1929">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1929">Enabled setting blob tier</span></span>
* <span data-ttu-id="e73ef-1930">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1930">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="e73ef-1931">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в</span><span class="sxs-lookup"><span data-stu-id="e73ef-1931">Added commands to add VNET rules and IP based rules to</span></span> `storage account network-rule`
* <span data-ttu-id="e73ef-1932">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1932">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="e73ef-1933">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1933">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="e73ef-1934">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1934">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1935">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1935">VM</span></span>

* <span data-ttu-id="e73ef-1936">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра</span><span class="sxs-lookup"><span data-stu-id="e73ef-1936">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using</span></span> `--instance-id *`
* <span data-ttu-id="e73ef-1937">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1937">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="e73ef-1938">Из черного списка имен администраторов удалены имена людей для команд</span><span class="sxs-lookup"><span data-stu-id="e73ef-1938">Removed human names from the admin name blacklist for</span></span> `[vm|vmss] create`
* <span data-ttu-id="e73ef-1939">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1939">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="e73ef-1940">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1940">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="e73ef-1941">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой</span><span class="sxs-lookup"><span data-stu-id="e73ef-1941">Fixed issue where `--no-wait` argument did not work wth</span></span> `vm availability-set create`


## <a name="august-15-2017"></a><span data-ttu-id="e73ef-1942">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1942">August 15, 2017</span></span>

<span data-ttu-id="e73ef-1943">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="e73ef-1943">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1944">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1944">ACS</span></span>

* <span data-ttu-id="e73ef-1945">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1945">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-1946">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-1946">Appservice</span></span>

* <span data-ttu-id="e73ef-1947">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1947">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="e73ef-1948">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-1948">Event Grid</span></span>

* <span data-ttu-id="e73ef-1949">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1949">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="e73ef-1950">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1950">August 11, 2017</span></span>

<span data-ttu-id="e73ef-1951">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="e73ef-1951">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-1952">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-1952">ACS</span></span>

* <span data-ttu-id="e73ef-1953">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1953">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="e73ef-1954">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-1954">Batch</span></span>

* <span data-ttu-id="e73ef-1955">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1955">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="e73ef-1956">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1956">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="e73ef-1957">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1957">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="e73ef-1958">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1958">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="e73ef-1959">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1959">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="e73ef-1960">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1960">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="e73ef-1961">Компонент</span><span class="sxs-lookup"><span data-stu-id="e73ef-1961">Component</span></span>

* <span data-ttu-id="e73ef-1962">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1962">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="e73ef-1963">Контейнер</span><span class="sxs-lookup"><span data-stu-id="e73ef-1963">Container</span></span>

* `create`<span data-ttu-id="e73ef-1964">: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1964">: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="e73ef-1965">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e73ef-1965">Data Lake Store</span></span>

* <span data-ttu-id="e73ef-1966">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1966">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="e73ef-1967">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-1967">Event Grid</span></span>

* <span data-ttu-id="e73ef-1968">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="e73ef-1968">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-1969">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-1969">Network</span></span>

* `lb`<span data-ttu-id="e73ef-1970">: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1970">: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* `application-gateway {subresource} delete`<span data-ttu-id="e73ef-1971">: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1971">: Fixed issue where `--no-wait` was not honored</span></span>
* `application-gateway http-settings update`<span data-ttu-id="e73ef-1972">: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1972">: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="e73ef-1973">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой</span><span class="sxs-lookup"><span data-stu-id="e73ef-1973">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with</span></span> `az network vpn-connection ipsec-policy add`

### <a name="profile"></a><span data-ttu-id="e73ef-1974">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-1974">Profile</span></span>

* `account list`<span data-ttu-id="e73ef-1975">: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1975">: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-1976">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-1976">Storage</span></span>

* <span data-ttu-id="e73ef-1977">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1977">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-1978">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-1978">VM</span></span>

* `availability-set`<span data-ttu-id="e73ef-1979">: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1979">: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="e73ef-1980">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1980">Exposed `list-skus` command</span></span>
* <span data-ttu-id="e73ef-1981">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1981">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="e73ef-1982">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1982">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="e73ef-1983">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1983">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="e73ef-1984">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1984">July 28, 2017</span></span>

<span data-ttu-id="e73ef-1985">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="e73ef-1985">Version 2.0.12</span></span>

* <span data-ttu-id="e73ef-1986">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1986">Added container commands</span></span>
* <span data-ttu-id="e73ef-1987">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1987">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="e73ef-1988">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-1988">Core</span></span>

* <span data-ttu-id="e73ef-1989">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1989">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="e73ef-1990">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1990">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="e73ef-1991">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1991">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="e73ef-1992">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1992">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="e73ef-1993">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1993">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="e73ef-1994">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1994">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="e73ef-1995">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1995">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e73ef-1996">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1996">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="e73ef-1997">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="e73ef-1997">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="e73ef-1998">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1998">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="e73ef-1999">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="e73ef-1999">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="e73ef-2000">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2000">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="e73ef-2001">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2001">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="e73ef-2002">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2002">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="e73ef-2003">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2003">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="e73ef-2004">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2004">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="e73ef-2005">ACR</span><span class="sxs-lookup"><span data-stu-id="e73ef-2005">ACR</span></span>

* <span data-ttu-id="e73ef-2006">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2006">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="e73ef-2007">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2007">Support SKU update for managed registries</span></span>
* <span data-ttu-id="e73ef-2008">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2008">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="e73ef-2009">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2009">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="e73ef-2010">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2010">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="e73ef-2011">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2011">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-2012">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-2012">ACS</span></span>

* <span data-ttu-id="e73ef-2013">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2013">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-2014">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="e73ef-2014">Appservice</span></span>

* <span data-ttu-id="e73ef-2015">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2015">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="e73ef-2016">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2016">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="e73ef-2017">Удалены все команды группы</span><span class="sxs-lookup"><span data-stu-id="e73ef-2017">Remove all commands under</span></span> `appservice web`
* <span data-ttu-id="e73ef-2018">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2018">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="e73ef-2019">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2019">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="e73ef-2020">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2020">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="e73ef-2021">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2021">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="e73ef-2022">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2022">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="e73ef-2023">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2023">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="e73ef-2024">Вместо него используется</span><span class="sxs-lookup"><span data-stu-id="e73ef-2024">Instead use</span></span> `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`

### <a name="batch"></a><span data-ttu-id="e73ef-2025">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="e73ef-2025">Batch</span></span>

* <span data-ttu-id="e73ef-2026">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2026">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="e73ef-2027">Параметр команды `pool create` переименован с `--target-dedicated` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-2027">Renamed `pool create` option `--target-dedicated` to</span></span> `--target-dedicated-nodes`
* <span data-ttu-id="e73ef-2028">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2028">Added `pool create` options `--target-low-priority-nodes` and</span></span> `--application-licenses`

### <a name="cdn"></a><span data-ttu-id="e73ef-2029">CDN</span><span class="sxs-lookup"><span data-stu-id="e73ef-2029">CDN</span></span>

* <span data-ttu-id="e73ef-2030">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2030">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="e73ef-2031">Облако</span><span class="sxs-lookup"><span data-stu-id="e73ef-2031">Cloud</span></span>

* <span data-ttu-id="e73ef-2032">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2032">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="e73ef-2033">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2033">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="e73ef-2034">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2034">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="e73ef-2035">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2035">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="e73ef-2036">Предоставлено</span><span class="sxs-lookup"><span data-stu-id="e73ef-2036">Exposed</span></span> `endpoint_vm_image_alias_doc`

### <a name="cosmosdb"></a><span data-ttu-id="e73ef-2037">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e73ef-2037">CosmosDB</span></span>

* <span data-ttu-id="e73ef-2038">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2038">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="e73ef-2039">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2039">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e73ef-2040">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e73ef-2040">Data Lake Analytics</span></span>

* <span data-ttu-id="e73ef-2041">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2041">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="e73ef-2042">Добавлено</span><span class="sxs-lookup"><span data-stu-id="e73ef-2042">Added</span></span> `dla job pipeline show`
* <span data-ttu-id="e73ef-2043">Добавлено</span><span class="sxs-lookup"><span data-stu-id="e73ef-2043">Added</span></span> `dla job recurrence list`

### <a name="data-lake-store"></a><span data-ttu-id="e73ef-2044">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e73ef-2044">Data Lake Store</span></span>

* <span data-ttu-id="e73ef-2045">Добавлена поддержка смены ключей пользовательского хранилища ключей в</span><span class="sxs-lookup"><span data-stu-id="e73ef-2045">Added support for user managed key vault key rotation in</span></span> `dls account update`
* <span data-ttu-id="e73ef-2046">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2046">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="e73ef-2047">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2047">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="e73ef-2048">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2048">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="e73ef-2049">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="e73ef-2049">Interactive</span></span>

* <span data-ttu-id="e73ef-2050">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2050">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="e73ef-2051">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2051">Increased test coverage</span></span>
* <span data-ttu-id="e73ef-2052">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2052">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="e73ef-2053">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2053">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="e73ef-2054">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2054">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="e73ef-2055">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2055">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="e73ef-2056">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2056">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="e73ef-2057">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2057">Added `--progress` flag</span></span>
* <span data-ttu-id="e73ef-2058">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2058">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="e73ef-2059">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2059">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="e73ef-2060">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="e73ef-2060">IoT</span></span>

* <span data-ttu-id="e73ef-2061">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="e73ef-2061">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="e73ef-2062">(3934).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2062">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="e73ef-2063">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="e73ef-2063">Key vault</span></span>

* <span data-ttu-id="e73ef-2064">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="e73ef-2064">Added commands for key vault recovery features:</span></span>
  * `keyvault` <span data-ttu-id="e73ef-2065">— подкоманды `purge`, `recover` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2065">subcommands `purge`, `recover`,</span></span> `keyvault list-deleted`
  * `keyvault secret` <span data-ttu-id="e73ef-2066">— подкоманды `backup`, `restore`, `purge`, `recover` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2066">subcommands `backup`, `restore`, `purge`, `recover`,</span></span> `list-deleted`
  * `keyvault certificate` <span data-ttu-id="e73ef-2067">— подкоманды `purge`, `recover` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2067">subcommands `purge`, `recover`,</span></span> `list-deleted`
  * `keyvault key` <span data-ttu-id="e73ef-2068">— подкоманды `purge`, `recover` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2068">subcommands `purge`, `recover`,</span></span> `list-deleted`
* <span data-ttu-id="e73ef-2069">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2069">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="e73ef-2070">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="e73ef-2070">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="e73ef-2071">(3307).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2071">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="e73ef-2072">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="e73ef-2072">Lab</span></span>

* <span data-ttu-id="e73ef-2073">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью</span><span class="sxs-lookup"><span data-stu-id="e73ef-2073">Added support for claiming any vm in the lab through</span></span> `az lab vm claim`
* <span data-ttu-id="e73ef-2074">Добавлен форматировщик табличных выходных данных команд `az lab vm list` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2074">Added table output formatter for `az lab vm list` and</span></span> `az lab vm show`

### <a name="monitor"></a><span data-ttu-id="e73ef-2075">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-2075">Monitor</span></span>

* <span data-ttu-id="e73ef-2076">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2076">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="e73ef-2077">Команда `monitor alert-rule-incidents list` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-2077">Renamed `monitor alert-rule-incidents list` to</span></span> `monitor alert list-incidents`
* <span data-ttu-id="e73ef-2078">Команда `monitor alert-rule-incidents show` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-2078">Renamed `monitor alert-rule-incidents show` to</span></span> `monitor alert show-incident`
* <span data-ttu-id="e73ef-2079">Команда `monitor metric-defintions list` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-2079">Renamed `monitor metric-defintions list` to</span></span> `monitor metrics list-definitions`
* <span data-ttu-id="e73ef-2080">Команда `monitor alert-rules` переименована в</span><span class="sxs-lookup"><span data-stu-id="e73ef-2080">Renamed `monitor alert-rules` to</span></span> `monitor alert`
* <span data-ttu-id="e73ef-2081">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="e73ef-2081">Changed `monitor alert create`:</span></span>
  * `condition` <span data-ttu-id="e73ef-2082">и `action` — эти подкоманды больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="e73ef-2082">and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="e73ef-2083">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="e73ef-2083">Add numerous parameters to simplify the rule creation process</span></span>
  * `location` <span data-ttu-id="e73ef-2084">больше не требуется</span><span class="sxs-lookup"><span data-stu-id="e73ef-2084">no longer required</span></span>
  * <span data-ttu-id="e73ef-2085">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="e73ef-2085">Add name and ID support for target</span></span>
  * <span data-ttu-id="e73ef-2086">Удалить</span><span class="sxs-lookup"><span data-stu-id="e73ef-2086">Remove</span></span> `--alert-rule-resource-name`
  * <span data-ttu-id="e73ef-2087">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="e73ef-2087">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * `description` <span data-ttu-id="e73ef-2088">— значения по умолчанию теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="e73ef-2088">defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="e73ef-2089">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2089">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="e73ef-2090">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2090">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="e73ef-2091">Добавлены вспомогательные аргументы и примеры использования для</span><span class="sxs-lookup"><span data-stu-id="e73ef-2091">Added convenience arguments and examples to</span></span> `monitor alert rule update`

### <a name="network"></a><span data-ttu-id="e73ef-2092">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-2092">Network</span></span>

* <span data-ttu-id="e73ef-2093">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2093">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="e73ef-2094">Добавлен аргумент `--private-access-services` для команды `vnet subnet create` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2094">Added `--private-access-services` argument to `vnet subnet create` and</span></span> `vnet subnet update`
* <span data-ttu-id="e73ef-2095">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2095">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="e73ef-2096">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2096">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="e73ef-2097">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2097">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and</span></span> `application-gateway address-pool update`
* <span data-ttu-id="e73ef-2098">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2098">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="e73ef-2099">В `application-gateway ssl-policy` добавлены команды `list-options`, `predefined list` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2099">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`,</span></span> `predefined show`
* <span data-ttu-id="e73ef-2100">Для команды `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2100">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`,</span></span> `--min-protocol-version`
* <span data-ttu-id="e73ef-2101">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2101">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="e73ef-2102">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2102">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`,</span></span> `--redirect-config`
* <span data-ttu-id="e73ef-2103">Добавлен аргумент `--redirect-config` для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-2103">Added argument `--redirect-config` to</span></span> `application-gateway url-path-map rule create`
* <span data-ttu-id="e73ef-2104">Добавлена поддержка `--no-wait` для</span><span class="sxs-lookup"><span data-stu-id="e73ef-2104">Added support for `--no-wait` to</span></span> `application-gateway url-path-map rule delete`
* <span data-ttu-id="e73ef-2105">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2105">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`,</span></span> `--match-status-codes`
* <span data-ttu-id="e73ef-2106">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2106">Added argument `--redirect-config` to `application-gateway rule create` and</span></span> `application-gateway rule update`
* <span data-ttu-id="e73ef-2107">Добавлена поддержка `--accelerated-networking` в командах `nic create` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2107">Added support for `--accelerated-networking` to `nic create` and</span></span> `nic update`
* <span data-ttu-id="e73ef-2108">Удален аргумент `--internal-dns-name-suffix` из команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-2108">Removed `--internal-dns-name-suffix` argument from</span></span> `nic create`
* <span data-ttu-id="e73ef-2109">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2109">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="e73ef-2110">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр</span><span class="sxs-lookup"><span data-stu-id="e73ef-2110">Fixed bug where `local-gateway create` ignored</span></span> `--local-address-prefixes`
* <span data-ttu-id="e73ef-2111">Добавлена поддержка `--dns-servers` в</span><span class="sxs-lookup"><span data-stu-id="e73ef-2111">Added support for `--dns-servers` to</span></span> `vnet update`
* <span data-ttu-id="e73ef-2112">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-2112">Fixed bug when creating a peering without route filtering with</span></span> `express-route peering create`
* <span data-ttu-id="e73ef-2113">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой</span><span class="sxs-lookup"><span data-stu-id="e73ef-2113">Fixed bug where `--provider` and `--bandwidth` arguments did not work with</span></span> `express-route update`
* <span data-ttu-id="e73ef-2114">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2114">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="e73ef-2115">Улучшено форматирование выходных данных команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-2115">Improved output formatting for</span></span> `network list-usages`
* <span data-ttu-id="e73ef-2116">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2116">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="e73ef-2117">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2117">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="e73ef-2118">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2118">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="e73ef-2119">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2119">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="e73ef-2120">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-2120">Profile</span></span>

* <span data-ttu-id="e73ef-2121">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2121">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="e73ef-2122">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2122">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="e73ef-2123">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2123">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="e73ef-2124">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2124">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="e73ef-2125">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2125">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="e73ef-2126">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="e73ef-2126">RDBMS</span></span>

* <span data-ttu-id="e73ef-2127">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2127">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="e73ef-2128">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2128">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="e73ef-2129">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2129">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="e73ef-2130">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2130">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-2131">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-2131">Resource</span></span>

* <span data-ttu-id="e73ef-2132">Улучшены запросы на ввод отсутствующих параметров для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-2132">Improved prompts for missing parameters for</span></span> `group deployment create`
* <span data-ttu-id="e73ef-2133">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2133">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="e73ef-2134">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2134">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="e73ef-2135">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2135">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="e73ef-2136">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2136">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="e73ef-2137">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2137">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and</span></span> `<resource-type>`
* <span data-ttu-id="e73ef-2138">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2138">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="e73ef-2139">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2139">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-2140">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-2140">Role</span></span>

* <span data-ttu-id="e73ef-2141">Поддержка вывода данных в формате файла проверки подлинности с помощью пакета SDK для команды</span><span class="sxs-lookup"><span data-stu-id="e73ef-2141">Support output in SDK auth file format for</span></span> `create-for-rbac`
* <span data-ttu-id="e73ef-2142">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2142">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="e73ef-2143">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2143">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="e73ef-2144">Отображаются предупреждения о прекращении поддержки при использовании параметра</span><span class="sxs-lookup"><span data-stu-id="e73ef-2144">Show deprecation warnings when using</span></span> `--expanded-view`
* <span data-ttu-id="e73ef-2145">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2145">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="e73ef-2146">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="e73ef-2146">Service Fabric</span></span>
* <span data-ttu-id="e73ef-2147">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2147">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="e73ef-2148">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2148">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="e73ef-2149">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2149">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-2150">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-2150">SQL</span></span>

* <span data-ttu-id="e73ef-2151">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2151">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="e73ef-2152">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2152">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="e73ef-2153">Добавлены команды `sql db list-editions` и</span><span class="sxs-lookup"><span data-stu-id="e73ef-2153">Added commands `sql db list-editions` and</span></span> `sql elastic-pool list-editions`

### <a name="storage"></a><span data-ttu-id="e73ef-2154">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-2154">Storage</span></span>

* <span data-ttu-id="e73ef-2155">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2155">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="e73ef-2156">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2156">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="e73ef-2157">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2157">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="e73ef-2158">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="e73ef-2158">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="e73ef-2159">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2159">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="e73ef-2160">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2160">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-2161">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-2161">VM</span></span>

* <span data-ttu-id="e73ef-2162">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2162">Support configuring nsg</span></span>
* <span data-ttu-id="e73ef-2163">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2163">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="e73ef-2164">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2164">Support managed service identities</span></span>
* <span data-ttu-id="e73ef-2165">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр</span><span class="sxs-lookup"><span data-stu-id="e73ef-2165">Fixed issue where `cmss create` with an existing load balancer required</span></span> `--backend-pool-name`
* <span data-ttu-id="e73ef-2166">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2166">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="e73ef-2167">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2167">May 10, 2017</span></span>

<span data-ttu-id="e73ef-2168">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="e73ef-2168">Version 2.0.6</span></span>

* <span data-ttu-id="e73ef-2169">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2169">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="e73ef-2170">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2170">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="e73ef-2171">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2171">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="e73ef-2172">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2172">Include Cognitive Services module</span></span>
* <span data-ttu-id="e73ef-2173">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2173">Include Service Fabric module</span></span>
* <span data-ttu-id="e73ef-2174">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2174">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="e73ef-2175">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2175">Add support for CDN commands</span></span>
* <span data-ttu-id="e73ef-2176">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2176">Remove Container module</span></span>
* <span data-ttu-id="e73ef-2177">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2177">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="e73ef-2178">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2178">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="e73ef-2179">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-2179">Core</span></span>

* <span data-ttu-id="e73ef-2180">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2180">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="e73ef-2181">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2181">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="e73ef-2182">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2182">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="e73ef-2183">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2183">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="e73ef-2184">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2184">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="e73ef-2185">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2185">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="e73ef-2186">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2186">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="e73ef-2187">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2187">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="e73ef-2188">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2188">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="e73ef-2189">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2189">core: Improved performance</span></span>
* <span data-ttu-id="e73ef-2190">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2190">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="e73ef-2191">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2191">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-2192">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-2192">ACS</span></span>

* <span data-ttu-id="e73ef-2193">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2193">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="e73ef-2194">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2194">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="e73ef-2195">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2195">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="e73ef-2196">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2196">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-2197">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-2197">AppService</span></span>

* <span data-ttu-id="e73ef-2198">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2198">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="e73ef-2199">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2199">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="e73ef-2200">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2200">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="e73ef-2201">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2201">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="e73ef-2202">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2202">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="e73ef-2203">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2203">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="e73ef-2204">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2204">support slot swap with preview</span></span>
* <span data-ttu-id="e73ef-2205">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2205">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="e73ef-2206">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2206">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="e73ef-2207">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="e73ef-2207">CosmosDB</span></span>

* <span data-ttu-id="e73ef-2208">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2208">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="e73ef-2209">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2209">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="e73ef-2210">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2210">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="e73ef-2211">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2211">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="e73ef-2212">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="e73ef-2212">Data Lake Analytics</span></span>

* <span data-ttu-id="e73ef-2213">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2213">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="e73ef-2214">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2214">Add support for new catalog item type: package.</span></span> <span data-ttu-id="e73ef-2215">Для доступа к нему используется</span><span class="sxs-lookup"><span data-stu-id="e73ef-2215">accessed through:</span></span> `az dla catalog package`
* <span data-ttu-id="e73ef-2216">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="e73ef-2216">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="e73ef-2217">Таблица</span><span class="sxs-lookup"><span data-stu-id="e73ef-2217">Table</span></span>
  * <span data-ttu-id="e73ef-2218">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="e73ef-2218">Table valued function</span></span>
  * <span data-ttu-id="e73ef-2219">Просмотр</span><span class="sxs-lookup"><span data-stu-id="e73ef-2219">View</span></span>
  * <span data-ttu-id="e73ef-2220">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2220">Table Statistics.</span></span> <span data-ttu-id="e73ef-2221">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2221">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="e73ef-2222">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="e73ef-2222">Data Lake Store</span></span>

* <span data-ttu-id="e73ef-2223">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2223">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="e73ef-2224">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2224">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="e73ef-2225">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2225">missed help for access show.</span></span> <span data-ttu-id="e73ef-2226">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2226">adding it.</span></span> <span data-ttu-id="e73ef-2227">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="e73ef-2227">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="e73ef-2228">Поиск</span><span class="sxs-lookup"><span data-stu-id="e73ef-2228">Find</span></span>

* <span data-ttu-id="e73ef-2229">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2229">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="e73ef-2230">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="e73ef-2230">KeyVault</span></span>

* <span data-ttu-id="e73ef-2231">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2231">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="e73ef-2232">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2232">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="e73ef-2233">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2233">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="e73ef-2234">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2234">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="e73ef-2235">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2235">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="e73ef-2236">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="e73ef-2236">Lab</span></span>

* <span data-ttu-id="e73ef-2237">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2237">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="e73ef-2238">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2238">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="e73ef-2239">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2239">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="e73ef-2240">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2240">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="e73ef-2241">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2241">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="e73ef-2242">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="e73ef-2242">Monitor</span></span>

* <span data-ttu-id="e73ef-2243">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2243">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="e73ef-2244">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2244">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="e73ef-2245">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-2245">Network</span></span>

* <span data-ttu-id="e73ef-2246">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2246">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="e73ef-2247">Добавлена поддержка параметра `--filters` в команде</span><span class="sxs-lookup"><span data-stu-id="e73ef-2247">Add support for `--filters` parameter for</span></span> `network watcher packet-capture create`
* <span data-ttu-id="e73ef-2248">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2248">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="e73ef-2249">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2249">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="e73ef-2250">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2250">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="e73ef-2251">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2251">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="e73ef-2252">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2252">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="e73ef-2253">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2253">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="e73ef-2254">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2254">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="e73ef-2255">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="e73ef-2255">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="e73ef-2256">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2256">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="e73ef-2257">BC: исправлена ошибка в выходных данных</span><span class="sxs-lookup"><span data-stu-id="e73ef-2257">BC: Fix bug in the output of</span></span> `vpn-connection create`
* <span data-ttu-id="e73ef-2258">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2258">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="e73ef-2259">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2259">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="e73ef-2260">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2260">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="e73ef-2261">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2261">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="e73ef-2262">Профиль</span><span class="sxs-lookup"><span data-stu-id="e73ef-2262">Profile</span></span>

* <span data-ttu-id="e73ef-2263">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2263">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="e73ef-2264">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2264">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="e73ef-2265">Redis</span><span class="sxs-lookup"><span data-stu-id="e73ef-2265">Redis</span></span>

* <span data-ttu-id="e73ef-2266">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2266">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="e73ef-2267">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2267">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="e73ef-2268">Ресурс</span><span class="sxs-lookup"><span data-stu-id="e73ef-2268">Resource</span></span>

* <span data-ttu-id="e73ef-2269">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2269">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="e73ef-2270">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2270">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="e73ef-2271">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2271">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="e73ef-2272">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2272">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="e73ef-2273">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="e73ef-2273">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="e73ef-2274">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2274">Add docs for az lock update.</span></span> <span data-ttu-id="e73ef-2275">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="e73ef-2275">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="e73ef-2276">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2276">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="e73ef-2277">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="e73ef-2277">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="e73ef-2278">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2278">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="e73ef-2279">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="e73ef-2279">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="e73ef-2280">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2280">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="e73ef-2281">Роль</span><span class="sxs-lookup"><span data-stu-id="e73ef-2281">Role</span></span>

* <span data-ttu-id="e73ef-2282">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2282">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="e73ef-2283">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2283">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="e73ef-2284">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2284">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="e73ef-2285">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2285">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="e73ef-2286">SQL</span><span class="sxs-lookup"><span data-stu-id="e73ef-2286">SQL</span></span>

* <span data-ttu-id="e73ef-2287">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2287">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="e73ef-2288">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2288">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="e73ef-2289">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-2289">Storage</span></span>

* <span data-ttu-id="e73ef-2290">Добавлено расположение по умолчанию группы ресурсов для</span><span class="sxs-lookup"><span data-stu-id="e73ef-2290">Default location to resource group location for</span></span> `storage account create`
* <span data-ttu-id="e73ef-2291">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2291">Add support for incremental blob copy</span></span>
* <span data-ttu-id="e73ef-2292">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2292">Add support for large block blob upload</span></span>
* <span data-ttu-id="e73ef-2293">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2293">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-2294">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-2294">VM</span></span>

* <span data-ttu-id="e73ef-2295">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2295">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="e73ef-2296">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="e73ef-2296">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="e73ef-2297">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="e73ef-2297">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="e73ef-2298">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="e73ef-2298">az vm/vmss disk</span></span>
  3. <span data-ttu-id="e73ef-2299">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2299">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="e73ef-2300">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2300">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="e73ef-2301">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2301">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="e73ef-2302">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2302">April 3, 2017</span></span>

<span data-ttu-id="e73ef-2303">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="e73ef-2303">Version 2.0.2</span></span>

<span data-ttu-id="e73ef-2304">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2304">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="e73ef-2305">Core</span><span class="sxs-lookup"><span data-stu-id="e73ef-2305">Core</span></span>

* <span data-ttu-id="e73ef-2306">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2306">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="e73ef-2307">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2307">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="e73ef-2308">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2308">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="e73ef-2309">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2309">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e73ef-2310">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2310">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="e73ef-2311">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="e73ef-2311">Add prompting for missing template parameters.</span></span> <span data-ttu-id="e73ef-2312">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2312">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="e73ef-2313">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2313">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="e73ef-2314">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2314">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="e73ef-2315">ACS</span><span class="sxs-lookup"><span data-stu-id="e73ef-2315">ACS</span></span>

* <span data-ttu-id="e73ef-2316">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2316">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="e73ef-2317">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="e73ef-2317">Add support for ssh key password prompting.</span></span> <span data-ttu-id="e73ef-2318">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2318">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="e73ef-2319">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="e73ef-2319">Add support for windows clusters.</span></span> <span data-ttu-id="e73ef-2320">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2320">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="e73ef-2321">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="e73ef-2321">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="e73ef-2322">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2322">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="e73ef-2323">AppService</span><span class="sxs-lookup"><span data-stu-id="e73ef-2323">AppService</span></span>

* <span data-ttu-id="e73ef-2324">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2324">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="e73ef-2325">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2325">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="e73ef-2326">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2326">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="e73ef-2327">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2327">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="e73ef-2328">Data Lake</span><span class="sxs-lookup"><span data-stu-id="e73ef-2328">DataLake</span></span>

* <span data-ttu-id="e73ef-2329">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2329">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="e73ef-2330">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2330">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="e73ef-2331">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="e73ef-2331">DocuemntDB</span></span>

* <span data-ttu-id="e73ef-2332">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2332">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="e73ef-2333">ВМ</span><span class="sxs-lookup"><span data-stu-id="e73ef-2333">VM</span></span>

* <span data-ttu-id="e73ef-2334">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2334">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="e73ef-2335">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2335">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="e73ef-2336">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2336">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="e73ef-2337">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2337">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="e73ef-2338">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2338">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="e73ef-2339">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2339">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="e73ef-2340">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2340">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="e73ef-2341">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2341">February 27, 2017</span></span>

<span data-ttu-id="e73ef-2342">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e73ef-2342">Version 2.0.0</span></span>

<span data-ttu-id="e73ef-2343">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="e73ef-2343">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="e73ef-2344">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="e73ef-2344">Container Service (acs)</span></span>
- <span data-ttu-id="e73ef-2345">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="e73ef-2345">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="e73ef-2346">Сеть</span><span class="sxs-lookup"><span data-stu-id="e73ef-2346">Networking</span></span>
- <span data-ttu-id="e73ef-2347">Хранилище</span><span class="sxs-lookup"><span data-stu-id="e73ef-2347">Storage</span></span>

<span data-ttu-id="e73ef-2348">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2348">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="e73ef-2349">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2349">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="e73ef-2350">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2350">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="e73ef-2351">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2351">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="e73ef-2352">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="e73ef-2352">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="e73ef-2353">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="e73ef-2353">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="e73ef-2354">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="e73ef-2354">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="e73ef-2355">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="e73ef-2355">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="e73ef-2356">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="e73ef-2356">Provide feedback from the command line with the `az feedback` command</span></span>

