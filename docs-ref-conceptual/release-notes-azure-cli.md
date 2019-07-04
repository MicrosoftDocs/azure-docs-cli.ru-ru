---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/18/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 8431946b169b550bfd3f5120cf26e2feeb5c9f2c
ms.sourcegitcommit: 399f0a2997675fbb280243e4234cf63c3bbca819
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2019
ms.locfileid: "67194870"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="884bc-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="884bc-103">Azure CLI release notes</span></span>

## <a name="june-18-2019"></a><span data-ttu-id="884bc-104">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-104">June 18, 2019</span></span>

<span data-ttu-id="884bc-105">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="884bc-105">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="884bc-106">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-106">Core</span></span>

<span data-ttu-id="884bc-107">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="884bc-107">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="884bc-108">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="884bc-108">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="884bc-109">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="884bc-109">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="884bc-110">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="884bc-110">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="884bc-111">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="884bc-111">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="884bc-112">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="884bc-112">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="884bc-113">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="884bc-113">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-114">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-114">ACR</span></span>
* <span data-ttu-id="884bc-115">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="884bc-115">Added 'acr check-health' command</span></span>
* <span data-ttu-id="884bc-116">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-116">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-117">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-117">ACS</span></span>
* <span data-ttu-id="884bc-118">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="884bc-118">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="884bc-119">AMS</span><span class="sxs-lookup"><span data-stu-id="884bc-119">AMS</span></span>
* <span data-ttu-id="884bc-120">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="884bc-120">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-121">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-121">AppService</span></span>
* <span data-ttu-id="884bc-122">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="884bc-122">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="884bc-123">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="884bc-123">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="884bc-124">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="884bc-124">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="884bc-125">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-125">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="884bc-126">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="884bc-126">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="884bc-127">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="884bc-127">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-128">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-128">Batch</span></span>
* <span data-ttu-id="884bc-129">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="884bc-129">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="884bc-130">Batch AI</span><span class="sxs-lookup"><span data-stu-id="884bc-130">BatchAI</span></span>
* <span data-ttu-id="884bc-131">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="884bc-131">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="884bc-132">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="884bc-132">BotService</span></span>
* <span data-ttu-id="884bc-133">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="884bc-133">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="884bc-134">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-134">CosmosDB</span></span>
* <span data-ttu-id="884bc-135">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="884bc-135">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="884bc-136">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="884bc-136">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="884bc-137">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="884bc-137">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="884bc-138">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="884bc-138">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="884bc-139">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="884bc-139">EventGrid</span></span>
* <span data-ttu-id="884bc-140">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="884bc-140">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="884bc-141">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="884bc-141">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="884bc-142">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="884bc-142">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="884bc-143">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="884bc-143">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="884bc-144">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-144">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="884bc-145">HDInsight</span><span class="sxs-lookup"><span data-stu-id="884bc-145">HDInsight</span></span>
* <span data-ttu-id="884bc-146">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-146">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-147">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-147">IoT</span></span>
* <span data-ttu-id="884bc-148">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="884bc-148">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="884bc-149">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="884bc-149">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="884bc-150">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-150">Network</span></span>
* <span data-ttu-id="884bc-151">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="884bc-151">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="884bc-152">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="884bc-152">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="884bc-153">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="884bc-153">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="884bc-154">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="884bc-154">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-155">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-155">Resource</span></span>
* <span data-ttu-id="884bc-156">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="884bc-156">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="884bc-157">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="884bc-157">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="884bc-158">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="884bc-158">ServiceBus</span></span>
* <span data-ttu-id="884bc-159">Исправлена ошибка [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="884bc-159">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-160">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-160">SQL</span></span>
* <span data-ttu-id="884bc-161">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="884bc-161">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="884bc-162">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="884bc-162">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="884bc-163">SQLVm</span><span class="sxs-lookup"><span data-stu-id="884bc-163">SQLVm</span></span>
* <span data-ttu-id="884bc-164">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="884bc-164">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="884bc-165">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="884bc-165">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-166">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-166">Storage</span></span>
* <span data-ttu-id="884bc-167">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="884bc-167">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="884bc-168">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="884bc-168">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-169">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-169">VM</span></span>
* <span data-ttu-id="884bc-170">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="884bc-170">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="884bc-171">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-171">June 4, 2019</span></span>

<span data-ttu-id="884bc-172">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="884bc-172">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="884bc-173">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-173">Core</span></span>
* <span data-ttu-id="884bc-174">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="884bc-174">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-175">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-175">ACR</span></span>
* <span data-ttu-id="884bc-176">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="884bc-176">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-177">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-177">ACS</span></span>
* <span data-ttu-id="884bc-178">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="884bc-178">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="884bc-179">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="884bc-179">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-180">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-180">Batch</span></span>
* <span data-ttu-id="884bc-181">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="884bc-181">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-182">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-182">IoT</span></span>
* <span data-ttu-id="884bc-183">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="884bc-183">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="884bc-184">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-184">Network</span></span>
* <span data-ttu-id="884bc-185">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="884bc-185">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="884bc-186">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="884bc-186">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="884bc-187">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-187">Resource</span></span>
* <span data-ttu-id="884bc-188">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="884bc-188">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="884bc-189">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-189">Role</span></span>
* <span data-ttu-id="884bc-190">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="884bc-190">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="884bc-191">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="884bc-191">Compute</span></span>
* <span data-ttu-id="884bc-192">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="884bc-192">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="884bc-193">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-193">May 21, 2019</span></span>

<span data-ttu-id="884bc-194">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="884bc-194">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="884bc-195">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-195">Core</span></span>
* <span data-ttu-id="884bc-196">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="884bc-196">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="884bc-197">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="884bc-197">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="884bc-198">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="884bc-198">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-199">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-199">ACR</span></span>
* <span data-ttu-id="884bc-200">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="884bc-200">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-201">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-201">ACS</span></span>
* <span data-ttu-id="884bc-202">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="884bc-202">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-203">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-203">AppService</span></span>
* <span data-ttu-id="884bc-204">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="884bc-204">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="884bc-205">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="884bc-205">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="884bc-206">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="884bc-206">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="884bc-207">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="884bc-207">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="884bc-208">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="884bc-208">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="884bc-209">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="884bc-209">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="884bc-210">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="884bc-210">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="884bc-211">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="884bc-211">BotService</span></span>
* <span data-ttu-id="884bc-212">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-212">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="884bc-213">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="884bc-213">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="884bc-214">Потребление</span><span class="sxs-lookup"><span data-stu-id="884bc-214">Consumption</span></span>
* <span data-ttu-id="884bc-215">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="884bc-215">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-216">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-216">IoT</span></span>
* <span data-ttu-id="884bc-217">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="884bc-217">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="884bc-218">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-218">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="884bc-220">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="884bc-220">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="884bc-221">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="884bc-221">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="884bc-222">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="884bc-222">RDBMS</span></span>
* <span data-ttu-id="884bc-223">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="884bc-223">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="884bc-224">RBAC</span><span class="sxs-lookup"><span data-stu-id="884bc-224">RBAC</span></span>
* <span data-ttu-id="884bc-225">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="884bc-225">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-226">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-226">Storage</span></span>
* <span data-ttu-id="884bc-227">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="884bc-227">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="884bc-228">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="884bc-228">Compute</span></span>
* <span data-ttu-id="884bc-229">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="884bc-229">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="884bc-230">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="884bc-230">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="884bc-231">__Примечание__. Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="884bc-231">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="884bc-232">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="884bc-232">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="884bc-233">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-233">May 6, 2019</span></span>

<span data-ttu-id="884bc-234">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="884bc-234">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-235">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-235">ACS</span></span>
* <span data-ttu-id="884bc-236">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="884bc-236">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="884bc-237">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="884bc-237">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="884bc-238">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-238">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="884bc-239">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="884bc-239">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-240">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-240">Appservice</span></span>
* <span data-ttu-id="884bc-241">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="884bc-241">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="884bc-242">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="884bc-242">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="884bc-243">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="884bc-243">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="884bc-244">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="884bc-244">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="884bc-245">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="884bc-245">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="884bc-246">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="884bc-246">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="884bc-247">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="884bc-247">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="884bc-248">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="884bc-248">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="884bc-249">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="884bc-249">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="884bc-250">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="884bc-250">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-251">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-251">Batch</span></span>
* <span data-ttu-id="884bc-252">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="884bc-252">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="884bc-253">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="884bc-253">Botservice</span></span>
* <span data-ttu-id="884bc-254">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="884bc-254">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="884bc-255">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="884bc-255">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="884bc-256">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="884bc-256">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="884bc-257">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-257">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="884bc-258">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-258">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="884bc-259">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="884bc-259">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="884bc-260">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-260">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="884bc-261">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="884bc-261">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="884bc-262">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="884bc-262">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="884bc-263">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="884bc-263">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="884bc-264">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="884bc-264">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="884bc-265">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="884bc-265">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="884bc-266">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="884bc-266">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="884bc-267">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="884bc-267">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="884bc-268">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-268">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="884bc-269">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="884bc-269">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="884bc-270">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="884bc-270">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="884bc-271">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="884bc-271">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="884bc-272">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="884bc-272">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="884bc-273">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="884bc-273">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="884bc-274">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="884bc-274">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="884bc-275">Настройка</span><span class="sxs-lookup"><span data-stu-id="884bc-275">Configure</span></span>
* <span data-ttu-id="884bc-276">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="884bc-276">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="884bc-277">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="884bc-277">Eventhubs</span></span>
* <span data-ttu-id="884bc-278">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="884bc-278">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="884bc-279">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-279">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="884bc-280">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-280">Network</span></span>
* <span data-ttu-id="884bc-281">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-281">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="884bc-282">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="884bc-282">Policy Insights</span></span>
* <span data-ttu-id="884bc-283">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="884bc-283">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="884bc-284">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-284">Role</span></span>
* <span data-ttu-id="884bc-285">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="884bc-285">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="884bc-286">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-286">Service Bus</span></span>
* <span data-ttu-id="884bc-287">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="884bc-287">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="884bc-288">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-288">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="884bc-289">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="884bc-289">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-290">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-290">SQL</span></span>
* <span data-ttu-id="884bc-291">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-291">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-292">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-292">VM</span></span>
* <span data-ttu-id="884bc-293">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="884bc-293">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="884bc-294">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="884bc-294">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="884bc-295">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-295">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="884bc-296">Добавлена новая группа команд `ppg` для управления группами размещения близкого расположения.</span><span class="sxs-lookup"><span data-stu-id="884bc-296">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="884bc-297">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="884bc-297">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="884bc-298">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-298">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="884bc-299">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-299">April 23, 2019</span></span>

<span data-ttu-id="884bc-300">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="884bc-300">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-301">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-301">ACS</span></span>
* <span data-ttu-id="884bc-302">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="884bc-302">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="884bc-303">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="884bc-303">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="884bc-304">AMS</span><span class="sxs-lookup"><span data-stu-id="884bc-304">AMS</span></span>
* <span data-ttu-id="884bc-305">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="884bc-305">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-306">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-306">AppService</span></span>
* <span data-ttu-id="884bc-307">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="884bc-307">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="884bc-308">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="884bc-308">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="884bc-309">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="884bc-309">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="884bc-310">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="884bc-310">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="884bc-311">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-311">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="884bc-312">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="884bc-312">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="884bc-313">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="884bc-313">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="884bc-314">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="884bc-314">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="884bc-315">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="884bc-315">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="884bc-316">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="884bc-316">Deployment Manager</span></span>
* <span data-ttu-id="884bc-317">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="884bc-317">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="884bc-318">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="884bc-318">Lab</span></span>
* <span data-ttu-id="884bc-319">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="884bc-319">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="884bc-320">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-320">Network</span></span>
* <span data-ttu-id="884bc-321">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="884bc-321">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-322">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-322">Resource</span></span>
* <span data-ttu-id="884bc-323">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="884bc-323">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="884bc-324">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="884bc-324">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="884bc-325">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="884bc-325">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="884bc-326">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="884bc-326">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-327">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-327">SQL</span></span>
* <span data-ttu-id="884bc-328">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="884bc-328">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="884bc-329">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-329">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="884bc-330">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-330">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="884bc-331">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-331">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-332">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-332">Storage</span></span>
* <span data-ttu-id="884bc-333">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="884bc-333">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-334">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-334">VM</span></span>
* <span data-ttu-id="884bc-335">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="884bc-335">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="884bc-336">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="884bc-336">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="884bc-337">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="884bc-337">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="884bc-338">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-338">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="884bc-339">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-339">Core</span></span>
* <span data-ttu-id="884bc-340">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="884bc-340">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-341">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-341">ACR</span></span>
* <span data-ttu-id="884bc-342">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="884bc-342">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="884bc-343">AMS</span><span class="sxs-lookup"><span data-stu-id="884bc-343">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="884bc-346">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-346">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="884bc-347">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-347">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-348">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-348">AppService</span></span>
* <span data-ttu-id="884bc-349">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="884bc-349">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="884bc-350">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="884bc-350">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="884bc-351">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-351">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="884bc-352">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="884bc-352">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="884bc-353">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="884bc-353">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="884bc-354">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="884bc-354">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="884bc-355">Добавлена поддержка параметров масштабирования плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="884bc-355">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="884bc-356">CDN</span><span class="sxs-lookup"><span data-stu-id="884bc-356">CDN</span></span>
* <span data-ttu-id="884bc-357">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="884bc-357">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="884bc-358">Отзыв</span><span class="sxs-lookup"><span data-stu-id="884bc-358">Feedback</span></span>
* <span data-ttu-id="884bc-359">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-359">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="884bc-360">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="884bc-360">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="884bc-361">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="884bc-361">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-362">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-362">Monitor</span></span>
* <span data-ttu-id="884bc-363">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-363">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="884bc-364">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-364">Network</span></span>
* <span data-ttu-id="884bc-365">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="884bc-365">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="884bc-366">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="884bc-366">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="884bc-367">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="884bc-367">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="884bc-368">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-368">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="884bc-369">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="884bc-369">PrivateDNS</span></span>
* <span data-ttu-id="884bc-370">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="884bc-370">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-371">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-371">Resource</span></span>
* <span data-ttu-id="884bc-372">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="884bc-372">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="884bc-373">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-373">Role</span></span>
* <span data-ttu-id="884bc-374">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="884bc-374">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="884bc-375">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="884bc-375">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-376">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-376">SQL</span></span>
* <span data-ttu-id="884bc-377">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="884bc-377">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-378">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-378">Storage</span></span>
* <span data-ttu-id="884bc-379">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="884bc-379">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="884bc-380">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="884bc-380">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="884bc-381">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="884bc-381">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="884bc-382">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="884bc-382">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="884bc-383">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-383">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="884bc-384">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-384">Core</span></span>
* <span data-ttu-id="884bc-385">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="884bc-385">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="884bc-386">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="884bc-386">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="884bc-387">Облако</span><span class="sxs-lookup"><span data-stu-id="884bc-387">Cloud</span></span>
* <span data-ttu-id="884bc-388">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="884bc-388">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-389">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-389">ACR</span></span>
* <span data-ttu-id="884bc-390">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="884bc-390">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="884bc-391">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-391">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="884bc-392">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="884bc-392">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="884bc-393">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="884bc-393">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-394">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-394">AppService</span></span>
* <span data-ttu-id="884bc-395">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="884bc-395">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="884bc-396">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="884bc-396">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="884bc-397">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="884bc-397">BOT Service</span></span>
* <span data-ttu-id="884bc-398">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="884bc-398">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="884bc-399">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="884bc-399">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="884bc-400">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="884bc-400">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="884bc-401">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="884bc-401">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="884bc-402">CDN</span><span class="sxs-lookup"><span data-stu-id="884bc-402">CDN</span></span>
* <span data-ttu-id="884bc-403">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-403">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="884bc-404">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-404">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="884bc-405">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-405">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="884bc-406">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="884bc-406">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="884bc-407">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-407">Cosmosdb</span></span>
* <span data-ttu-id="884bc-408">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="884bc-408">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="884bc-409">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="884bc-409">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-410">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-410">Interactive</span></span>
* <span data-ttu-id="884bc-411">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="884bc-411">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-412">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-412">Monitor</span></span>
* <span data-ttu-id="884bc-413">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-413">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="884bc-414">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-414">Network</span></span>
* <span data-ttu-id="884bc-415">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="884bc-415">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="884bc-416">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-416">Profile</span></span>
* <span data-ttu-id="884bc-417">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="884bc-417">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="884bc-418">Postgres</span><span class="sxs-lookup"><span data-stu-id="884bc-418">Postgres</span></span> 
* <span data-ttu-id="884bc-419">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="884bc-419">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="884bc-420">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="884bc-420">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-421">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-421">Resource</span></span>
* <span data-ttu-id="884bc-422">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-422">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="884bc-423">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="884bc-423">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="884bc-424">График</span><span class="sxs-lookup"><span data-stu-id="884bc-424">Graph</span></span>
* <span data-ttu-id="884bc-425">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="884bc-425">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="884bc-426">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="884bc-426">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="884bc-427">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="884bc-427">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="884bc-428">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="884bc-428">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="884bc-429">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="884bc-429">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-430">storage</span><span class="sxs-lookup"><span data-stu-id="884bc-430">storage</span></span>
* <span data-ttu-id="884bc-431">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="884bc-431">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="884bc-432">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="884bc-432">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="884bc-433">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="884bc-433">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="884bc-434">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="884bc-434">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-435">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-435">VM</span></span>
* <span data-ttu-id="884bc-436">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-436">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="884bc-437">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-437">March 12, 2019</span></span>

<span data-ttu-id="884bc-438">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="884bc-438">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="884bc-439">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-439">Core</span></span>

* <span data-ttu-id="884bc-440">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="884bc-440">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-441">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-441">ACR</span></span>

* <span data-ttu-id="884bc-442">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="884bc-442">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-443">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-443">ACS</span></span>

* <span data-ttu-id="884bc-444">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="884bc-444">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="884bc-445">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-445">AppService</span></span>

* <span data-ttu-id="884bc-446">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="884bc-446">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="884bc-447">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-447">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="884bc-448">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="884bc-448">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="884bc-449">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="884bc-449">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="884bc-450">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="884bc-450">Botservice</span></span>

* <span data-ttu-id="884bc-451">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="884bc-451">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="884bc-452">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="884bc-452">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="884bc-453">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-453">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="884bc-454">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="884bc-454">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="884bc-455">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-455">Container</span></span>

* <span data-ttu-id="884bc-456">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="884bc-456">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="884bc-457">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="884bc-457">EventHub</span></span>

* <span data-ttu-id="884bc-458">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="884bc-458">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="884bc-459">Поиск</span><span class="sxs-lookup"><span data-stu-id="884bc-459">Find</span></span>

* <span data-ttu-id="884bc-460">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="884bc-460">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="884bc-461">HDInsight</span><span class="sxs-lookup"><span data-stu-id="884bc-461">HDInsight</span></span>

* <span data-ttu-id="884bc-462">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="884bc-462">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="884bc-463">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-463">Network</span></span>

* <span data-ttu-id="884bc-464">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="884bc-464">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="884bc-465">Rdbms</span><span class="sxs-lookup"><span data-stu-id="884bc-465">Rdbms</span></span>

* <span data-ttu-id="884bc-466">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="884bc-466">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="884bc-467">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-467">Role</span></span>

* <span data-ttu-id="884bc-468">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="884bc-468">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="884bc-469">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="884bc-469">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="884bc-470">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="884bc-470">Service Fabric</span></span>

* <span data-ttu-id="884bc-471">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="884bc-471">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="884bc-472">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-472">February 26, 2019</span></span>

<span data-ttu-id="884bc-473">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="884bc-473">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="884bc-474">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-474">Core</span></span>

* <span data-ttu-id="884bc-475">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="884bc-475">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-476">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-476">ACR</span></span>

* <span data-ttu-id="884bc-477">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-477">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="884bc-478">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="884bc-478">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-479">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-479">ACS</span></span>

* <span data-ttu-id="884bc-480">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="884bc-480">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-481">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-481">AppService</span></span>

* <span data-ttu-id="884bc-482">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="884bc-482">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-483">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-483">Batch</span></span>
* <span data-ttu-id="884bc-484">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="884bc-484">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="884bc-485">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="884bc-485">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="884bc-486">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="884bc-486">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="884bc-487">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="884bc-487">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="884bc-488">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="884bc-488">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="884bc-489">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="884bc-489">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="884bc-490">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-490">CosmosDB</span></span>

* <span data-ttu-id="884bc-491">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="884bc-491">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="884bc-492">Kusto</span><span class="sxs-lookup"><span data-stu-id="884bc-492">Kusto</span></span>

* <span data-ttu-id="884bc-493">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="884bc-493">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="884bc-494">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-494">Network</span></span>

* <span data-ttu-id="884bc-495">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="884bc-495">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="884bc-496">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="884bc-496">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="884bc-497">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="884bc-497">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="884bc-498">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-498">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="884bc-499">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-499">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="884bc-500">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="884bc-500">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="884bc-501">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="884bc-501">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-502">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-502">Resource</span></span>

* <span data-ttu-id="884bc-503">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="884bc-503">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="884bc-504">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-504">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="884bc-505">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-505">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="884bc-506">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-506">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="884bc-507">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="884bc-507">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="884bc-508">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-508">Role</span></span>

* <span data-ttu-id="884bc-509">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-509">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-510">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-510">VM</span></span>

* <span data-ttu-id="884bc-511">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="884bc-511">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="884bc-512">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-512">February 12, 2019</span></span>

<span data-ttu-id="884bc-513">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="884bc-513">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="884bc-514">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-514">Core</span></span>

* <span data-ttu-id="884bc-515">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="884bc-515">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="884bc-516">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="884bc-516">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-517">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-517">ACR</span></span>
* <span data-ttu-id="884bc-518">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="884bc-518">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="884bc-519">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="884bc-519">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-520">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-520">ACS</span></span>
* <span data-ttu-id="884bc-521">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="884bc-521">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="884bc-522">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="884bc-522">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="884bc-523">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="884bc-523">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="884bc-524">AMS</span><span class="sxs-lookup"><span data-stu-id="884bc-524">AMS</span></span>
* <span data-ttu-id="884bc-525">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-525">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="884bc-526">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-526">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-527">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-527">Appservice</span></span>
* <span data-ttu-id="884bc-528">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="884bc-528">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="884bc-529">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="884bc-529">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="884bc-530">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-530">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="884bc-531">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="884bc-531">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="884bc-532">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="884bc-532">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="884bc-533">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="884bc-533">Botservice</span></span>
* <span data-ttu-id="884bc-534">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="884bc-534">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="884bc-535">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="884bc-535">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="884bc-536">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-536">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="884bc-537">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="884bc-537">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="884bc-538">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="884bc-538">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="884bc-539">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="884bc-539">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="884bc-540">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="884bc-540">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="884bc-541">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="884bc-541">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="884bc-542">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="884bc-542">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="884bc-543">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="884bc-543">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="884bc-544">Key Vault</span><span class="sxs-lookup"><span data-stu-id="884bc-544">Key Vault</span></span>
* <span data-ttu-id="884bc-545">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="884bc-545">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-546">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-546">Monitor</span></span>
* <span data-ttu-id="884bc-547">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="884bc-547">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="884bc-548">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-548">Network</span></span>
* <span data-ttu-id="884bc-549">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="884bc-549">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="884bc-550">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="884bc-550">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="884bc-551">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="884bc-551">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="884bc-552">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="884bc-552">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="884bc-553">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="884bc-553">Policy Insights</span></span>
* <span data-ttu-id="884bc-554">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="884bc-554">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="884bc-555">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="884bc-555">RDBMS</span></span>
* <span data-ttu-id="884bc-556">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="884bc-556">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="884bc-557">Redis</span><span class="sxs-lookup"><span data-stu-id="884bc-557">Redis</span></span>
* <span data-ttu-id="884bc-558">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="884bc-558">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="884bc-559">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="884bc-559">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="884bc-560">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="884bc-560">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="884bc-561">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="884bc-561">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="884bc-562">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="884bc-562">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="884bc-563">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="884bc-563">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="884bc-564">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="884bc-564">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="884bc-565">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-565">Role</span></span>
* <span data-ttu-id="884bc-566">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="884bc-566">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="884bc-567">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-567">SQL VM</span></span>
* <span data-ttu-id="884bc-568">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="884bc-568">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-569">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-569">VM</span></span>
* <span data-ttu-id="884bc-570">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="884bc-570">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="884bc-571">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-571">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="884bc-572">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="884bc-572">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="884bc-573">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="884bc-573">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="884bc-574">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-574">January 31, 2019</span></span>

<span data-ttu-id="884bc-575">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="884bc-575">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="884bc-576">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-576">Core</span></span>

* <span data-ttu-id="884bc-577">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="884bc-577">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="884bc-578">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-578">January 28, 2019</span></span>

<span data-ttu-id="884bc-579">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="884bc-579">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-580">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-580">ACR</span></span>
* <span data-ttu-id="884bc-581">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="884bc-581">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-582">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-582">ACS</span></span>
* <span data-ttu-id="884bc-583">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="884bc-583">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="884bc-584">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="884bc-584">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="884bc-585">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="884bc-585">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="884bc-586">AMS</span><span class="sxs-lookup"><span data-stu-id="884bc-586">AMS</span></span>
* <span data-ttu-id="884bc-587">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="884bc-587">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="884bc-588">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="884bc-588">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-589">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-589">Appservice</span></span>
* <span data-ttu-id="884bc-590">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-590">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="884bc-591">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="884bc-591">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="884bc-592">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="884bc-592">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="884bc-593">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-593">Container</span></span>
* <span data-ttu-id="884bc-594">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="884bc-594">Added `container start` command</span></span>
* <span data-ttu-id="884bc-595">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-595">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="884bc-596">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="884bc-596">EventGrid</span></span>
* <span data-ttu-id="884bc-597">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-597">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="884bc-598">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="884bc-598">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="884bc-599">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="884bc-599">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="884bc-600">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="884bc-600">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="884bc-601">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="884bc-601">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="884bc-602">HDInsight</span><span class="sxs-lookup"><span data-stu-id="884bc-602">HDInsight</span></span>
* <span data-ttu-id="884bc-603">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="884bc-603">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="884bc-604">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="884bc-604">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="884bc-605">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-605">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="884bc-606">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="884bc-606">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="884bc-607">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="884bc-607">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="884bc-608">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-608">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-609">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-609">IoT</span></span>
* <span data-ttu-id="884bc-610">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="884bc-610">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="884bc-611">Kusto</span><span class="sxs-lookup"><span data-stu-id="884bc-611">Kusto</span></span>
* <span data-ttu-id="884bc-612">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="884bc-612">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-613">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-613">Monitor</span></span>
* <span data-ttu-id="884bc-614">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="884bc-614">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="884bc-615">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-615">Profile</span></span>
* <span data-ttu-id="884bc-616">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-616">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="884bc-617">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-617">Network</span></span>
* <span data-ttu-id="884bc-618">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="884bc-618">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="884bc-619">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="884bc-619">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-620">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-620">Resource</span></span>
* <span data-ttu-id="884bc-621">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-621">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="884bc-622">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-622">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="884bc-623">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-623">SQL Virtual Machine</span></span>
* <span data-ttu-id="884bc-624">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="884bc-624">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-625">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-625">Storage</span></span>
* <span data-ttu-id="884bc-626">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="884bc-626">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="884bc-627">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="884bc-627">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-628">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-628">VM</span></span>
* <span data-ttu-id="884bc-629">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="884bc-629">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="884bc-630">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="884bc-630">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="884bc-631">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-631">January 15, 2019</span></span>

<span data-ttu-id="884bc-632">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="884bc-632">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-633">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-633">ACR</span></span>
* <span data-ttu-id="884bc-634">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="884bc-634">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="884bc-635">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="884bc-635">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="884bc-636">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="884bc-636">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="884bc-637">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-637">ACS</span></span>
* <span data-ttu-id="884bc-638">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="884bc-638">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-639">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-639">Appservice</span></span>
* <span data-ttu-id="884bc-640">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="884bc-640">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="884bc-641">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="884bc-641">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="884bc-642">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="884bc-642">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="884bc-643">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="884bc-643">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="884bc-644">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="884bc-644">Botservice</span></span>
* <span data-ttu-id="884bc-645">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-645">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="884bc-646">Настройка</span><span class="sxs-lookup"><span data-stu-id="884bc-646">Configure</span></span>
* <span data-ttu-id="884bc-647">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="884bc-647">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="884bc-648">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-648">CosmosDB</span></span>
* <span data-ttu-id="884bc-649">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="884bc-649">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="884bc-650">HDInsight</span><span class="sxs-lookup"><span data-stu-id="884bc-650">HDInsight</span></span>
* <span data-ttu-id="884bc-651">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="884bc-651">Added commands for managing applications</span></span>
* <span data-ttu-id="884bc-652">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="884bc-652">Added commands for managing script actions</span></span>
* <span data-ttu-id="884bc-653">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="884bc-653">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="884bc-654">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="884bc-654">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="884bc-655">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-655">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="884bc-656">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-656">Network</span></span>
* <span data-ttu-id="884bc-657">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="884bc-657">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="884bc-658">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="884bc-658">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="884bc-659">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="884bc-659">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="884bc-660">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-660">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="884bc-661">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-661">Role</span></span>
* <span data-ttu-id="884bc-662">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="884bc-662">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="884bc-663">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="884bc-663">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="884bc-664">Безопасность</span><span class="sxs-lookup"><span data-stu-id="884bc-664">Security</span></span>
* <span data-ttu-id="884bc-665">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="884bc-665">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-666">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-666">Storage</span></span>
* <span data-ttu-id="884bc-667">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="884bc-667">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="884bc-668">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="884bc-668">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="884bc-669">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="884bc-669">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="884bc-670">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="884bc-670">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="884bc-671">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="884bc-671">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-672">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-672">VM</span></span>
* <span data-ttu-id="884bc-673">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="884bc-673">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="884bc-674">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-674">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="884bc-675">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="884bc-675">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="884bc-676">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="884bc-676">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="884bc-677">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-677">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="884bc-678">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="884bc-678">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="884bc-679">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-679">December 20, 2018</span></span>

<span data-ttu-id="884bc-680">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="884bc-680">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="884bc-681">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-681">Appservice</span></span>
* <span data-ttu-id="884bc-682">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="884bc-682">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="884bc-683">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="884bc-683">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="884bc-684">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="884bc-684">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="884bc-685">IoT Central</span><span class="sxs-lookup"><span data-stu-id="884bc-685">IoTCentral</span></span>
* <span data-ttu-id="884bc-686">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="884bc-686">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="884bc-687">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-687">Role</span></span>
* <span data-ttu-id="884bc-688">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="884bc-688">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-689">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-689">SQL</span></span>
* <span data-ttu-id="884bc-690">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="884bc-690">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-691">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-691">VM</span></span>
* <span data-ttu-id="884bc-692">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-692">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="884bc-693">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-693">December 18, 2018</span></span>

<span data-ttu-id="884bc-694">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="884bc-694">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="884bc-695">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-695">ACR</span></span>
* <span data-ttu-id="884bc-696">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-696">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="884bc-697">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="884bc-697">Condensed the table layout for task list</span></span>
* <span data-ttu-id="884bc-698">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="884bc-698">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-699">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-699">ACS</span></span>
* <span data-ttu-id="884bc-700">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="884bc-700">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="884bc-701">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="884bc-701">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="884bc-702">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="884bc-702">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="884bc-703">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-703">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="884bc-704">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="884bc-704">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="884bc-705">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="884bc-705">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-706">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-706">Appservice</span></span>
* <span data-ttu-id="884bc-707">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="884bc-707">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="884bc-708">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="884bc-708">Botservice</span></span>
* <span data-ttu-id="884bc-709">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-709">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="884bc-710">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="884bc-710">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="884bc-711">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="884bc-711">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="884bc-712">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="884bc-712">Reduced Kudu network calls</span></span>
* <span data-ttu-id="884bc-713">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-713">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="884bc-714">Потребление</span><span class="sxs-lookup"><span data-stu-id="884bc-714">Consumption</span></span>
* <span data-ttu-id="884bc-715">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="884bc-715">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="884bc-716">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-716">CosmosDB</span></span>
* <span data-ttu-id="884bc-717">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="884bc-717">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="884bc-718">Maps</span><span class="sxs-lookup"><span data-stu-id="884bc-718">Maps</span></span>
* <span data-ttu-id="884bc-719">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="884bc-719">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="884bc-720">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-720">Network</span></span>
* <span data-ttu-id="884bc-721">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="884bc-721">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="884bc-722">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="884bc-722">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-723">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-723">Resource</span></span>
* <span data-ttu-id="884bc-724">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-724">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="884bc-725">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-725">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-726">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-726">Storage</span></span>
*  <span data-ttu-id="884bc-727">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="884bc-727">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-728">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-728">VM</span></span>
* <span data-ttu-id="884bc-729">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-729">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="884bc-730">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-730">December 4, 2018</span></span>

<span data-ttu-id="884bc-731">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="884bc-731">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="884bc-732">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-732">Core</span></span>
* <span data-ttu-id="884bc-733">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-733">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="884bc-734">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="884bc-734">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-735">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-735">Appservice</span></span>
* <span data-ttu-id="884bc-736">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="884bc-736">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="884bc-737">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="884bc-737">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="884bc-738">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-738">Network</span></span>
* <span data-ttu-id="884bc-739">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="884bc-739">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="884bc-740">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-740">Role</span></span>
* <span data-ttu-id="884bc-741">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="884bc-741">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="884bc-742">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-742">VM</span></span>
* <span data-ttu-id="884bc-743">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="884bc-743">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="884bc-744">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="884bc-744">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="884bc-745">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="884bc-745">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="884bc-746">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="884bc-746">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="884bc-747">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-747">November 20, 2018</span></span>

<span data-ttu-id="884bc-748">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="884bc-748">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="884bc-749">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-749">Core</span></span>
* <span data-ttu-id="884bc-750">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="884bc-750">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-751">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-751">ACR</span></span>
* <span data-ttu-id="884bc-752">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="884bc-752">Added context token to task step</span></span>
* <span data-ttu-id="884bc-753">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="884bc-753">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="884bc-754">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="884bc-754">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-755">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-755">Appservice</span></span>
* <span data-ttu-id="884bc-756">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="884bc-756">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="884bc-757">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-757">Updated the default `node_version`.</span></span> <span data-ttu-id="884bc-758">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="884bc-758">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="884bc-759">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="884bc-759">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="884bc-760">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="884bc-760">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="884bc-761">IotCentral</span><span class="sxs-lookup"><span data-stu-id="884bc-761">IotCentral</span></span>
* <span data-ttu-id="884bc-762">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="884bc-762">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="884bc-763">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="884bc-763">KeyVault</span></span>
* <span data-ttu-id="884bc-764">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="884bc-764">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="884bc-765">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-765">Network</span></span>
* <span data-ttu-id="884bc-766">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="884bc-766">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="884bc-767">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="884bc-767">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="884bc-768">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="884bc-768">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="884bc-769">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="884bc-769">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="884bc-770">Rdbms</span><span class="sxs-lookup"><span data-stu-id="884bc-770">Rdbms</span></span>
* <span data-ttu-id="884bc-771">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="884bc-771">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="884bc-772">RBAC:</span><span class="sxs-lookup"><span data-stu-id="884bc-772">Rbac</span></span>
* <span data-ttu-id="884bc-773">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-773">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="884bc-774">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="884bc-774">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="884bc-775">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-775">Storage</span></span>
* <span data-ttu-id="884bc-776">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="884bc-776">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="884bc-777">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="884bc-777">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="884bc-778">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="884bc-778">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="884bc-779">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="884bc-779">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-780">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-780">VM</span></span>
* <span data-ttu-id="884bc-781">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="884bc-781">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="884bc-782">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="884bc-782">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="884bc-783">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="884bc-783">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="884bc-784">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="884bc-784">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="884bc-785">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-785">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="884bc-786">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-786">Added `snapshot wait` command</span></span>
* <span data-ttu-id="884bc-787">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="884bc-787">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="884bc-788">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-788">November 6, 2018</span></span>

<span data-ttu-id="884bc-789">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="884bc-789">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="884bc-790">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-790">Core</span></span>
* <span data-ttu-id="884bc-791">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="884bc-791">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-792">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-792">ACR</span></span>
* <span data-ttu-id="884bc-793">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="884bc-793">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="884bc-794">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="884bc-794">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-795">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-795">ACS</span></span>
* <span data-ttu-id="884bc-796">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-796">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="884bc-797">Помощник</span><span class="sxs-lookup"><span data-stu-id="884bc-797">Advisor</span></span>
* <span data-ttu-id="884bc-798">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="884bc-798">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="884bc-799">AMS</span><span class="sxs-lookup"><span data-stu-id="884bc-799">AMS</span></span>
* <span data-ttu-id="884bc-800">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="884bc-800">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="884bc-801">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="884bc-801">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="884bc-802">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-802">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="884bc-803">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="884bc-803">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="884bc-804">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="884bc-804">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="884bc-805">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="884bc-805">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="884bc-806">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="884bc-806">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="884bc-807">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="884bc-807">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="884bc-808">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="884bc-808">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="884bc-809">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="884bc-809">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="884bc-810">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="884bc-810">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="884bc-811">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="884bc-811">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="884bc-812">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="884bc-812">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="884bc-813">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="884bc-813">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="884bc-814">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="884bc-814">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="884bc-815">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="884bc-815">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="884bc-816">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="884bc-816">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-817">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-817">AppService</span></span>
* <span data-ttu-id="884bc-818">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="884bc-818">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="884bc-819">Настройка</span><span class="sxs-lookup"><span data-stu-id="884bc-819">Configure</span></span>
* <span data-ttu-id="884bc-820">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="884bc-820">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="884bc-821">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-821">Container</span></span>
* <span data-ttu-id="884bc-822">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="884bc-822">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="884bc-823">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="884bc-823">EventHub</span></span>
* <span data-ttu-id="884bc-824">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-824">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-825">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-825">Interactive</span></span>
* <span data-ttu-id="884bc-826">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="884bc-826">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-827">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-827">Monitor</span></span>
* <span data-ttu-id="884bc-828">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-828">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="884bc-829">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-829">Network</span></span>
* <span data-ttu-id="884bc-830">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="884bc-830">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="884bc-831">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="884bc-831">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="884bc-832">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-832">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="884bc-833">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-833">Profile</span></span>
* <span data-ttu-id="884bc-834">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="884bc-834">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="884bc-835">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="884bc-835">RDBMS</span></span>
* <span data-ttu-id="884bc-836">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="884bc-836">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-837">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-837">Resource</span></span>
* <span data-ttu-id="884bc-838">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="884bc-838">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="884bc-839">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-839">Role</span></span>
* <span data-ttu-id="884bc-840">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="884bc-840">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="884bc-841">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-841">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="884bc-842">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="884bc-842">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-843">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-843">Storage</span></span>
* <span data-ttu-id="884bc-844">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="884bc-844">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-845">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-845">VM</span></span>
* <span data-ttu-id="884bc-846">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="884bc-846">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="884bc-847">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="884bc-847">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="884bc-848">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="884bc-848">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="884bc-849">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="884bc-849">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="884bc-850">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="884bc-850">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="884bc-851">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="884bc-851">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="884bc-852">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-852">October 23, 2018</span></span>

<span data-ttu-id="884bc-853">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="884bc-853">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="884bc-854">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-854">Core</span></span>
* <span data-ttu-id="884bc-855">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="884bc-855">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="884bc-856">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="884bc-856">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-857">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-857">ACR</span></span>
* <span data-ttu-id="884bc-858">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="884bc-858">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="884bc-859">CDN</span><span class="sxs-lookup"><span data-stu-id="884bc-859">CDN</span></span>
* <span data-ttu-id="884bc-860">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-860">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="884bc-861">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="884bc-861">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="884bc-862">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-862">Container</span></span>
* <span data-ttu-id="884bc-863">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="884bc-863">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="884bc-864">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="884bc-864">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="884bc-865">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="884bc-865">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="884bc-866">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-866">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="884bc-867">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="884bc-867">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="884bc-868">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="884bc-868">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="884bc-869">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-869">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="884bc-870">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-870">CosmosDB</span></span>
* <span data-ttu-id="884bc-871">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="884bc-871">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-872">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-872">Interactive</span></span>
* <span data-ttu-id="884bc-873">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="884bc-873">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="884bc-874">IoT Central</span><span class="sxs-lookup"><span data-stu-id="884bc-874">IoT Central</span></span>
* <span data-ttu-id="884bc-875">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="884bc-875">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="884bc-876">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="884bc-876">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-877">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-877">Monitor</span></span>
* <span data-ttu-id="884bc-878">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="884bc-878">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="884bc-879">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="884bc-879">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="884bc-880">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="884bc-880">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="884bc-881">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="884bc-881">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="884bc-882">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="884bc-882">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="884bc-883">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="884bc-883">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="884bc-884">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="884bc-884">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="884bc-885">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="884bc-885">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="884bc-886">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="884bc-886">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="884bc-887">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-887">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="884bc-888">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-888">Network</span></span>
* <span data-ttu-id="884bc-889">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="884bc-889">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="884bc-890">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="884bc-890">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="884bc-891">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="884bc-891">ServiceBus</span></span>
* <span data-ttu-id="884bc-892">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="884bc-892">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-893">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-893">SQL</span></span>
* <span data-ttu-id="884bc-894">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="884bc-894">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-895">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-895">Storage</span></span>
* <span data-ttu-id="884bc-896">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-896">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="884bc-897">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="884bc-897">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-898">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-898">VM</span></span>
* <span data-ttu-id="884bc-899">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="884bc-899">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="884bc-900">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="884bc-900">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="884bc-901">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="884bc-901">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="884bc-902">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-902">October 16, 2018</span></span>

<span data-ttu-id="884bc-903">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="884bc-903">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-904">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-904">VM</span></span>
* <span data-ttu-id="884bc-905">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="884bc-905">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="884bc-906">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-906">October 9, 2018</span></span>

<span data-ttu-id="884bc-907">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="884bc-907">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="884bc-908">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-908">Core</span></span>
* <span data-ttu-id="884bc-909">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="884bc-909">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-910">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-910">ACR</span></span>
* <span data-ttu-id="884bc-911">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="884bc-911">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-912">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-912">ACS</span></span>
* <span data-ttu-id="884bc-913">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="884bc-913">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="884bc-914">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="884bc-914">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="884bc-915">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="884bc-915">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="884bc-916">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="884bc-916">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="884bc-917">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-917">Container</span></span>
* <span data-ttu-id="884bc-918">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="884bc-918">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="884bc-919">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="884bc-919">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="884bc-920">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="884bc-920">Event Hub</span></span>
* <span data-ttu-id="884bc-921">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-921">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="884bc-922">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="884bc-922">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="884bc-923">расширения.</span><span class="sxs-lookup"><span data-stu-id="884bc-923">Extensions</span></span>
* <span data-ttu-id="884bc-924">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="884bc-924">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="884bc-925">HDInsight</span><span class="sxs-lookup"><span data-stu-id="884bc-925">HDInsight</span></span>
* <span data-ttu-id="884bc-926">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="884bc-926">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-927">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-927">IoT</span></span>
* <span data-ttu-id="884bc-928">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="884bc-928">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="884bc-929">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="884bc-929">KeyVault</span></span>
* <span data-ttu-id="884bc-930">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="884bc-930">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="884bc-931">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-931">Network</span></span>
* <span data-ttu-id="884bc-932">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-932">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="884bc-933">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="884bc-933">See #6052</span></span>
* <span data-ttu-id="884bc-934">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-934">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="884bc-935">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="884bc-935">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="884bc-936">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="884bc-936">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="884bc-937">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="884bc-937">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="884bc-938">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="884bc-938">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="884bc-939">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-939">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="884bc-940">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-940">Role</span></span>
* <span data-ttu-id="884bc-941">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="884bc-941">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="884bc-942">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="884bc-942">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="884bc-943">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="884bc-943">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="884bc-944">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="884bc-944">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="884bc-945">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-945">Service Bus</span></span>
* <span data-ttu-id="884bc-946">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="884bc-946">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-947">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-947">VM</span></span>
* <span data-ttu-id="884bc-948">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="884bc-948">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="884bc-949">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="884bc-949">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="884bc-950">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="884bc-950">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="884bc-951">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="884bc-951">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="884bc-952">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="884bc-952">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="884bc-953">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="884bc-953">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="884bc-954">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-954">September 21, 2018</span></span>

<span data-ttu-id="884bc-955">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="884bc-955">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-956">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-956">ACR</span></span>
* <span data-ttu-id="884bc-957">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="884bc-957">Added ACR Task commands</span></span>
* <span data-ttu-id="884bc-958">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="884bc-958">Added quick run command</span></span>
* <span data-ttu-id="884bc-959">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="884bc-959">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="884bc-960">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="884bc-960">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="884bc-961">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="884bc-961">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="884bc-962">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="884bc-962">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-963">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-963">ACS</span></span>
* <span data-ttu-id="884bc-964">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="884bc-964">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="884bc-965">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="884bc-965">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-966">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-966">AppService</span></span>

* <span data-ttu-id="884bc-967">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="884bc-967">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="884bc-968">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="884bc-968">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="884bc-969">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="884bc-969">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="884bc-970">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="884bc-970">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-971">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-971">Batch</span></span>
* <span data-ttu-id="884bc-972">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="884bc-972">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="884bc-973">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="884bc-973">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="884bc-974">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-974">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="884bc-975">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="884bc-975">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="884bc-976">Azure Batch AI</span><span class="sxs-lookup"><span data-stu-id="884bc-976">Batch AI</span></span> 
* <span data-ttu-id="884bc-977">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-977">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="884bc-978">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="884bc-978">Cognitive Services</span></span>
* <span data-ttu-id="884bc-979">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="884bc-979">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="884bc-980">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="884bc-980">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="884bc-981">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="884bc-981">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="884bc-982">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="884bc-982">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="884bc-983">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="884bc-983">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="884bc-984">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="884bc-984">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="884bc-985">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-985">Container</span></span>
* <span data-ttu-id="884bc-986">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-986">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="884bc-987">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="884bc-987">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="884bc-988">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="884bc-988">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="884bc-989">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-989">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="884bc-990">Data Lake</span><span class="sxs-lookup"><span data-stu-id="884bc-990">Datalake</span></span>
* <span data-ttu-id="884bc-991">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="884bc-991">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="884bc-992">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="884bc-992">Interactive Shell</span></span>
* <span data-ttu-id="884bc-993">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-993">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="884bc-994">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="884bc-994">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-995">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-995">IoT</span></span>
* <span data-ttu-id="884bc-996">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="884bc-996">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="884bc-997">Key Vault</span><span class="sxs-lookup"><span data-stu-id="884bc-997">Key Vault</span></span>
* <span data-ttu-id="884bc-998">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="884bc-998">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="884bc-999">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-999">Network</span></span>
* <span data-ttu-id="884bc-1000">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1000">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="884bc-1001">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-1001">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="884bc-1002">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="884bc-1002">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="884bc-1003">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1003">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="884bc-1004">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1004">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="884bc-1005">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1005">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="884bc-1006">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="884bc-1006">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="884bc-1007">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1007">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="884bc-1008">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1008">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="884bc-1009">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1009">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="884bc-1010">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1010">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="884bc-1011">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1011">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="884bc-1012">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1012">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="884bc-1013">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="884bc-1013">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="884bc-1014">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1014">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="884bc-1015">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="884bc-1015">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="884bc-1016">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="884bc-1016">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="884bc-1017">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="884bc-1017">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="884bc-1018">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="884bc-1018">RDBMS</span></span>
* <span data-ttu-id="884bc-1019">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="884bc-1019">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="884bc-1020">резервирование.</span><span class="sxs-lookup"><span data-stu-id="884bc-1020">Reservation</span></span>
* <span data-ttu-id="884bc-1021">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1021">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="884bc-1022">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="884bc-1022">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="884bc-1023">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="884bc-1023">Manage App</span></span>
* <span data-ttu-id="884bc-1024">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="884bc-1024">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="884bc-1025">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="884bc-1025">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="884bc-1026">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-1026">Role</span></span>
* <span data-ttu-id="884bc-1027">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="884bc-1027">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="884bc-1028">SignalR</span><span class="sxs-lookup"><span data-stu-id="884bc-1028">SignalR</span></span>
* <span data-ttu-id="884bc-1029">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="884bc-1029">First release</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1030">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1030">Storage</span></span>
* <span data-ttu-id="884bc-1031">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="884bc-1031">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="884bc-1032">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="884bc-1032">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1033">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1033">VM</span></span>
* <span data-ttu-id="884bc-1034">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="884bc-1034">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="884bc-1035">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1035">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="884bc-1036">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1036">August 28, 2018</span></span>

<span data-ttu-id="884bc-1037">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="884bc-1037">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1038">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1038">Core</span></span>

* <span data-ttu-id="884bc-1039">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="884bc-1039">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="884bc-1040">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="884bc-1040">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1041">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1041">ACR</span></span>

* <span data-ttu-id="884bc-1042">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="884bc-1042">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="884bc-1043">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1043">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1044">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1044">ACS</span></span>

* <span data-ttu-id="884bc-1045">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1045">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="884bc-1046">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="884bc-1046">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1047">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-1047">AppService</span></span>

* <span data-ttu-id="884bc-1048">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="884bc-1048">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="884bc-1049">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="884bc-1049">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="884bc-1050">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="884bc-1050">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="884bc-1051">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="884bc-1051">Backup</span></span>

* <span data-ttu-id="884bc-1052">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="884bc-1052">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="884bc-1053">Служба Azure Bot</span><span class="sxs-lookup"><span data-stu-id="884bc-1053">Bot Service</span></span>

* <span data-ttu-id="884bc-1054">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="884bc-1054">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="884bc-1055">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="884bc-1055">Cognitive Services</span></span>

* <span data-ttu-id="884bc-1056">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="884bc-1056">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-1057">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-1057">IoT</span></span>

* <span data-ttu-id="884bc-1058">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="884bc-1058">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-1059">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-1059">Monitor</span></span>

* <span data-ttu-id="884bc-1060">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="884bc-1060">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="884bc-1061">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="884bc-1061">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1062">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1062">Network</span></span>

* <span data-ttu-id="884bc-1063">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="884bc-1063">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-1064">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-1064">Resource</span></span>

* <span data-ttu-id="884bc-1065">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="884bc-1065">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1066">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1066">Storage</span></span>

* <span data-ttu-id="884bc-1067">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="884bc-1067">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1068">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1068">VM</span></span>

* <span data-ttu-id="884bc-1069">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="884bc-1069">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="884bc-1070">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1070">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="884bc-1071">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1071">Auguest 14, 2018</span></span>

<span data-ttu-id="884bc-1072">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="884bc-1072">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1073">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1073">Core</span></span>

* <span data-ttu-id="884bc-1074">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1074">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="884bc-1075">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="884bc-1075">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="884bc-1076">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="884bc-1076">Telemetry</span></span>

* <span data-ttu-id="884bc-1077">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="884bc-1077">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1078">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1078">ACR</span></span>

* <span data-ttu-id="884bc-1079">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1079">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="884bc-1080">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1080">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1081">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1081">ACS</span></span>

* <span data-ttu-id="884bc-1082">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="884bc-1082">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="884bc-1083">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="884bc-1083">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="884bc-1084">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="884bc-1084">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="884bc-1085">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="884bc-1085">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="884bc-1086">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="884bc-1086">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="884bc-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-1087">AppService</span></span>

* <span data-ttu-id="884bc-1088">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1088">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="884bc-1089">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="884bc-1089">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="884bc-1090">Batch AI</span><span class="sxs-lookup"><span data-stu-id="884bc-1090">BatchAI</span></span>

* <span data-ttu-id="884bc-1091">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="884bc-1091">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="884bc-1092">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1092">Container</span></span>

* <span data-ttu-id="884bc-1093">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="884bc-1093">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="884bc-1094">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-1094">IoT</span></span>

* <span data-ttu-id="884bc-1095">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="884bc-1095">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="884bc-1096">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1096">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="884bc-1097">IoT Central</span><span class="sxs-lookup"><span data-stu-id="884bc-1097">Iot Central</span></span>

* <span data-ttu-id="884bc-1098">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="884bc-1098">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="884bc-1099">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="884bc-1099">KeyVault</span></span>


* <span data-ttu-id="884bc-1100">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="884bc-1100">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="884bc-1101">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="884bc-1101">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="884bc-1102">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="884bc-1102">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="884bc-1103">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="884bc-1103">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="884bc-1104">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="884bc-1104">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="884bc-1105">Передача</span><span class="sxs-lookup"><span data-stu-id="884bc-1105">Relay</span></span>

* <span data-ttu-id="884bc-1106">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="884bc-1106">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-1107">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-1107">Sql</span></span>

* <span data-ttu-id="884bc-1108">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1108">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1109">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1109">Storage</span></span>

* <span data-ttu-id="884bc-1110">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="884bc-1110">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="884bc-1111">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="884bc-1111">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="884bc-1112">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="884bc-1112">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="884bc-1113">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="884bc-1113">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="884bc-1114">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="884bc-1114">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1115">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1115">VM</span></span>

* <span data-ttu-id="884bc-1116">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="884bc-1116">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="884bc-1117">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1117">July 31, 2018</span></span>

<span data-ttu-id="884bc-1118">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="884bc-1118">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1119">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1119">ACR</span></span>

* <span data-ttu-id="884bc-1120">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1120">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="884bc-1121">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1121">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1122">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1122">ACS</span></span>

* <span data-ttu-id="884bc-1123">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="884bc-1123">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-1124">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-1124">Batch</span></span>

* <span data-ttu-id="884bc-1125">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="884bc-1125">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1126">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1126">Container</span></span>

* <span data-ttu-id="884bc-1127">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1127">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1128">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1128">Network</span></span>

* <span data-ttu-id="884bc-1129">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="884bc-1129">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="884bc-1130">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-1130">Resource</span></span>

* <span data-ttu-id="884bc-1131">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1131">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="884bc-1132">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="884bc-1132">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="884bc-1133">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-1133">Role</span></span>

* <span data-ttu-id="884bc-1134">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="884bc-1134">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="884bc-1135">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="884bc-1135">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="884bc-1136">Поиск</span><span class="sxs-lookup"><span data-stu-id="884bc-1136">Search</span></span>

* <span data-ttu-id="884bc-1137">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="884bc-1137">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="884bc-1138">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-1138">Service Bus</span></span>

* <span data-ttu-id="884bc-1139">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="884bc-1139">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="884bc-1140">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="884bc-1140">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="884bc-1141">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="884bc-1141">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="884bc-1142">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1142">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1143">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1143">Storage</span></span>

* <span data-ttu-id="884bc-1144">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="884bc-1144">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="884bc-1145">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="884bc-1145">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1146">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1146">VM</span></span>

* <span data-ttu-id="884bc-1147">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="884bc-1147">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="884bc-1148">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1148">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="884bc-1149">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="884bc-1149">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="884bc-1150">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="884bc-1150">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="884bc-1151">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1151">July 18, 2018</span></span>

<span data-ttu-id="884bc-1152">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="884bc-1152">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1153">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1153">Core</span></span>

* <span data-ttu-id="884bc-1154">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="884bc-1154">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="884bc-1155">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="884bc-1155">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="884bc-1156">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="884bc-1156">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1157">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1157">ACR</span></span>

* <span data-ttu-id="884bc-1158">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="884bc-1158">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="884bc-1159">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1159">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="884bc-1160">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="884bc-1160">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="884bc-1161">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="884bc-1161">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1162">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1162">ACS</span></span>

* <span data-ttu-id="884bc-1163">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="884bc-1163">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1164">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-1164">AppService</span></span>

* <span data-ttu-id="884bc-1165">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="884bc-1165">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-1166">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-1166">Batch</span></span>

* <span data-ttu-id="884bc-1167">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="884bc-1167">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="884bc-1168">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="884bc-1168">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="884bc-1169">Azure Batch AI</span><span class="sxs-lookup"><span data-stu-id="884bc-1169">Batch AI</span></span>

* <span data-ttu-id="884bc-1170">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1170">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1171">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1171">Container</span></span>

* <span data-ttu-id="884bc-1172">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="884bc-1172">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="884bc-1173">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="884bc-1173">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1174">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1174">Network</span></span>

* <span data-ttu-id="884bc-1175">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1175">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="884bc-1176">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1176">Added `network nic wait`</span></span>
* <span data-ttu-id="884bc-1177">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="884bc-1177">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="884bc-1178">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="884bc-1178">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="884bc-1179">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-1179">Resource</span></span>

* <span data-ttu-id="884bc-1180">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1180">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="884bc-1181">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1181">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="884bc-1182">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1182">Added `deployment wait` command</span></span>
* <span data-ttu-id="884bc-1183">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="884bc-1183">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-1184">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-1184">SQL</span></span>

* <span data-ttu-id="884bc-1185">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1185">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="884bc-1186">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1186">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="884bc-1187">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1187">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1188">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1188">Storage</span></span>

* <span data-ttu-id="884bc-1189">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1189">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1190">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1190">VM</span></span>

* <span data-ttu-id="884bc-1191">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-1191">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="884bc-1192">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1192">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="884bc-1193">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1193">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="884bc-1194">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1194">July 3, 2018</span></span>

<span data-ttu-id="884bc-1195">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="884bc-1195">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="884bc-1196">AKS</span><span class="sxs-lookup"><span data-stu-id="884bc-1196">AKS</span></span>

* <span data-ttu-id="884bc-1197">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1197">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="884bc-1198">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1198">July 3, 2018</span></span>

<span data-ttu-id="884bc-1199">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="884bc-1199">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1200">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1200">Core</span></span>

* <span data-ttu-id="884bc-1201">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="884bc-1201">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1202">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1202">ACR</span></span>

* <span data-ttu-id="884bc-1203">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="884bc-1203">Added polling build status</span></span>
* <span data-ttu-id="884bc-1204">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="884bc-1204">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="884bc-1205">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1205">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1206">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1206">ACS</span></span>

* <span data-ttu-id="884bc-1207">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-1207">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="884bc-1208">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-1208">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="884bc-1209">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1209">Updated options for `aks browse` command.</span></span> <span data-ttu-id="884bc-1210">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1210">Added `--listen-port` support</span></span>
* <span data-ttu-id="884bc-1211">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1211">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="884bc-1212">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="884bc-1212">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="884bc-1213">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1213">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1214">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-1214">AppService</span></span>

* <span data-ttu-id="884bc-1215">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1215">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="884bc-1216">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="884bc-1216">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="884bc-1217">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="884bc-1217">Backup</span></span>

* <span data-ttu-id="884bc-1218">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="884bc-1218">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="884bc-1219">Batch AI</span><span class="sxs-lookup"><span data-stu-id="884bc-1219">BatchAI</span></span>

* <span data-ttu-id="884bc-1220">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1220">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="884bc-1221">Облако</span><span class="sxs-lookup"><span data-stu-id="884bc-1221">Cloud</span></span>

* <span data-ttu-id="884bc-1222">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1222">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1223">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1223">Container</span></span>

* <span data-ttu-id="884bc-1224">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="884bc-1224">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="884bc-1225">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1225">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="884bc-1226">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="884bc-1226">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="884bc-1227">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="884bc-1227">Extension</span></span>

* <span data-ttu-id="884bc-1228">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="884bc-1228">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1229">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1229">Network</span></span>

* <span data-ttu-id="884bc-1230">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="884bc-1230">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="884bc-1231">Rdbms</span><span class="sxs-lookup"><span data-stu-id="884bc-1231">Rdbms</span></span>

* <span data-ttu-id="884bc-1232">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1232">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-1233">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-1233">Resource</span></span>

* <span data-ttu-id="884bc-1234">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1234">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1235">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1235">VM</span></span>

* <span data-ttu-id="884bc-1236">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="884bc-1236">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="884bc-1237">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1237">June 25, 2018</span></span>

<span data-ttu-id="884bc-1238">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="884bc-1238">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="884bc-1239">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="884bc-1239">CLI</span></span>

* <span data-ttu-id="884bc-1240">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="884bc-1240">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="884bc-1241">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1241">June 19, 2018</span></span>

<span data-ttu-id="884bc-1242">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="884bc-1242">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1243">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1243">Core</span></span>

* <span data-ttu-id="884bc-1244">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-1244">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1245">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1245">ACR</span></span>

* <span data-ttu-id="884bc-1246">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1246">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="884bc-1247">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="884bc-1247">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1248">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1248">ACS</span></span>

* <span data-ttu-id="884bc-1249">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1249">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="884bc-1250">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1250">Added `--update` support</span></span>
* <span data-ttu-id="884bc-1251">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1251">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="884bc-1252">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1252">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="884bc-1253">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1253">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="884bc-1254">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1254">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="884bc-1255">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1255">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="884bc-1256">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1256">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1257">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-1257">AppService</span></span>

* <span data-ttu-id="884bc-1258">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="884bc-1258">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="884bc-1259">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1259">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-1260">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-1260">Batch</span></span>

* <span data-ttu-id="884bc-1261">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1261">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="884bc-1262">Azure Batch AI</span><span class="sxs-lookup"><span data-stu-id="884bc-1262">Batch AI</span></span>

* <span data-ttu-id="884bc-1263">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="884bc-1263">Added support for workspaces.</span></span> <span data-ttu-id="884bc-1264">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1264">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="884bc-1265">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1265">Added support for experiments.</span></span> <span data-ttu-id="884bc-1266">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="884bc-1266">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="884bc-1267">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="884bc-1267">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="884bc-1268">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1268">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="884bc-1269">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1269">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="884bc-1270">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1270">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="884bc-1271">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="884bc-1271">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="884bc-1272">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1272">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="884bc-1273">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1273">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="884bc-1274">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1274">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="884bc-1275">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1275">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="884bc-1276">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1276">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="884bc-1277">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1277">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="884bc-1278">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="884bc-1278">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="884bc-1279">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1279">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="884bc-1280">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="884bc-1280">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="884bc-1281">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="884bc-1281">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="884bc-1282">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="884bc-1282">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="884bc-1283">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="884bc-1283">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="884bc-1284">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="884bc-1284">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="884bc-1285">Maps</span><span class="sxs-lookup"><span data-stu-id="884bc-1285">Maps</span></span>

* <span data-ttu-id="884bc-1286">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1286">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1287">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1287">Network</span></span>

* <span data-ttu-id="884bc-1288">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="884bc-1288">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="884bc-1289">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="884bc-1289">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="884bc-1290">#6502</span><span class="sxs-lookup"><span data-stu-id="884bc-1290">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="884bc-1291">Резервирование</span><span class="sxs-lookup"><span data-stu-id="884bc-1291">Reservations</span></span>

* <span data-ttu-id="884bc-1292">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1292">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="884bc-1293">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1293">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="884bc-1294">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1294">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="884bc-1295">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1295">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="884bc-1296">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1296">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="884bc-1297">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1297">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="884bc-1298">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-1298">Role</span></span>

* <span data-ttu-id="884bc-1299">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="884bc-1299">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-1300">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-1300">SQL</span></span>

* <span data-ttu-id="884bc-1301">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1301">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1302">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1302">Storage</span></span>

* <span data-ttu-id="884bc-1303">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="884bc-1303">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1304">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1304">VM</span></span>

* <span data-ttu-id="884bc-1305">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1305">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="884bc-1306">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1306">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="884bc-1307">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="884bc-1307">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="884bc-1308">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1308">June 13, 2018</span></span>

<span data-ttu-id="884bc-1309">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="884bc-1309">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1310">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1310">Core</span></span>

* <span data-ttu-id="884bc-1311">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="884bc-1311">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="884bc-1312">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1312">June 13, 2018</span></span>

<span data-ttu-id="884bc-1313">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="884bc-1313">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="884bc-1314">AKS</span><span class="sxs-lookup"><span data-stu-id="884bc-1314">AKS</span></span>

* <span data-ttu-id="884bc-1315">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="884bc-1315">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="884bc-1316">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="884bc-1316">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="884bc-1317">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="884bc-1317">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="884bc-1318">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="884bc-1318">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="884bc-1319">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="884bc-1319">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1320">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-1320">AppService</span></span>

* <span data-ttu-id="884bc-1321">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="884bc-1321">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="884bc-1322">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1322">June 5, 2018</span></span>

<span data-ttu-id="884bc-1323">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="884bc-1323">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-1324">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-1324">Interactive</span></span>

* <span data-ttu-id="884bc-1325">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="884bc-1325">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="884bc-1326">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1326">June 5, 2018</span></span>

<span data-ttu-id="884bc-1327">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="884bc-1327">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1328">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1328">Core</span></span>

* <span data-ttu-id="884bc-1329">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="884bc-1329">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="884bc-1330">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="884bc-1330">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1331">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1331">ACR</span></span>

* <span data-ttu-id="884bc-1332">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="884bc-1332">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="884bc-1333">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1333">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="884bc-1334">AKS</span><span class="sxs-lookup"><span data-stu-id="884bc-1334">AKS</span></span>

* <span data-ttu-id="884bc-1335">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="884bc-1335">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-1336">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-1336">Batch</span></span>

* <span data-ttu-id="884bc-1337">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="884bc-1337">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-1338">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-1338">IOT</span></span>

* <span data-ttu-id="884bc-1339">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="884bc-1339">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1340">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1340">Network</span></span>

* <span data-ttu-id="884bc-1341">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1341">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="884bc-1342">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="884bc-1342">Policy Insights</span></span>

* <span data-ttu-id="884bc-1343">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="884bc-1343">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="884bc-1344">ARM</span><span class="sxs-lookup"><span data-stu-id="884bc-1344">ARM</span></span>

* <span data-ttu-id="884bc-1345">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1345">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-1346">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-1346">SQL</span></span>

* <span data-ttu-id="884bc-1347">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="884bc-1347">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="884bc-1348">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="884bc-1348">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="884bc-1349">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1349">Storage</span></span>

* <span data-ttu-id="884bc-1350">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1350">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1351">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1351">VM</span></span>

* <span data-ttu-id="884bc-1352">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1352">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="884bc-1353">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1353">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="884bc-1354">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1354">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="884bc-1355">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1355">May 22, 2018</span></span>

<span data-ttu-id="884bc-1356">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="884bc-1356">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1357">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1357">Core</span></span>

* <span data-ttu-id="884bc-1358">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1358">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1359">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1359">ACS</span></span>

* <span data-ttu-id="884bc-1360">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1360">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="884bc-1361">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="884bc-1361">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1362">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-1362">AppService</span></span>

* <span data-ttu-id="884bc-1363">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="884bc-1363">Improved generic update commands</span></span>
* <span data-ttu-id="884bc-1364">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1364">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1365">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1365">Container</span></span>

* <span data-ttu-id="884bc-1366">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="884bc-1366">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="884bc-1367">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-1367">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="884bc-1368">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="884bc-1368">Extension</span></span>

* <span data-ttu-id="884bc-1369">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="884bc-1369">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-1370">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-1370">Interactive</span></span>

* <span data-ttu-id="884bc-1371">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="884bc-1371">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="884bc-1372">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1372">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="884bc-1373">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="884bc-1373">KeyVault</span></span>

* <span data-ttu-id="884bc-1374">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="884bc-1374">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1375">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1375">Network</span></span>

* <span data-ttu-id="884bc-1376">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="884bc-1376">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="884bc-1377">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="884bc-1377">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-1378">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-1378">SQL</span></span>

* <span data-ttu-id="884bc-1379">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="884bc-1379">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="884bc-1380">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1380">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="884bc-1381">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1381">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="884bc-1382">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="884bc-1382">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="884bc-1383">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="884bc-1383">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="884bc-1384">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1384">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="884bc-1385">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1385">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="884bc-1386">`edition`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1386">`edition`.</span></span> <span data-ttu-id="884bc-1387">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1387">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="884bc-1388">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1388">`elasticPoolName`.</span></span> <span data-ttu-id="884bc-1389">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1389">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="884bc-1390">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="884bc-1390">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="884bc-1391">`edition`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1391">`edition`.</span></span> <span data-ttu-id="884bc-1392">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1392">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="884bc-1393">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1393">`dtu`.</span></span> <span data-ttu-id="884bc-1394">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1394">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="884bc-1395">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1395">`databaseDtuMin`.</span></span> <span data-ttu-id="884bc-1396">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1396">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="884bc-1397">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1397">`databaseDtuMax`.</span></span> <span data-ttu-id="884bc-1398">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1398">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="884bc-1399">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1399">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="884bc-1400">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1400">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1401">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1401">Storage</span></span>

* <span data-ttu-id="884bc-1402">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1402">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="884bc-1403">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1403">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1404">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1404">VM</span></span>

* <span data-ttu-id="884bc-1405">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1405">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="884bc-1406">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1406">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="884bc-1407">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1407">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="884bc-1408">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1408">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="884bc-1409">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1409">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="884bc-1410">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1410">May 7, 2018</span></span>

<span data-ttu-id="884bc-1411">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="884bc-1411">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1412">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1412">Core</span></span>

* <span data-ttu-id="884bc-1413">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="884bc-1413">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="884bc-1414">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1414">Added limited support for positional arguments</span></span>
* <span data-ttu-id="884bc-1415">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1415">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="884bc-1416">#5591</span><span class="sxs-lookup"><span data-stu-id="884bc-1416">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="884bc-1417">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1417">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="884bc-1418">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="884bc-1418">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="884bc-1419">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="884bc-1419">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="884bc-1420">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1420">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="884bc-1421">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="884bc-1421">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1422">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1422">ACR</span></span>

* <span data-ttu-id="884bc-1423">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="884bc-1423">Added ACR Build commands</span></span>
* <span data-ttu-id="884bc-1424">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="884bc-1424">Improved resource not found error messages</span></span>
* <span data-ttu-id="884bc-1425">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="884bc-1425">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="884bc-1426">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="884bc-1426">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="884bc-1427">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="884bc-1427">Improved repository commands error messages</span></span>
* <span data-ttu-id="884bc-1428">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="884bc-1428">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1429">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1429">ACS</span></span>

* <span data-ttu-id="884bc-1430">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-1430">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="884bc-1431">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="884bc-1431">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="884bc-1432">AMS</span><span class="sxs-lookup"><span data-stu-id="884bc-1432">AMS</span></span>

* <span data-ttu-id="884bc-1433">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="884bc-1433">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1434">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-1434">Appservice</span></span>

* <span data-ttu-id="884bc-1435">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="884bc-1435">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="884bc-1436">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1436">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="884bc-1437">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="884bc-1437">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="884bc-1438">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-1438">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="884bc-1439">Azure Batch AI</span><span class="sxs-lookup"><span data-stu-id="884bc-1439">Batch AI</span></span>

* <span data-ttu-id="884bc-1440">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="884bc-1440">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="884bc-1441">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="884bc-1441">Cognitive Services</span></span>

* <span data-ttu-id="884bc-1442">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="884bc-1442">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="884bc-1443">Потребление</span><span class="sxs-lookup"><span data-stu-id="884bc-1443">Consumption</span></span>

* <span data-ttu-id="884bc-1444">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="884bc-1444">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1445">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1445">Container</span></span>

* <span data-ttu-id="884bc-1446">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="884bc-1446">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="884bc-1447">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-1447">Cosmos DB</span></span>

* <span data-ttu-id="884bc-1448">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-1448">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="884bc-1449">DMS</span><span class="sxs-lookup"><span data-stu-id="884bc-1449">DMS</span></span>

* <span data-ttu-id="884bc-1450">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="884bc-1450">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="884bc-1451">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="884bc-1451">Extension</span></span>

* <span data-ttu-id="884bc-1452">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="884bc-1452">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-1453">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-1453">Interactive</span></span>

* <span data-ttu-id="884bc-1454">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="884bc-1454">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="884bc-1455">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="884bc-1455">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="884bc-1456">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1456">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="884bc-1457">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-1457">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="884bc-1458">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="884bc-1458">Lab</span></span>

* <span data-ttu-id="884bc-1459">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="884bc-1459">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1460">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1460">Network</span></span>

* <span data-ttu-id="884bc-1461">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="884bc-1461">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="884bc-1462">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-1462">Profile</span></span>

* <span data-ttu-id="884bc-1463">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1463">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="884bc-1464">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="884bc-1464">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="884bc-1465">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1465">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="884bc-1466">Redis</span><span class="sxs-lookup"><span data-stu-id="884bc-1466">Redis</span></span>

* <span data-ttu-id="884bc-1467">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1467">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="884bc-1468">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="884bc-1468">Deprecated `redis list-all`.</span></span> <span data-ttu-id="884bc-1469">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1469">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="884bc-1470">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1470">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="884bc-1471">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-1471">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="884bc-1472">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-1472">Role</span></span>

* <span data-ttu-id="884bc-1473">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="884bc-1473">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1474">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1474">Storage</span></span>

* <span data-ttu-id="884bc-1475">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="884bc-1475">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="884bc-1476">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="884bc-1476">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="884bc-1477">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="884bc-1477">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="884bc-1478">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="884bc-1478">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="884bc-1479">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="884bc-1479">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1480">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1480">VM</span></span>

* <span data-ttu-id="884bc-1481">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="884bc-1481">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="884bc-1482">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="884bc-1482">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="884bc-1483">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="884bc-1483">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="884bc-1484">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1484">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="884bc-1485">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="884bc-1485">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="884bc-1486">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="884bc-1486">Added write accelerator support</span></span>
* <span data-ttu-id="884bc-1487">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1487">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="884bc-1488">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="884bc-1488">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="884bc-1489">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="884bc-1489">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="884bc-1490">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1490">April 10, 2018</span></span>

<span data-ttu-id="884bc-1491">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="884bc-1491">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1492">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1492">ACR</span></span>

* <span data-ttu-id="884bc-1493">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="884bc-1493">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1494">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1494">ACS</span></span>

* <span data-ttu-id="884bc-1495">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="884bc-1495">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1496">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-1496">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="884bc-1498">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="884bc-1498">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="884bc-1499">Batch AI</span><span class="sxs-lookup"><span data-stu-id="884bc-1499">BatchAI</span></span>

* <span data-ttu-id="884bc-1500">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="884bc-1500">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="884bc-1501">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="884bc-1501">Job level mounting</span></span>
  - <span data-ttu-id="884bc-1502">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1502">Environment variables with secret values</span></span>
  - <span data-ttu-id="884bc-1503">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="884bc-1503">Performance counters settings</span></span>
  - <span data-ttu-id="884bc-1504">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="884bc-1504">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="884bc-1505">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1505">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="884bc-1506">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="884bc-1506">Usage and limits reporting</span></span>
  - <span data-ttu-id="884bc-1507">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1507">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="884bc-1508">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1508">Support for custom images</span></span>
  - <span data-ttu-id="884bc-1509">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="884bc-1509">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="884bc-1510">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="884bc-1510">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="884bc-1511">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1511">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="884bc-1512">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="884bc-1512">National clouds are supported</span></span>
* <span data-ttu-id="884bc-1513">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="884bc-1513">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="884bc-1514">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="884bc-1514">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="884bc-1515">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="884bc-1515">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="884bc-1516">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="884bc-1516">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="884bc-1517">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="884bc-1517">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="884bc-1518">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="884bc-1518">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="884bc-1519">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1519">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="884bc-1520">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="884bc-1520">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="884bc-1521">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="884bc-1521">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="884bc-1522">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1522">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="884bc-1523">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="884bc-1523">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="884bc-1524">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1524">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="884bc-1525">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1525">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="884bc-1526">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="884bc-1526">Billing</span></span>

* <span data-ttu-id="884bc-1527">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="884bc-1527">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="884bc-1528">Потребление</span><span class="sxs-lookup"><span data-stu-id="884bc-1528">Consumption</span></span>

* <span data-ttu-id="884bc-1529">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1529">Added `marketplace` commands</span></span>
* <span data-ttu-id="884bc-1530">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1530">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="884bc-1531">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1531">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="884bc-1532">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1532">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="884bc-1533">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1533">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="884bc-1534">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1534">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1535">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1535">Container</span></span>

* <span data-ttu-id="884bc-1536">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1536">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="884bc-1537">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="884bc-1537">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="884bc-1538">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="884bc-1538">Extension</span></span>

* <span data-ttu-id="884bc-1539">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1539">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-1540">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-1540">Interactive</span></span>

* <span data-ttu-id="884bc-1541">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="884bc-1541">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="884bc-1542">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-1542">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="884bc-1543">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1543">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1544">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1544">Network</span></span>

* <span data-ttu-id="884bc-1545">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1545">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="884bc-1546">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1546">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="884bc-1547">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="884bc-1547">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="884bc-1548">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="884bc-1548">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="884bc-1549">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="884bc-1549">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="884bc-1550">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1550">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="884bc-1551">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1551">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="884bc-1552">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="884bc-1552">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="884bc-1553">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-1553">Profile</span></span>

* <span data-ttu-id="884bc-1554">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1554">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="884bc-1555">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1555">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="884bc-1556">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="884bc-1556">RDBMS</span></span>

* <span data-ttu-id="884bc-1557">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1557">Added `georestore` command</span></span>
* <span data-ttu-id="884bc-1558">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="884bc-1558">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-1559">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-1559">Resource</span></span>

* <span data-ttu-id="884bc-1560">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1560">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="884bc-1561">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1561">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-1562">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-1562">SQL</span></span>

* <span data-ttu-id="884bc-1563">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1563">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1564">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1564">Storage</span></span>

* <span data-ttu-id="884bc-1565">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="884bc-1565">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1566">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1566">VM</span></span>

* <span data-ttu-id="884bc-1567">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="884bc-1567">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="884bc-1568">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="884bc-1568">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="884bc-1570">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1570">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="884bc-1571">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="884bc-1571">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="884bc-1572">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="884bc-1572">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="884bc-1573">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="884bc-1573">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="884bc-1574">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1574">March 27, 2018</span></span>

<span data-ttu-id="884bc-1575">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="884bc-1575">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1576">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1576">Core</span></span>

* <span data-ttu-id="884bc-1577">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="884bc-1577">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1578">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1578">ACS</span></span>

* <span data-ttu-id="884bc-1579">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="884bc-1579">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1580">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-1580">Appservice</span></span>

* <span data-ttu-id="884bc-1581">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1581">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="884bc-1582">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1582">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="884bc-1583">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="884bc-1583">Backup</span></span>

* <span data-ttu-id="884bc-1584">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1584">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="884bc-1585">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="884bc-1585">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="884bc-1586">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="884bc-1586">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="884bc-1587">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1587">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1588">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1588">Container</span></span>

* <span data-ttu-id="884bc-1589">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1589">Added `container exec` command.</span></span> <span data-ttu-id="884bc-1590">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-1590">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="884bc-1591">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-1591">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="884bc-1592">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="884bc-1592">Extension</span></span>

* <span data-ttu-id="884bc-1593">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="884bc-1593">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="884bc-1594">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1594">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="884bc-1595">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-1595">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-1596">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-1596">Interactive</span></span>

* <span data-ttu-id="884bc-1597">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-1597">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="884bc-1598">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1598">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="884bc-1599">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-1599">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="884bc-1600">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="884bc-1600">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="884bc-1601">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="884bc-1601">Lab</span></span>

* <span data-ttu-id="884bc-1602">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1602">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-1603">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-1603">Monitor</span></span>

* <span data-ttu-id="884bc-1604">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="884bc-1604">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="884bc-1605">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="884bc-1605">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="884bc-1606">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="884bc-1606">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1607">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1607">Network</span></span>

* <span data-ttu-id="884bc-1608">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="884bc-1608">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="884bc-1609">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-1609">Profile</span></span>

* <span data-ttu-id="884bc-1610">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1610">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="884bc-1611">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="884bc-1611">RDBMS</span></span>

* <span data-ttu-id="884bc-1612">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="884bc-1612">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-1613">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-1613">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="884bc-1615">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-1615">Role</span></span>

* <span data-ttu-id="884bc-1616">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1616">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="884bc-1617">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="884bc-1617">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="884bc-1618">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="884bc-1618">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="884bc-1619">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1619">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="884bc-1620">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1620">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1621">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1621">Storage</span></span>

* <span data-ttu-id="884bc-1622">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="884bc-1622">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="884bc-1623">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="884bc-1623">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1624">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1624">VM</span></span>

* <span data-ttu-id="884bc-1625">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="884bc-1625">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="884bc-1626">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1626">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="884bc-1627">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="884bc-1627">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="884bc-1628">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="884bc-1628">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="884bc-1629">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1629">March 13, 2018</span></span>

<span data-ttu-id="884bc-1630">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="884bc-1630">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1631">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1631">ACR</span></span>

* <span data-ttu-id="884bc-1632">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1632">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="884bc-1633">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="884bc-1633">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="884bc-1634">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="884bc-1634">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1635">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1635">ACS</span></span>

* <span data-ttu-id="884bc-1636">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="884bc-1636">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="884bc-1637">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1637">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="884bc-1638">Помощник</span><span class="sxs-lookup"><span data-stu-id="884bc-1638">Advisor</span></span>

* <span data-ttu-id="884bc-1639">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1639">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="884bc-1640">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1640">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="884bc-1641">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1641">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="884bc-1642">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1642">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="884bc-1643">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1643">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1644">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-1644">Appservice</span></span>

* <span data-ttu-id="884bc-1645">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="884bc-1645">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="884bc-1646">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1646">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="884bc-1647">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="884bc-1647">Eventhubs</span></span>

* <span data-ttu-id="884bc-1648">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="884bc-1648">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="884bc-1649">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="884bc-1649">Extension</span></span>

* <span data-ttu-id="884bc-1650">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="884bc-1650">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-1651">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-1651">Interactive</span></span>

* <span data-ttu-id="884bc-1652">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="884bc-1652">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="884bc-1653">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="884bc-1653">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="884bc-1654">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="884bc-1654">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="884bc-1655">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="884bc-1655">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-1656">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-1656">Monitor</span></span>

* <span data-ttu-id="884bc-1657">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="884bc-1657">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="884bc-1658">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1658">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="884bc-1659">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1659">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="884bc-1660">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1660">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1661">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1661">Network</span></span>

* <span data-ttu-id="884bc-1662">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1662">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="884bc-1663">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="884bc-1663">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="884bc-1664">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1664">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="884bc-1665">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1665">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="884bc-1666">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-1666">Profile</span></span>

* <span data-ttu-id="884bc-1667">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="884bc-1667">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="884bc-1668">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1668">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="884bc-1669">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="884bc-1669">RDBMS</span></span>

* <span data-ttu-id="884bc-1670">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="884bc-1670">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="884bc-1671">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-1671">Service Bus</span></span>

* <span data-ttu-id="884bc-1672">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="884bc-1672">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1673">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1673">Storage</span></span>

* <span data-ttu-id="884bc-1674">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="884bc-1674">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="884bc-1675">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="884bc-1675">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1676">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1676">VM</span></span>

* <span data-ttu-id="884bc-1677">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="884bc-1677">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="884bc-1678">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="884bc-1678">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="884bc-1679">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1679">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="884bc-1680">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="884bc-1680">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="884bc-1681">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="884bc-1681">February 27, 2018</span></span>

<span data-ttu-id="884bc-1682">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="884bc-1682">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1683">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1683">Core</span></span>

* <span data-ttu-id="884bc-1684">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="884bc-1684">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="884bc-1685">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="884bc-1685">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="884bc-1686">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1686">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1687">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1687">ACS</span></span>

* <span data-ttu-id="884bc-1688">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-1688">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="884bc-1689">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="884bc-1689">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="884bc-1690">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1690">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="884bc-1691">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1691">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1692">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-1692">Appservice</span></span>

* <span data-ttu-id="884bc-1693">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="884bc-1693">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="884bc-1694">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="884bc-1694">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="884bc-1695">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="884bc-1695">Cognitive Services</span></span>

* <span data-ttu-id="884bc-1696">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="884bc-1696">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="884bc-1697">Потребление</span><span class="sxs-lookup"><span data-stu-id="884bc-1697">Consumption</span></span>

* <span data-ttu-id="884bc-1698">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="884bc-1698">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="884bc-1699">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="884bc-1699">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1700">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1700">Container</span></span>

* <span data-ttu-id="884bc-1701">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="884bc-1701">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1702">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1702">Network</span></span>

* <span data-ttu-id="884bc-1703">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1703">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-1704">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-1704">Resource</span></span>

* <span data-ttu-id="884bc-1705">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="884bc-1705">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="884bc-1706">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-1706">Role</span></span>

* <span data-ttu-id="884bc-1707">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-1707">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-1708">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-1708">SQL</span></span>

* <span data-ttu-id="884bc-1709">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1709">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1710">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1710">Storage</span></span>

* <span data-ttu-id="884bc-1711">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1711">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1712">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1712">VM</span></span>

* <span data-ttu-id="884bc-1713">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="884bc-1713">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="884bc-1714">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1714">February 13, 2018</span></span>

<span data-ttu-id="884bc-1715">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="884bc-1715">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1716">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1716">Core</span></span>

* <span data-ttu-id="884bc-1717">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="884bc-1717">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1718">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1718">ACS</span></span>

* <span data-ttu-id="884bc-1719">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="884bc-1719">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="884bc-1720">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1720">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="884bc-1721">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="884bc-1721">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="884bc-1722">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="884bc-1722">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="884bc-1723">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="884bc-1723">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="884bc-1724">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1724">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="884bc-1725">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="884bc-1725">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="884bc-1726">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1726">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1727">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-1727">Appservice</span></span>

* <span data-ttu-id="884bc-1728">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1728">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="884bc-1729">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1729">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="884bc-1730">CDN</span><span class="sxs-lookup"><span data-stu-id="884bc-1730">CDN</span></span>

* <span data-ttu-id="884bc-1731">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1731">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1732">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1732">Container</span></span>

* <span data-ttu-id="884bc-1733">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="884bc-1733">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="884bc-1734">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-1734">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="884bc-1735">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-1735">CosmosDB</span></span>

* <span data-ttu-id="884bc-1736">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="884bc-1736">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="884bc-1737">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="884bc-1737">Extension</span></span>

* <span data-ttu-id="884bc-1738">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1738">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="884bc-1739">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1739">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="884bc-1740">Отзыв</span><span class="sxs-lookup"><span data-stu-id="884bc-1740">Feedback</span></span>

* <span data-ttu-id="884bc-1741">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="884bc-1741">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-1742">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-1742">Interactive</span></span>

* <span data-ttu-id="884bc-1743">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="884bc-1743">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="884bc-1744">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="884bc-1744">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-1745">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-1745">IoT</span></span>

* <span data-ttu-id="884bc-1746">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="884bc-1746">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="884bc-1747">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="884bc-1747">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="884bc-1748">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1748">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="884bc-1749">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="884bc-1749">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-1750">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-1750">Monitor</span></span>

* <span data-ttu-id="884bc-1751">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1751">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1752">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1752">Network</span></span>

* <span data-ttu-id="884bc-1753">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="884bc-1753">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="884bc-1754">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-1754">Profile</span></span>

* <span data-ttu-id="884bc-1755">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="884bc-1755">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-1756">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-1756">Resource</span></span>

* <span data-ttu-id="884bc-1757">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1757">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="884bc-1758">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-1758">Role</span></span>

* <span data-ttu-id="884bc-1759">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="884bc-1759">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-1760">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-1760">SQL</span></span>

* <span data-ttu-id="884bc-1761">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1761">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="884bc-1762">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1762">Added `sql db rename`</span></span>
* <span data-ttu-id="884bc-1763">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="884bc-1763">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1764">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1764">Storage</span></span>

* <span data-ttu-id="884bc-1765">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="884bc-1765">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1766">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1766">VM</span></span>

* <span data-ttu-id="884bc-1767">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="884bc-1767">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="884bc-1768">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="884bc-1768">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="884bc-1769">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="884bc-1769">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="884bc-1770">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1770">January 31, 2018</span></span>

<span data-ttu-id="884bc-1771">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="884bc-1771">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1772">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1772">Core</span></span>

* <span data-ttu-id="884bc-1773">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="884bc-1773">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="884bc-1774">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="884bc-1774">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="884bc-1775">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="884bc-1775">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="884bc-1776">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="884bc-1776">Use `--verbose` to see</span></span>
* <span data-ttu-id="884bc-1777">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-1777">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1778">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1778">ACS</span></span>

* <span data-ttu-id="884bc-1779">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1779">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="884bc-1780">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1780">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1781">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-1781">Appservice</span></span>

* <span data-ttu-id="884bc-1782">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="884bc-1782">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="884bc-1783">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="884bc-1783">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="884bc-1784">CDN</span><span class="sxs-lookup"><span data-stu-id="884bc-1784">CDN</span></span>

* <span data-ttu-id="884bc-1785">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1785">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="884bc-1786">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-1786">CosmosDB</span></span>

* <span data-ttu-id="884bc-1787">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="884bc-1787">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-1788">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-1788">Interactive</span></span>

* <span data-ttu-id="884bc-1789">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="884bc-1789">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1790">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1790">Network</span></span>

* <span data-ttu-id="884bc-1791">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1791">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="884bc-1792">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-1792">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="884bc-1793">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1793">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="884bc-1794">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1794">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="884bc-1795">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1795">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="884bc-1796">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="884bc-1796">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="884bc-1797">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="884bc-1797">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="884bc-1798">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="884bc-1798">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="884bc-1799">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1799">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="884bc-1800">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1800">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="884bc-1801">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-1801">Profile</span></span>

* <span data-ttu-id="884bc-1802">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="884bc-1802">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-1803">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-1803">Resource</span></span>

* <span data-ttu-id="884bc-1804">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="884bc-1804">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1805">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1805">Storage</span></span>

* <span data-ttu-id="884bc-1806">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="884bc-1806">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="884bc-1807">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="884bc-1807">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="884bc-1808">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1808">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="884bc-1809">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1809">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="884bc-1810">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="884bc-1810">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1811">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1811">VM</span></span>

* <span data-ttu-id="884bc-1812">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="884bc-1812">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="884bc-1813">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1813">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="884bc-1814">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="884bc-1814">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="884bc-1815">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1815">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="884bc-1816">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1816">January 17, 2018</span></span>

<span data-ttu-id="884bc-1817">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="884bc-1817">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1818">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1818">ACR</span></span>

* <span data-ttu-id="884bc-1819">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="884bc-1819">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="884bc-1820">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="884bc-1820">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1821">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1821">ACS</span></span>

* <span data-ttu-id="884bc-1822">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1822">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="884bc-1823">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-1823">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1824">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-1824">Appservice</span></span>

* <span data-ttu-id="884bc-1825">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="884bc-1825">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="884bc-1826">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1826">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="884bc-1827">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1827">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="884bc-1828">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="884bc-1828">Backup</span></span>

* <span data-ttu-id="884bc-1829">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="884bc-1829">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="884bc-1830">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="884bc-1830">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="884bc-1831">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="884bc-1831">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="884bc-1832">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="884bc-1832">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="884bc-1833">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="884bc-1833">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-1834">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-1834">Batch</span></span>

* <span data-ttu-id="884bc-1835">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="884bc-1835">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="884bc-1836">Облако</span><span class="sxs-lookup"><span data-stu-id="884bc-1836">Cloud</span></span>

* <span data-ttu-id="884bc-1837">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1837">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="884bc-1838">Потребление</span><span class="sxs-lookup"><span data-stu-id="884bc-1838">Consumption</span></span>

* <span data-ttu-id="884bc-1839">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1839">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="884bc-1840">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-1840">Event Grid</span></span>

* <span data-ttu-id="884bc-1841">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1841">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="884bc-1842">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1842">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="884bc-1843">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1843">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="884bc-1844">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1844">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="884bc-1845">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1845">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="884bc-1846">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1846">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="884bc-1847">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1847">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="884bc-1848">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1848">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-1849">Interactive</span><span class="sxs-lookup"><span data-stu-id="884bc-1849">Interactive</span></span>

* <span data-ttu-id="884bc-1850">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="884bc-1850">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="884bc-1851">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="884bc-1851">Fixed errors on startup</span></span>
* <span data-ttu-id="884bc-1852">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="884bc-1852">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-1853">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-1853">IoT</span></span>

* <span data-ttu-id="884bc-1854">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="884bc-1854">Added support for device provisioning service</span></span>
* <span data-ttu-id="884bc-1855">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="884bc-1855">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="884bc-1856">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="884bc-1856">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-1857">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-1857">Monitor</span></span>

* <span data-ttu-id="884bc-1858">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="884bc-1858">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="884bc-1859">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1859">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="884bc-1860">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="884bc-1860">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1861">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1861">Network</span></span>

* <span data-ttu-id="884bc-1862">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="884bc-1862">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="884bc-1863">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="884bc-1863">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="884bc-1864">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-1864">Profile</span></span>

* <span data-ttu-id="884bc-1865">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="884bc-1865">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="884bc-1866">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-1866">Role</span></span>

* <span data-ttu-id="884bc-1867">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1867">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="884bc-1868">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="884bc-1868">Service Fabric</span></span>

* <span data-ttu-id="884bc-1869">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="884bc-1869">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="884bc-1870">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-1870">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1871">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1871">VM</span></span>

* <span data-ttu-id="884bc-1872">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1872">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="884bc-1873">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="884bc-1873">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="884bc-1874">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1874">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="884bc-1875">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="884bc-1875">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="884bc-1876">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="884bc-1876">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="884bc-1877">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1877">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="884bc-1878">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1878">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="884bc-1879">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1879">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="884bc-1880">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1880">December 19, 2017</span></span>

<span data-ttu-id="884bc-1881">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="884bc-1881">Version 2.0.23</span></span>

* <span data-ttu-id="884bc-1882">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="884bc-1882">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1883">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1883">Container</span></span>

* <span data-ttu-id="884bc-1884">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-1884">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1885">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1885">Network</span></span>

* <span data-ttu-id="884bc-1886">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="884bc-1886">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="884bc-1887">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="884bc-1887">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1888">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1888">Storage</span></span>

* <span data-ttu-id="884bc-1889">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="884bc-1889">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1890">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1890">VM</span></span>

* <span data-ttu-id="884bc-1891">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="884bc-1891">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="884bc-1892">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1892">December 5, 2017</span></span>

<span data-ttu-id="884bc-1893">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="884bc-1893">Version 2.0.22</span></span>

* <span data-ttu-id="884bc-1894">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1894">Removed `az component` commands.</span></span> <span data-ttu-id="884bc-1895">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1895">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1896">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1896">Core</span></span>
* <span data-ttu-id="884bc-1897">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="884bc-1897">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="884bc-1898">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="884bc-1898">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-1899">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1899">ACS</span></span>

* <span data-ttu-id="884bc-1900">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1900">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="884bc-1901">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1901">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="884bc-1902">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="884bc-1902">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="884bc-1903">Помощник</span><span class="sxs-lookup"><span data-stu-id="884bc-1903">Advisor</span></span>

* <span data-ttu-id="884bc-1904">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="884bc-1904">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1905">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-1905">Appservice</span></span>

* <span data-ttu-id="884bc-1906">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1906">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="884bc-1907">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="884bc-1907">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="884bc-1908">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1908">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="884bc-1909">Потребление</span><span class="sxs-lookup"><span data-stu-id="884bc-1909">Consumption</span></span>

* <span data-ttu-id="884bc-1910">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="884bc-1910">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1911">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1911">Container</span></span>

* <span data-ttu-id="884bc-1912">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="884bc-1912">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-1913">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-1913">Monitor</span></span>

* <span data-ttu-id="884bc-1914">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="884bc-1914">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-1915">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-1915">Resource</span></span>

* <span data-ttu-id="884bc-1916">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="884bc-1916">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="884bc-1917">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-1917">Role</span></span>

* <span data-ttu-id="884bc-1918">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1918">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="884bc-1919">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="884bc-1919">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="884bc-1920">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1920">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-1921">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-1921">SQL</span></span>

* <span data-ttu-id="884bc-1922">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1922">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="884bc-1923">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1923">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1924">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1924">VM</span></span>

* <span data-ttu-id="884bc-1925">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1925">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="884bc-1926">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1926">November 14, 2017</span></span>

<span data-ttu-id="884bc-1927">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="884bc-1927">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1928">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1928">ACR</span></span>

* <span data-ttu-id="884bc-1929">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="884bc-1929">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="884bc-1930">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-1930">ACS</span></span>

* <span data-ttu-id="884bc-1931">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="884bc-1931">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="884bc-1932">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="884bc-1932">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="884bc-1933">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1933">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="884bc-1934">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="884bc-1934">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="884bc-1935">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="884bc-1935">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-1936">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-1936">Appservice</span></span>

* <span data-ttu-id="884bc-1937">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="884bc-1937">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="884bc-1938">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1938">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="884bc-1939">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1939">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="884bc-1940">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1940">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="884bc-1941">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="884bc-1941">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="884bc-1942">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="884bc-1942">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-1943">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-1943">Batch</span></span>

* <span data-ttu-id="884bc-1944">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1944">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="884bc-1945">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="884bc-1945">Batchai</span></span>

* <span data-ttu-id="884bc-1946">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1946">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="884bc-1947">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1947">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="884bc-1948">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1948">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="884bc-1949">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1949">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="884bc-1950">Облако</span><span class="sxs-lookup"><span data-stu-id="884bc-1950">Cloud</span></span>

* <span data-ttu-id="884bc-1951">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="884bc-1951">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="884bc-1952">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-1952">Container</span></span>

* <span data-ttu-id="884bc-1953">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1953">Added support to open multiple ports</span></span>
* <span data-ttu-id="884bc-1954">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-1954">Added container group restart policy</span></span>
* <span data-ttu-id="884bc-1955">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="884bc-1955">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="884bc-1956">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="884bc-1956">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="884bc-1957">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="884bc-1957">Data Lake Analytics</span></span>

* <span data-ttu-id="884bc-1958">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="884bc-1958">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="884bc-1959">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="884bc-1959">Data Lake Store</span></span>

* <span data-ttu-id="884bc-1960">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="884bc-1960">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="884bc-1961">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="884bc-1961">Extension</span></span>

* <span data-ttu-id="884bc-1962">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="884bc-1962">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="884bc-1963">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="884bc-1963">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-1964">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-1964">IoT</span></span>

* <span data-ttu-id="884bc-1965">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1965">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-1966">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-1966">Monitor</span></span>

* <span data-ttu-id="884bc-1967">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1967">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="884bc-1968">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-1968">Network</span></span>

* <span data-ttu-id="884bc-1969">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="884bc-1969">Added support for CAA DNS records</span></span>
* <span data-ttu-id="884bc-1970">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1970">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="884bc-1971">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="884bc-1971">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="884bc-1972">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1972">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="884bc-1973">Резервирование</span><span class="sxs-lookup"><span data-stu-id="884bc-1973">Reservations</span></span>

* <span data-ttu-id="884bc-1974">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="884bc-1974">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-1975">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-1975">Resource</span></span>

* <span data-ttu-id="884bc-1976">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1976">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-1977">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-1977">SQL</span></span>

* <span data-ttu-id="884bc-1978">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1978">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-1979">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-1979">Storage</span></span>

* <span data-ttu-id="884bc-1980">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-1980">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="884bc-1981">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="884bc-1981">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="884bc-1982">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1982">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="884bc-1983">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1983">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="884bc-1984">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1984">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="884bc-1985">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1985">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="884bc-1986">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1986">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-1987">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-1987">VM</span></span>

* <span data-ttu-id="884bc-1988">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1988">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="884bc-1989">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="884bc-1989">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="884bc-1990">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1990">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="884bc-1991">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="884bc-1991">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="884bc-1992">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="884bc-1992">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="884bc-1993">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-1993">October 24, 2017</span></span>

<span data-ttu-id="884bc-1994">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="884bc-1994">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="884bc-1995">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-1995">Core</span></span>

* <span data-ttu-id="884bc-1996">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="884bc-1996">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-1997">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-1997">ACR</span></span>

* <span data-ttu-id="884bc-1998">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="884bc-1998">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="884bc-1999">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="884bc-1999">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="884bc-2000">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="884bc-2000">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-2001">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-2001">ACS</span></span>

* <span data-ttu-id="884bc-2002">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="884bc-2002">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="884bc-2003">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="884bc-2003">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-2004">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-2004">Appservice</span></span>

* <span data-ttu-id="884bc-2005">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="884bc-2005">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="884bc-2006">Компонент</span><span class="sxs-lookup"><span data-stu-id="884bc-2006">Component</span></span>

* <span data-ttu-id="884bc-2007">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="884bc-2007">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-2008">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-2008">Monitor</span></span>

* <span data-ttu-id="884bc-2009">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2009">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-2010">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-2010">Resource</span></span>

* <span data-ttu-id="884bc-2011">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="884bc-2011">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="884bc-2012">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="884bc-2012">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-2013">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-2013">VM</span></span>

* <span data-ttu-id="884bc-2014">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="884bc-2014">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="884bc-2015">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-2015">October 9, 2017</span></span>

<span data-ttu-id="884bc-2016">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="884bc-2016">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="884bc-2017">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-2017">Core</span></span>

* <span data-ttu-id="884bc-2018">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="884bc-2018">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-2019">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-2019">Appservice</span></span>

* <span data-ttu-id="884bc-2020">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2020">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-2021">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-2021">Batch</span></span>

* <span data-ttu-id="884bc-2022">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="884bc-2022">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="884bc-2023">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="884bc-2023">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="884bc-2024">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-2024">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="884bc-2025">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="884bc-2025">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="884bc-2026">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="884bc-2026">Batchai</span></span>

* <span data-ttu-id="884bc-2027">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="884bc-2027">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="884bc-2028">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="884bc-2028">Keyvault</span></span>

* <span data-ttu-id="884bc-2029">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="884bc-2029">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="884bc-2030">(#4448)</span><span class="sxs-lookup"><span data-stu-id="884bc-2030">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="884bc-2031">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-2031">Network</span></span>

* <span data-ttu-id="884bc-2032">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="884bc-2032">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="884bc-2033">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="884bc-2033">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-2034">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-2034">Resource</span></span>

* <span data-ttu-id="884bc-2035">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2035">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="884bc-2036">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="884bc-2036">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="884bc-2037">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="884bc-2037">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="884bc-2038">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="884bc-2038">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-2039">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-2039">Sql</span></span>

* <span data-ttu-id="884bc-2040">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="884bc-2040">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="884bc-2041">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="884bc-2041">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="884bc-2042">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="884bc-2042">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-2043">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-2043">Storage</span></span>

* <span data-ttu-id="884bc-2044">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="884bc-2044">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-2045">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="884bc-2045">Vm</span></span>

* <span data-ttu-id="884bc-2046">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="884bc-2046">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="884bc-2047">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2047">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="884bc-2048">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2048">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="884bc-2049">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2049">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="884bc-2050">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="884bc-2050">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="884bc-2051">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-2051">September 22, 2017</span></span>

<span data-ttu-id="884bc-2052">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="884bc-2052">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-2053">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-2053">Resource</span></span>

* <span data-ttu-id="884bc-2054">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="884bc-2054">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="884bc-2055">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="884bc-2055">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="884bc-2056">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="884bc-2056">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="884bc-2057">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2057">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="884bc-2058">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-2058">Network</span></span>

* <span data-ttu-id="884bc-2059">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="884bc-2059">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="884bc-2060">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="884bc-2060">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="884bc-2061">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="884bc-2061">Added `asg` application security group commands</span></span>
* <span data-ttu-id="884bc-2062">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="884bc-2062">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="884bc-2063">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="884bc-2063">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="884bc-2064">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="884bc-2064">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="884bc-2065">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2065">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-2066">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-2066">Storage</span></span>

* <span data-ttu-id="884bc-2067">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="884bc-2067">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="884bc-2068">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="884bc-2068">Eventgrid</span></span>

* <span data-ttu-id="884bc-2069">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="884bc-2069">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-2070">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-2070">SQL</span></span>

* <span data-ttu-id="884bc-2071">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="884bc-2071">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="884bc-2072">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="884bc-2072">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="884bc-2073">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="884bc-2073">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="884bc-2074">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="884bc-2074">Keyvault</span></span>

* <span data-ttu-id="884bc-2075">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="884bc-2075">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-2076">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-2076">VM</span></span>

* <span data-ttu-id="884bc-2077">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="884bc-2077">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="884bc-2078">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="884bc-2078">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="884bc-2079">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="884bc-2079">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="884bc-2080">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="884bc-2080">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="884bc-2081">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="884bc-2081">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="884bc-2082">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="884bc-2082">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-2083">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-2083">ACS</span></span>

* <span data-ttu-id="884bc-2084">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="884bc-2084">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-2085">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-2085">Appservice</span></span>

* <span data-ttu-id="884bc-2086">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="884bc-2086">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="884bc-2087">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="884bc-2087">Backup</span></span>

* <span data-ttu-id="884bc-2088">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="884bc-2088">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="884bc-2089">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-2089">September 11, 2017</span></span>

<span data-ttu-id="884bc-2090">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="884bc-2090">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="884bc-2091">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-2091">Core</span></span>

* <span data-ttu-id="884bc-2092">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="884bc-2092">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="884bc-2093">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="884bc-2093">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-2094">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-2094">Acs</span></span>

* <span data-ttu-id="884bc-2095">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2095">Added `acs list-locations` command</span></span>
* <span data-ttu-id="884bc-2096">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-2096">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-2097">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-2097">Appservice</span></span>

* <span data-ttu-id="884bc-2098">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="884bc-2098">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="884bc-2099">CDN</span><span class="sxs-lookup"><span data-stu-id="884bc-2099">CDN</span></span>

* <span data-ttu-id="884bc-2100">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2100">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="884bc-2101">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="884bc-2101">Extension</span></span>

* <span data-ttu-id="884bc-2102">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="884bc-2102">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="884bc-2103">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="884bc-2103">Keyvault</span></span>

* <span data-ttu-id="884bc-2104">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2104">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="884bc-2105">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-2105">Network</span></span>

* <span data-ttu-id="884bc-2106">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2106">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="884bc-2107">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2107">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="884bc-2108">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2108">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="884bc-2109">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2109">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="884bc-2110">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2110">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-2111">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-2111">Resource</span></span>

* <span data-ttu-id="884bc-2112">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2112">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="884bc-2113">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2113">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="884bc-2114">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="884bc-2114">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="884bc-2115">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="884bc-2115">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-2116">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-2116">SQL</span></span>

* <span data-ttu-id="884bc-2117">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2117">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-2118">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-2118">VM</span></span>

* <span data-ttu-id="884bc-2119">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="884bc-2119">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="884bc-2120">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="884bc-2120">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="884bc-2121">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2121">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="884bc-2122">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="884bc-2122">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="884bc-2123">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="884bc-2123">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="884bc-2124">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-2124">August 31, 2017</span></span>

<span data-ttu-id="884bc-2125">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="884bc-2125">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="884bc-2126">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="884bc-2126">Keyvault</span></span>

* <span data-ttu-id="884bc-2127">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2127">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="884bc-2128">Sf</span><span class="sxs-lookup"><span data-stu-id="884bc-2128">Sf</span></span>

* <span data-ttu-id="884bc-2129">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="884bc-2129">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-2130">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-2130">Storage</span></span>

* <span data-ttu-id="884bc-2131">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="884bc-2131">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="884bc-2132">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="884bc-2132">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="884bc-2133">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-2133">August 28, 2017</span></span>

<span data-ttu-id="884bc-2134">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="884bc-2134">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="884bc-2135">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="884bc-2135">CLI</span></span>

* <span data-ttu-id="884bc-2136">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="884bc-2136">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-2137">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-2137">ACS</span></span>

* <span data-ttu-id="884bc-2138">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="884bc-2138">Corrected preview regions</span></span>
* <span data-ttu-id="884bc-2139">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2139">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="884bc-2140">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="884bc-2140">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-2141">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-2141">Appservice</span></span>

* <span data-ttu-id="884bc-2142">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2142">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="884bc-2143">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2143">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="884bc-2144">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2144">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="884bc-2145">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="884bc-2145">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="884bc-2146">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="884bc-2146">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-2147">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-2147">IoT</span></span>

* <span data-ttu-id="884bc-2148">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="884bc-2148">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="884bc-2149">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-2149">Network</span></span>

* <span data-ttu-id="884bc-2150">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2150">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="884bc-2151">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2151">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="884bc-2152">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2152">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="884bc-2153">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2153">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="884bc-2154">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2154">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="884bc-2155">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-2155">Profile</span></span>

* <span data-ttu-id="884bc-2156">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="884bc-2156">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="884bc-2157">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="884bc-2157">Service Fabric</span></span>

* <span data-ttu-id="884bc-2158">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="884bc-2158">Preview release</span></span>
* <span data-ttu-id="884bc-2159">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="884bc-2159">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="884bc-2160">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="884bc-2160">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="884bc-2161">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2161">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-2162">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-2162">Storage</span></span>

* <span data-ttu-id="884bc-2163">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="884bc-2163">Enabled setting blob tier</span></span>
* <span data-ttu-id="884bc-2164">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-2164">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="884bc-2165">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2165">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="884bc-2166">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="884bc-2166">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="884bc-2167">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2167">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="884bc-2168">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2168">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-2169">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-2169">VM</span></span>

* <span data-ttu-id="884bc-2170">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2170">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="884bc-2171">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2171">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="884bc-2172">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="884bc-2172">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="884bc-2173">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="884bc-2173">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="884bc-2174">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="884bc-2174">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="884bc-2175">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2175">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="884bc-2176">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-2176">August 15, 2017</span></span>

<span data-ttu-id="884bc-2177">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="884bc-2177">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-2178">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-2178">ACS</span></span>

* <span data-ttu-id="884bc-2179">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="884bc-2179">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-2180">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-2180">Appservice</span></span>

* <span data-ttu-id="884bc-2181">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="884bc-2181">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="884bc-2182">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-2182">Event Grid</span></span>

* <span data-ttu-id="884bc-2183">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="884bc-2183">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="884bc-2184">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-2184">August 11, 2017</span></span>

<span data-ttu-id="884bc-2185">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="884bc-2185">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-2186">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-2186">ACS</span></span>

* <span data-ttu-id="884bc-2187">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="884bc-2187">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-2188">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-2188">Batch</span></span>

* <span data-ttu-id="884bc-2189">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="884bc-2189">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="884bc-2190">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="884bc-2190">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="884bc-2191">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="884bc-2191">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="884bc-2192">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="884bc-2192">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="884bc-2193">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="884bc-2193">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="884bc-2194">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="884bc-2194">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="884bc-2195">Компонент</span><span class="sxs-lookup"><span data-stu-id="884bc-2195">Component</span></span>

* <span data-ttu-id="884bc-2196">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="884bc-2196">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="884bc-2197">Контейнер</span><span class="sxs-lookup"><span data-stu-id="884bc-2197">Container</span></span>

* <span data-ttu-id="884bc-2198">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="884bc-2198">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="884bc-2199">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="884bc-2199">Data Lake Store</span></span>

* <span data-ttu-id="884bc-2200">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="884bc-2200">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="884bc-2201">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-2201">Event Grid</span></span>

* <span data-ttu-id="884bc-2202">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="884bc-2202">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="884bc-2203">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-2203">Network</span></span>

* <span data-ttu-id="884bc-2204">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="884bc-2204">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="884bc-2205">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2205">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="884bc-2206">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2206">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="884bc-2207">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2207">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="884bc-2208">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-2208">Profile</span></span>

* <span data-ttu-id="884bc-2209">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="884bc-2209">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-2210">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-2210">Storage</span></span>

* <span data-ttu-id="884bc-2211">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="884bc-2211">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-2212">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-2212">VM</span></span>

* <span data-ttu-id="884bc-2213">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="884bc-2213">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="884bc-2214">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2214">Exposed `list-skus` command</span></span>
* <span data-ttu-id="884bc-2215">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="884bc-2215">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="884bc-2216">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="884bc-2216">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="884bc-2217">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="884bc-2217">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="884bc-2218">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-2218">July 28, 2017</span></span>

<span data-ttu-id="884bc-2219">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="884bc-2219">Version 2.0.12</span></span>

* <span data-ttu-id="884bc-2220">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="884bc-2220">Added container commands</span></span>
* <span data-ttu-id="884bc-2221">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="884bc-2221">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="884bc-2222">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-2222">Core</span></span>

* <span data-ttu-id="884bc-2223">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="884bc-2223">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="884bc-2224">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="884bc-2224">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="884bc-2225">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="884bc-2225">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="884bc-2226">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="884bc-2226">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="884bc-2227">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="884bc-2227">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="884bc-2228">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="884bc-2228">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="884bc-2229">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="884bc-2229">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="884bc-2230">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="884bc-2230">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="884bc-2231">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="884bc-2231">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="884bc-2232">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="884bc-2232">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="884bc-2233">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="884bc-2233">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="884bc-2234">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="884bc-2234">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="884bc-2235">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="884bc-2235">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="884bc-2236">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="884bc-2236">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="884bc-2237">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="884bc-2237">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="884bc-2238">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="884bc-2238">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="884bc-2239">ACR</span><span class="sxs-lookup"><span data-stu-id="884bc-2239">ACR</span></span>

* <span data-ttu-id="884bc-2240">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="884bc-2240">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="884bc-2241">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="884bc-2241">Support SKU update for managed registries</span></span>
* <span data-ttu-id="884bc-2242">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="884bc-2242">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="884bc-2243">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="884bc-2243">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="884bc-2244">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="884bc-2244">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="884bc-2245">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="884bc-2245">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-2246">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-2246">ACS</span></span>

* <span data-ttu-id="884bc-2247">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="884bc-2247">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-2248">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="884bc-2248">Appservice</span></span>

* <span data-ttu-id="884bc-2249">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="884bc-2249">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="884bc-2250">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="884bc-2250">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="884bc-2251">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2251">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="884bc-2252">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="884bc-2252">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="884bc-2253">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="884bc-2253">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="884bc-2254">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="884bc-2254">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="884bc-2255">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="884bc-2255">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="884bc-2256">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="884bc-2256">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="884bc-2257">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="884bc-2257">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="884bc-2258">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2258">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="884bc-2259">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="884bc-2259">Batch</span></span>

* <span data-ttu-id="884bc-2260">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="884bc-2260">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="884bc-2261">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2261">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="884bc-2262">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2262">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="884bc-2263">CDN</span><span class="sxs-lookup"><span data-stu-id="884bc-2263">CDN</span></span>

* <span data-ttu-id="884bc-2264">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="884bc-2264">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="884bc-2265">Облако</span><span class="sxs-lookup"><span data-stu-id="884bc-2265">Cloud</span></span>

* <span data-ttu-id="884bc-2266">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="884bc-2266">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="884bc-2267">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="884bc-2267">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="884bc-2268">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="884bc-2268">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="884bc-2269">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="884bc-2269">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="884bc-2270">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2270">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="884bc-2271">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-2271">CosmosDB</span></span>

* <span data-ttu-id="884bc-2272">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="884bc-2272">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="884bc-2273">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="884bc-2273">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="884bc-2274">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="884bc-2274">Data Lake Analytics</span></span>

* <span data-ttu-id="884bc-2275">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2275">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="884bc-2276">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2276">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="884bc-2277">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2277">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="884bc-2278">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="884bc-2278">Data Lake Store</span></span>

* <span data-ttu-id="884bc-2279">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2279">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="884bc-2280">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="884bc-2280">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="884bc-2281">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2281">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="884bc-2282">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="884bc-2282">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="884bc-2283">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="884bc-2283">Interactive</span></span>

* <span data-ttu-id="884bc-2284">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="884bc-2284">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="884bc-2285">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="884bc-2285">Increased test coverage</span></span>
* <span data-ttu-id="884bc-2286">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="884bc-2286">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="884bc-2287">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="884bc-2287">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="884bc-2288">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="884bc-2288">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="884bc-2289">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="884bc-2289">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="884bc-2290">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="884bc-2290">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="884bc-2291">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2291">Added `--progress` flag</span></span>
* <span data-ttu-id="884bc-2292">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2292">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="884bc-2293">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="884bc-2293">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="884bc-2294">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="884bc-2294">IoT</span></span>

* <span data-ttu-id="884bc-2295">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="884bc-2295">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="884bc-2296">(3934).</span><span class="sxs-lookup"><span data-stu-id="884bc-2296">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="884bc-2297">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="884bc-2297">Key vault</span></span>

* <span data-ttu-id="884bc-2298">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="884bc-2298">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="884bc-2299">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2299">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="884bc-2300">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="884bc-2300">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="884bc-2301">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="884bc-2301">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="884bc-2302">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2302">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="884bc-2303">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="884bc-2303">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="884bc-2304">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="884bc-2304">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="884bc-2305">(3307).</span><span class="sxs-lookup"><span data-stu-id="884bc-2305">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="884bc-2306">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="884bc-2306">Lab</span></span>

* <span data-ttu-id="884bc-2307">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2307">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="884bc-2308">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2308">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-2309">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-2309">Monitor</span></span>

* <span data-ttu-id="884bc-2310">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="884bc-2310">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="884bc-2311">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2311">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="884bc-2312">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2312">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="884bc-2313">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2313">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="884bc-2314">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2314">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="884bc-2315">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="884bc-2315">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="884bc-2316">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="884bc-2316">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="884bc-2317">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="884bc-2317">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="884bc-2318">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="884bc-2318">`location` no longer required</span></span>
  * <span data-ttu-id="884bc-2319">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="884bc-2319">Add name and ID support for target</span></span>
  * <span data-ttu-id="884bc-2320">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="884bc-2320">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="884bc-2321">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="884bc-2321">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="884bc-2322">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="884bc-2322">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="884bc-2323">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="884bc-2323">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="884bc-2324">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2324">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="884bc-2325">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2325">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="884bc-2326">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-2326">Network</span></span>

* <span data-ttu-id="884bc-2327">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2327">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="884bc-2328">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2328">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="884bc-2329">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="884bc-2329">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="884bc-2330">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2330">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="884bc-2331">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2331">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="884bc-2332">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2332">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="884bc-2333">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2333">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="884bc-2334">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2334">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="884bc-2335">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2335">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="884bc-2336">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2336">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="884bc-2337">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2337">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="884bc-2338">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2338">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="884bc-2339">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2339">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="884bc-2340">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2340">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="884bc-2341">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2341">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="884bc-2342">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2342">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="884bc-2343">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="884bc-2343">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="884bc-2344">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2344">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="884bc-2345">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2345">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="884bc-2346">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2346">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="884bc-2347">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2347">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="884bc-2348">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2348">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="884bc-2349">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2349">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="884bc-2350">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="884bc-2350">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="884bc-2351">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="884bc-2351">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="884bc-2352">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="884bc-2352">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="884bc-2353">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="884bc-2353">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="884bc-2354">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-2354">Profile</span></span>

* <span data-ttu-id="884bc-2355">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="884bc-2355">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="884bc-2356">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="884bc-2356">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="884bc-2357">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="884bc-2357">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="884bc-2358">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="884bc-2358">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="884bc-2359">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="884bc-2359">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="884bc-2360">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="884bc-2360">RDBMS</span></span>

* <span data-ttu-id="884bc-2361">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="884bc-2361">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="884bc-2362">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="884bc-2362">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="884bc-2363">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="884bc-2363">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="884bc-2364">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="884bc-2364">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-2365">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-2365">Resource</span></span>

* <span data-ttu-id="884bc-2366">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2366">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="884bc-2367">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2367">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="884bc-2368">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2368">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="884bc-2369">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2369">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="884bc-2370">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="884bc-2370">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="884bc-2371">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2371">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="884bc-2372">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="884bc-2372">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="884bc-2373">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2373">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="884bc-2374">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-2374">Role</span></span>

* <span data-ttu-id="884bc-2375">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="884bc-2375">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="884bc-2376">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="884bc-2376">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="884bc-2377">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="884bc-2377">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="884bc-2378">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="884bc-2378">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="884bc-2379">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2379">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="884bc-2380">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="884bc-2380">Service Fabric</span></span>
* <span data-ttu-id="884bc-2381">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="884bc-2381">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="884bc-2382">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="884bc-2382">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="884bc-2383">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="884bc-2383">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-2384">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-2384">SQL</span></span>

* <span data-ttu-id="884bc-2385">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2385">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="884bc-2386">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2386">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="884bc-2387">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2387">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-2388">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-2388">Storage</span></span>

* <span data-ttu-id="884bc-2389">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="884bc-2389">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="884bc-2390">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="884bc-2390">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="884bc-2391">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="884bc-2391">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="884bc-2392">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="884bc-2392">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="884bc-2393">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="884bc-2393">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="884bc-2394">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="884bc-2394">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-2395">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-2395">VM</span></span>

* <span data-ttu-id="884bc-2396">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="884bc-2396">Support configuring nsg</span></span>
* <span data-ttu-id="884bc-2397">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="884bc-2397">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="884bc-2398">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="884bc-2398">Support managed service identities</span></span>
* <span data-ttu-id="884bc-2399">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2399">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="884bc-2400">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="884bc-2400">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="884bc-2401">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-2401">May 10, 2017</span></span>

<span data-ttu-id="884bc-2402">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="884bc-2402">Version 2.0.6</span></span>

* <span data-ttu-id="884bc-2403">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="884bc-2403">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="884bc-2404">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="884bc-2404">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="884bc-2405">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="884bc-2405">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="884bc-2406">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="884bc-2406">Include Cognitive Services module</span></span>
* <span data-ttu-id="884bc-2407">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="884bc-2407">Include Service Fabric module</span></span>
* <span data-ttu-id="884bc-2408">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="884bc-2408">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="884bc-2409">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="884bc-2409">Add support for CDN commands</span></span>
* <span data-ttu-id="884bc-2410">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="884bc-2410">Remove Container module</span></span>
* <span data-ttu-id="884bc-2411">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2411">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="884bc-2412">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2412">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="884bc-2413">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-2413">Core</span></span>

* <span data-ttu-id="884bc-2414">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="884bc-2414">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="884bc-2415">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2415">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="884bc-2416">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2416">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="884bc-2417">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2417">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="884bc-2418">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2418">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="884bc-2419">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2419">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="884bc-2420">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2420">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="884bc-2421">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2421">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="884bc-2422">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2422">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="884bc-2423">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="884bc-2423">core: Improved performance</span></span>
* <span data-ttu-id="884bc-2424">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="884bc-2424">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="884bc-2425">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="884bc-2425">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-2426">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-2426">ACS</span></span>

* <span data-ttu-id="884bc-2427">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="884bc-2427">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="884bc-2428">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="884bc-2428">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="884bc-2429">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="884bc-2429">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="884bc-2430">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2430">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-2431">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-2431">AppService</span></span>

* <span data-ttu-id="884bc-2432">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="884bc-2432">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="884bc-2433">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="884bc-2433">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="884bc-2434">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="884bc-2434">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="884bc-2435">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="884bc-2435">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="884bc-2436">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="884bc-2436">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="884bc-2437">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2437">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="884bc-2438">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="884bc-2438">support slot swap with preview</span></span>
* <span data-ttu-id="884bc-2439">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2439">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="884bc-2440">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2440">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="884bc-2441">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="884bc-2441">CosmosDB</span></span>

* <span data-ttu-id="884bc-2442">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="884bc-2442">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="884bc-2443">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="884bc-2443">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="884bc-2444">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="884bc-2444">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="884bc-2445">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="884bc-2445">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="884bc-2446">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="884bc-2446">Data Lake Analytics</span></span>

* <span data-ttu-id="884bc-2447">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="884bc-2447">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="884bc-2448">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="884bc-2448">Add support for new catalog item type: package.</span></span> <span data-ttu-id="884bc-2449">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2449">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="884bc-2450">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="884bc-2450">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="884bc-2451">Таблица</span><span class="sxs-lookup"><span data-stu-id="884bc-2451">Table</span></span>
  * <span data-ttu-id="884bc-2452">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="884bc-2452">Table valued function</span></span>
  * <span data-ttu-id="884bc-2453">Просмотр</span><span class="sxs-lookup"><span data-stu-id="884bc-2453">View</span></span>
  * <span data-ttu-id="884bc-2454">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="884bc-2454">Table Statistics.</span></span> <span data-ttu-id="884bc-2455">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="884bc-2455">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="884bc-2456">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="884bc-2456">Data Lake Store</span></span>

* <span data-ttu-id="884bc-2457">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="884bc-2457">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="884bc-2458">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2458">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="884bc-2459">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="884bc-2459">missed help for access show.</span></span> <span data-ttu-id="884bc-2460">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="884bc-2460">adding it.</span></span> <span data-ttu-id="884bc-2461">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="884bc-2461">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="884bc-2462">Поиск</span><span class="sxs-lookup"><span data-stu-id="884bc-2462">Find</span></span>

* <span data-ttu-id="884bc-2463">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="884bc-2463">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="884bc-2464">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="884bc-2464">KeyVault</span></span>

* <span data-ttu-id="884bc-2465">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="884bc-2465">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="884bc-2466">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="884bc-2466">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="884bc-2467">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="884bc-2467">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="884bc-2468">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="884bc-2468">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="884bc-2469">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2469">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="884bc-2470">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="884bc-2470">Lab</span></span>

* <span data-ttu-id="884bc-2471">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="884bc-2471">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="884bc-2472">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="884bc-2472">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="884bc-2473">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="884bc-2473">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="884bc-2474">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="884bc-2474">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="884bc-2475">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="884bc-2475">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="884bc-2476">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="884bc-2476">Monitor</span></span>

* <span data-ttu-id="884bc-2477">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2477">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="884bc-2478">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2478">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="884bc-2479">Network</span><span class="sxs-lookup"><span data-stu-id="884bc-2479">Network</span></span>

* <span data-ttu-id="884bc-2480">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2480">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="884bc-2481">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2481">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="884bc-2482">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="884bc-2482">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="884bc-2483">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="884bc-2483">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="884bc-2484">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="884bc-2484">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="884bc-2485">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="884bc-2485">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="884bc-2486">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="884bc-2486">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="884bc-2487">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="884bc-2487">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="884bc-2488">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2488">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="884bc-2489">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="884bc-2489">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="884bc-2490">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2490">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="884bc-2491">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2491">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="884bc-2492">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="884bc-2492">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="884bc-2493">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="884bc-2493">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="884bc-2494">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="884bc-2494">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="884bc-2495">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="884bc-2495">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="884bc-2496">Профиль</span><span class="sxs-lookup"><span data-stu-id="884bc-2496">Profile</span></span>

* <span data-ttu-id="884bc-2497">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2497">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="884bc-2498">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2498">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="884bc-2499">Redis</span><span class="sxs-lookup"><span data-stu-id="884bc-2499">Redis</span></span>

* <span data-ttu-id="884bc-2500">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="884bc-2500">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="884bc-2501">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="884bc-2501">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="884bc-2502">Ресурс</span><span class="sxs-lookup"><span data-stu-id="884bc-2502">Resource</span></span>

* <span data-ttu-id="884bc-2503">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2503">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="884bc-2504">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2504">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="884bc-2505">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2505">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="884bc-2506">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="884bc-2506">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="884bc-2507">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="884bc-2507">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="884bc-2508">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="884bc-2508">Add docs for az lock update.</span></span> <span data-ttu-id="884bc-2509">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="884bc-2509">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="884bc-2510">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="884bc-2510">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="884bc-2511">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="884bc-2511">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="884bc-2512">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="884bc-2512">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="884bc-2513">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="884bc-2513">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="884bc-2514">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2514">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="884bc-2515">Роль</span><span class="sxs-lookup"><span data-stu-id="884bc-2515">Role</span></span>

* <span data-ttu-id="884bc-2516">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2516">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="884bc-2517">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2517">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="884bc-2518">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2518">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="884bc-2519">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="884bc-2519">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="884bc-2520">SQL</span><span class="sxs-lookup"><span data-stu-id="884bc-2520">SQL</span></span>

* <span data-ttu-id="884bc-2521">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="884bc-2521">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="884bc-2522">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2522">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="884bc-2523">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-2523">Storage</span></span>

* <span data-ttu-id="884bc-2524">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2524">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="884bc-2525">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="884bc-2525">Add support for incremental blob copy</span></span>
* <span data-ttu-id="884bc-2526">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="884bc-2526">Add support for large block blob upload</span></span>
* <span data-ttu-id="884bc-2527">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="884bc-2527">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-2528">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-2528">VM</span></span>

* <span data-ttu-id="884bc-2529">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="884bc-2529">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="884bc-2530">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="884bc-2530">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="884bc-2531">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="884bc-2531">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="884bc-2532">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="884bc-2532">az vm/vmss disk</span></span>
  3. <span data-ttu-id="884bc-2533">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="884bc-2533">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="884bc-2534">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="884bc-2534">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="884bc-2535">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2535">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="884bc-2536">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-2536">April 3, 2017</span></span>

<span data-ttu-id="884bc-2537">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="884bc-2537">Version 2.0.2</span></span>

<span data-ttu-id="884bc-2538">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="884bc-2538">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="884bc-2539">Core</span><span class="sxs-lookup"><span data-stu-id="884bc-2539">Core</span></span>

* <span data-ttu-id="884bc-2540">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-2540">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="884bc-2541">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2541">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="884bc-2542">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2542">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="884bc-2543">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2543">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="884bc-2544">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2544">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="884bc-2545">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="884bc-2545">Add prompting for missing template parameters.</span></span> <span data-ttu-id="884bc-2546">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2546">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="884bc-2547">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="884bc-2547">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="884bc-2548">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="884bc-2548">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="884bc-2549">ACS</span><span class="sxs-lookup"><span data-stu-id="884bc-2549">ACS</span></span>

* <span data-ttu-id="884bc-2550">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2550">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="884bc-2551">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="884bc-2551">Add support for ssh key password prompting.</span></span> <span data-ttu-id="884bc-2552">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2552">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="884bc-2553">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="884bc-2553">Add support for windows clusters.</span></span> <span data-ttu-id="884bc-2554">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2554">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="884bc-2555">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="884bc-2555">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="884bc-2556">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2556">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="884bc-2557">AppService</span><span class="sxs-lookup"><span data-stu-id="884bc-2557">AppService</span></span>

* <span data-ttu-id="884bc-2558">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2558">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="884bc-2559">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2559">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="884bc-2560">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2560">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="884bc-2561">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2561">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="884bc-2562">Data Lake</span><span class="sxs-lookup"><span data-stu-id="884bc-2562">DataLake</span></span>

* <span data-ttu-id="884bc-2563">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="884bc-2563">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="884bc-2564">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="884bc-2564">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="884bc-2565">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="884bc-2565">DocuemntDB</span></span>

* <span data-ttu-id="884bc-2566">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2566">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="884bc-2567">ВМ</span><span class="sxs-lookup"><span data-stu-id="884bc-2567">VM</span></span>

* <span data-ttu-id="884bc-2568">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2568">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="884bc-2569">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2569">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="884bc-2570">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2570">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="884bc-2571">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2571">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="884bc-2572">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2572">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="884bc-2573">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2573">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="884bc-2574">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="884bc-2574">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="884bc-2575">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="884bc-2575">February 27, 2017</span></span>

<span data-ttu-id="884bc-2576">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="884bc-2576">Version 2.0.0</span></span>

<span data-ttu-id="884bc-2577">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="884bc-2577">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="884bc-2578">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="884bc-2578">Container Service (acs)</span></span>
- <span data-ttu-id="884bc-2579">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="884bc-2579">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="884bc-2580">Сеть</span><span class="sxs-lookup"><span data-stu-id="884bc-2580">Networking</span></span>
- <span data-ttu-id="884bc-2581">Хранилище</span><span class="sxs-lookup"><span data-stu-id="884bc-2581">Storage</span></span>

<span data-ttu-id="884bc-2582">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2582">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="884bc-2583">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="884bc-2583">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="884bc-2584">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="884bc-2584">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="884bc-2585">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="884bc-2585">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="884bc-2586">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="884bc-2586">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="884bc-2587">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="884bc-2587">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="884bc-2588">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="884bc-2588">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="884bc-2589">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="884bc-2589">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="884bc-2590">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="884bc-2590">Provide feedback from the command line with the `az feedback` command</span></span>

