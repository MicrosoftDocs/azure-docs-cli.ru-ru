---
title: "Заметки о выпуске Azure CLI 2.0"
description: "Узнайте о последних обновлениях в Azure CLI 2.0"
keywords: "Azure CLI 2.0, заметки о выпуске"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 01/17/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 86babea3030ea932de1858a391014e5d0bba7f73
ms.sourcegitcommit: cae66f994cb7b7f829f75ac528093fdb6851f64e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="3c015-104">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="3c015-104">Azure CLI 2.0 release notes</span></span>

## <a name="january-17-2018"></a><span data-ttu-id="3c015-105">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-105">January 17, 2018</span></span>

<span data-ttu-id="3c015-106">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="3c015-106">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="3c015-107">ACR</span><span class="sxs-lookup"><span data-stu-id="3c015-107">ACR</span></span>

* <span data-ttu-id="3c015-108">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="3c015-108">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="3c015-109">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="3c015-109">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="3c015-110">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-110">ACS</span></span>

* <span data-ttu-id="3c015-111">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="3c015-111">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="3c015-112">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="3c015-112">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-113">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3c015-113">Appservice</span></span>

* <span data-ttu-id="3c015-114">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="3c015-114">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="3c015-115">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="3c015-115">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="3c015-116">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="3c015-116">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="3c015-117">Архивация</span><span class="sxs-lookup"><span data-stu-id="3c015-117">Backup</span></span>

* <span data-ttu-id="3c015-118">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="3c015-118">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="3c015-119">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="3c015-119">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="3c015-120">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="3c015-120">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="3c015-121">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="3c015-121">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="3c015-122">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="3c015-122">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="3c015-123">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="3c015-123">Batch</span></span>

* <span data-ttu-id="3c015-124">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="3c015-124">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="3c015-125">Облако</span><span class="sxs-lookup"><span data-stu-id="3c015-125">Cloud</span></span>

* <span data-ttu-id="3c015-126">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="3c015-126">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="3c015-127">Потребление</span><span class="sxs-lookup"><span data-stu-id="3c015-127">Consumption</span></span>

* <span data-ttu-id="3c015-128">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="3c015-128">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="3c015-129">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="3c015-129">Event Grid</span></span>

* <span data-ttu-id="3c015-130">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="3c015-130">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="3c015-131">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="3c015-131">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="3c015-132">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="3c015-132">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="3c015-133">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="3c015-133">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="3c015-134">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-134">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="3c015-135">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-135">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="3c015-136">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="3c015-136">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="3c015-137">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="3c015-137">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="3c015-138">Interactive</span><span class="sxs-lookup"><span data-stu-id="3c015-138">Interactive</span></span>

* <span data-ttu-id="3c015-139">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="3c015-139">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="3c015-140">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="3c015-140">Fixed errors on startup</span></span>
* <span data-ttu-id="3c015-141">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="3c015-141">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="3c015-142">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="3c015-142">IoT</span></span>

* <span data-ttu-id="3c015-143">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="3c015-143">Added support for device provisioning service</span></span>
* <span data-ttu-id="3c015-144">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="3c015-144">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="3c015-145">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="3c015-145">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="3c015-146">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="3c015-146">Monitor</span></span>

* <span data-ttu-id="3c015-147">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="3c015-147">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="3c015-148">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-148">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="3c015-149">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="3c015-149">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span> 

### <a name="network"></a><span data-ttu-id="3c015-150">Сеть</span><span class="sxs-lookup"><span data-stu-id="3c015-150">Network</span></span>

* <span data-ttu-id="3c015-151">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="3c015-151">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="3c015-152">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="3c015-152">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="3c015-153">Профиль</span><span class="sxs-lookup"><span data-stu-id="3c015-153">Profile</span></span>

* <span data-ttu-id="3c015-154">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3c015-154">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="3c015-155">Роль</span><span class="sxs-lookup"><span data-stu-id="3c015-155">Role</span></span>

* <span data-ttu-id="3c015-156">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="3c015-156">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3c015-157">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3c015-157">Service Fabric</span></span>

* <span data-ttu-id="3c015-158">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="3c015-158">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="3c015-159">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="3c015-159">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-160">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-160">VM</span></span>

* <span data-ttu-id="3c015-161">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="3c015-161">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="3c015-162">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Значение по умолчанию `vmss` для одной зоны заменено на данные подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="3c015-162">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="3c015-163">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="3c015-163">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="3c015-164">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="3c015-164">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="3c015-165">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="3c015-165">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="3c015-166">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="3c015-166">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="3c015-167">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-167">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="3c015-168">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="3c015-168">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="3c015-169">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-169">December 19, 2017</span></span>

<span data-ttu-id="3c015-170">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="3c015-170">Version 2.0.23</span></span>

* <span data-ttu-id="3c015-171">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="3c015-171">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="3c015-172">Контейнер</span><span class="sxs-lookup"><span data-stu-id="3c015-172">Container</span></span>

* <span data-ttu-id="3c015-173">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="3c015-173">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="3c015-174">Сеть</span><span class="sxs-lookup"><span data-stu-id="3c015-174">Network</span></span>

* <span data-ttu-id="3c015-175">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c015-175">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="3c015-176">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c015-176">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="3c015-177">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3c015-177">Storage</span></span>

* <span data-ttu-id="3c015-178">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="3c015-178">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-179">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-179">VM</span></span>

* <span data-ttu-id="3c015-180">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="3c015-180">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="3c015-181">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-181">December 5, 2017</span></span>

<span data-ttu-id="3c015-182">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="3c015-182">Version 2.0.22</span></span>

* <span data-ttu-id="3c015-183">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="3c015-183">Removed `az component` commands.</span></span> <span data-ttu-id="3c015-184">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="3c015-184">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="3c015-185">Core</span><span class="sxs-lookup"><span data-stu-id="3c015-185">Core</span></span>
* <span data-ttu-id="3c015-186">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="3c015-186">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="3c015-187">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="3c015-187">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="3c015-188">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-188">ACS</span></span>

* <span data-ttu-id="3c015-189">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="3c015-189">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="3c015-190">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-190">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="3c015-191">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="3c015-191">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="3c015-192">Помощник</span><span class="sxs-lookup"><span data-stu-id="3c015-192">Advisor</span></span>

* <span data-ttu-id="3c015-193">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="3c015-193">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-194">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3c015-194">Appservice</span></span>

* <span data-ttu-id="3c015-195">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="3c015-195">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="3c015-196">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="3c015-196">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="3c015-197">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="3c015-197">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="3c015-198">Потребление</span><span class="sxs-lookup"><span data-stu-id="3c015-198">Consumption</span></span>

* <span data-ttu-id="3c015-199">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="3c015-199">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="3c015-200">Контейнер</span><span class="sxs-lookup"><span data-stu-id="3c015-200">Container</span></span>

* <span data-ttu-id="3c015-201">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="3c015-201">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="3c015-202">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="3c015-202">Monitor</span></span>

* <span data-ttu-id="3c015-203">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="3c015-203">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="3c015-204">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3c015-204">Resource</span></span>

* <span data-ttu-id="3c015-205">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="3c015-205">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="3c015-206">Роль</span><span class="sxs-lookup"><span data-stu-id="3c015-206">Role</span></span>

* <span data-ttu-id="3c015-207">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="3c015-207">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="3c015-208">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="3c015-208">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="3c015-209">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="3c015-209">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="3c015-210">SQL</span><span class="sxs-lookup"><span data-stu-id="3c015-210">SQL</span></span>

* <span data-ttu-id="3c015-211">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="3c015-211">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="3c015-212">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-212">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-213">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-213">VM</span></span>

* <span data-ttu-id="3c015-214">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="3c015-214">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="3c015-215">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-215">November 14, 2017</span></span>

<span data-ttu-id="3c015-216">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="3c015-216">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="3c015-217">ACR</span><span class="sxs-lookup"><span data-stu-id="3c015-217">ACR</span></span>

* <span data-ttu-id="3c015-218">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="3c015-218">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="3c015-219">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-219">ACS</span></span>

* <span data-ttu-id="3c015-220">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="3c015-220">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="3c015-221">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="3c015-221">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="3c015-222">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="3c015-222">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="3c015-223">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="3c015-223">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="3c015-224">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="3c015-224">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-225">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3c015-225">Appservice</span></span>

* <span data-ttu-id="3c015-226">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="3c015-226">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="3c015-227">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="3c015-227">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="3c015-228">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="3c015-228">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="3c015-229">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="3c015-229">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="3c015-230">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="3c015-230">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="3c015-231">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="3c015-231">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="3c015-232">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="3c015-232">Batch</span></span>

* <span data-ttu-id="3c015-233">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="3c015-233">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="3c015-234">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="3c015-234">Batchai</span></span>

* <span data-ttu-id="3c015-235">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-235">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="3c015-236">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-236">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="3c015-237">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="3c015-237">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="3c015-238">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-238">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="3c015-239">Облако</span><span class="sxs-lookup"><span data-stu-id="3c015-239">Cloud</span></span>

* <span data-ttu-id="3c015-240">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="3c015-240">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="3c015-241">Контейнер</span><span class="sxs-lookup"><span data-stu-id="3c015-241">Container</span></span>

* <span data-ttu-id="3c015-242">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="3c015-242">Added support to open multiple ports</span></span>
* <span data-ttu-id="3c015-243">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="3c015-243">Added container group restart policy</span></span>
* <span data-ttu-id="3c015-244">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="3c015-244">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="3c015-245">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="3c015-245">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3c015-246">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3c015-246">Data Lake Analytics</span></span>

* <span data-ttu-id="3c015-247">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="3c015-247">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3c015-248">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3c015-248">Data Lake Store</span></span>

* <span data-ttu-id="3c015-249">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="3c015-249">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="3c015-250">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="3c015-250">Extension</span></span>

* <span data-ttu-id="3c015-251">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="3c015-251">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="3c015-252">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="3c015-252">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="3c015-253">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="3c015-253">IoT</span></span>

* <span data-ttu-id="3c015-254">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="3c015-254">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="3c015-255">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="3c015-255">Monitor</span></span>

* <span data-ttu-id="3c015-256">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="3c015-256">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="3c015-257">Сеть</span><span class="sxs-lookup"><span data-stu-id="3c015-257">Network</span></span>

* <span data-ttu-id="3c015-258">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="3c015-258">Added support for CAA DNS records</span></span>
* <span data-ttu-id="3c015-259">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-259">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="3c015-260">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="3c015-260">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="3c015-261">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="3c015-261">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="3c015-262">Резервирование</span><span class="sxs-lookup"><span data-stu-id="3c015-262">Reservations</span></span>

* <span data-ttu-id="3c015-263">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="3c015-263">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="3c015-264">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3c015-264">Resource</span></span>

* <span data-ttu-id="3c015-265">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="3c015-265">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="3c015-266">SQL</span><span class="sxs-lookup"><span data-stu-id="3c015-266">SQL</span></span>

* <span data-ttu-id="3c015-267">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3c015-267">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="3c015-268">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3c015-268">Storage</span></span>

* <span data-ttu-id="3c015-269">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3c015-269">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="3c015-270">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="3c015-270">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="3c015-271">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="3c015-271">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="3c015-272">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="3c015-272">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="3c015-273">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-273">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="3c015-274">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="3c015-274">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="3c015-275">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3c015-275">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-276">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-276">VM</span></span>

* <span data-ttu-id="3c015-277">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="3c015-277">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="3c015-278">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="3c015-278">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="3c015-279">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="3c015-279">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="3c015-280">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="3c015-280">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="3c015-281">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="3c015-281">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="3c015-282">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-282">October 24, 2017</span></span>

<span data-ttu-id="3c015-283">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="3c015-283">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="3c015-284">Core</span><span class="sxs-lookup"><span data-stu-id="3c015-284">Core</span></span>

* <span data-ttu-id="3c015-285">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="3c015-285">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="3c015-286">ACR</span><span class="sxs-lookup"><span data-stu-id="3c015-286">ACR</span></span>

* <span data-ttu-id="3c015-287">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="3c015-287">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="3c015-288">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="3c015-288">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="3c015-289">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="3c015-289">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="3c015-290">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-290">ACS</span></span>

* <span data-ttu-id="3c015-291">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="3c015-291">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="3c015-292">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="3c015-292">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-293">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3c015-293">Appservice</span></span>

* <span data-ttu-id="3c015-294">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="3c015-294">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="3c015-295">Компонент</span><span class="sxs-lookup"><span data-stu-id="3c015-295">Component</span></span>

* <span data-ttu-id="3c015-296">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="3c015-296">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="3c015-297">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="3c015-297">Monitor</span></span>

* <span data-ttu-id="3c015-298">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="3c015-298">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="3c015-299">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3c015-299">Resource</span></span>

* <span data-ttu-id="3c015-300">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="3c015-300">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="3c015-301">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="3c015-301">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-302">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-302">VM</span></span>

* <span data-ttu-id="3c015-303">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="3c015-303">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="3c015-304">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-304">October 9, 2017</span></span>

<span data-ttu-id="3c015-305">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="3c015-305">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="3c015-306">Core</span><span class="sxs-lookup"><span data-stu-id="3c015-306">Core</span></span>

* <span data-ttu-id="3c015-307">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="3c015-307">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-308">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3c015-308">Appservice</span></span>

* <span data-ttu-id="3c015-309">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-309">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="3c015-310">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="3c015-310">Batch</span></span>

* <span data-ttu-id="3c015-311">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="3c015-311">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="3c015-312">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="3c015-312">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="3c015-313">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="3c015-313">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="3c015-314">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="3c015-314">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="3c015-315">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="3c015-315">Batchai</span></span>

* <span data-ttu-id="3c015-316">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="3c015-316">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c015-317">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="3c015-317">Keyvault</span></span>

* <span data-ttu-id="3c015-318">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3c015-318">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="3c015-319">(#4448)</span><span class="sxs-lookup"><span data-stu-id="3c015-319">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="3c015-320">Сеть</span><span class="sxs-lookup"><span data-stu-id="3c015-320">Network</span></span>

* <span data-ttu-id="3c015-321">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="3c015-321">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="3c015-322">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="3c015-322">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="3c015-323">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3c015-323">Resource</span></span>

* <span data-ttu-id="3c015-324">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="3c015-324">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="3c015-325">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="3c015-325">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="3c015-326">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="3c015-326">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="3c015-327">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="3c015-327">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="3c015-328">SQL</span><span class="sxs-lookup"><span data-stu-id="3c015-328">Sql</span></span>

* <span data-ttu-id="3c015-329">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="3c015-329">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="3c015-330">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="3c015-330">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="3c015-331">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="3c015-331">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="3c015-332">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3c015-332">Storage</span></span>

* <span data-ttu-id="3c015-333">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3c015-333">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-334">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="3c015-334">Vm</span></span>

* <span data-ttu-id="3c015-335">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="3c015-335">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="3c015-336">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-336">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="3c015-337">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="3c015-337">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="3c015-338">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-338">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="3c015-339">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="3c015-339">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="3c015-340">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-340">September 22, 2017</span></span>

<span data-ttu-id="3c015-341">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="3c015-341">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="3c015-342">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3c015-342">Resource</span></span>

* <span data-ttu-id="3c015-343">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="3c015-343">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="3c015-344">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="3c015-344">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="3c015-345">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="3c015-345">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="3c015-346">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="3c015-346">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="3c015-347">Сеть</span><span class="sxs-lookup"><span data-stu-id="3c015-347">Network</span></span>

* <span data-ttu-id="3c015-348">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="3c015-348">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="3c015-349">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="3c015-349">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="3c015-350">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="3c015-350">Added `asg` application security group commands</span></span>
* <span data-ttu-id="3c015-351">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="3c015-351">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="3c015-352">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c015-352">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="3c015-353">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c015-353">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="3c015-354">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="3c015-354">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="3c015-355">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3c015-355">Storage</span></span>

* <span data-ttu-id="3c015-356">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="3c015-356">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="3c015-357">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="3c015-357">Eventgrid</span></span>

* <span data-ttu-id="3c015-358">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="3c015-358">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="3c015-359">SQL</span><span class="sxs-lookup"><span data-stu-id="3c015-359">SQL</span></span>

* <span data-ttu-id="3c015-360">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="3c015-360">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="3c015-361">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="3c015-361">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="3c015-362">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="3c015-362">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c015-363">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="3c015-363">Keyvault</span></span>

* <span data-ttu-id="3c015-364">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="3c015-364">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-365">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-365">VM</span></span>

* <span data-ttu-id="3c015-366">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="3c015-366">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="3c015-367">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="3c015-367">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="3c015-368">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="3c015-368">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="3c015-369">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="3c015-369">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="3c015-370">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="3c015-370">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="3c015-371">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="3c015-371">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="3c015-372">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-372">ACS</span></span>

* <span data-ttu-id="3c015-373">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="3c015-373">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-374">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3c015-374">Appservice</span></span>

* <span data-ttu-id="3c015-375">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="3c015-375">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="3c015-376">Архивация</span><span class="sxs-lookup"><span data-stu-id="3c015-376">Backup</span></span>

* <span data-ttu-id="3c015-377">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="3c015-377">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="3c015-378">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-378">September 11, 2017</span></span>

<span data-ttu-id="3c015-379">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="3c015-379">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="3c015-380">Core</span><span class="sxs-lookup"><span data-stu-id="3c015-380">Core</span></span>

* <span data-ttu-id="3c015-381">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="3c015-381">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="3c015-382">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="3c015-382">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="3c015-383">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-383">Acs</span></span>

* <span data-ttu-id="3c015-384">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="3c015-384">Added `acs list-locations` command</span></span>
* <span data-ttu-id="3c015-385">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3c015-385">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-386">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3c015-386">Appservice</span></span>

* <span data-ttu-id="3c015-387">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="3c015-387">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="3c015-388">CDN</span><span class="sxs-lookup"><span data-stu-id="3c015-388">CDN</span></span>

* <span data-ttu-id="3c015-389">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-389">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="3c015-390">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="3c015-390">Extension</span></span>

* <span data-ttu-id="3c015-391">Первый выпуск.</span><span class="sxs-lookup"><span data-stu-id="3c015-391">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c015-392">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="3c015-392">Keyvault</span></span>

* <span data-ttu-id="3c015-393">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="3c015-393">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="3c015-394">Сеть</span><span class="sxs-lookup"><span data-stu-id="3c015-394">Network</span></span>

* <span data-ttu-id="3c015-395">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="3c015-395">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="3c015-396">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-396">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="3c015-397">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-397">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="3c015-398">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-398">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="3c015-399">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-399">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="3c015-400">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3c015-400">Resource</span></span>

* <span data-ttu-id="3c015-401">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-401">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="3c015-402">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-402">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="3c015-403">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="3c015-403">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="3c015-404">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="3c015-404">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="3c015-405">SQL</span><span class="sxs-lookup"><span data-stu-id="3c015-405">SQL</span></span>

* <span data-ttu-id="3c015-406">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="3c015-406">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-407">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-407">VM</span></span>

* <span data-ttu-id="3c015-408">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="3c015-408">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="3c015-409">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="3c015-409">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="3c015-410">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-410">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="3c015-411">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="3c015-411">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="3c015-412">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="3c015-412">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="3c015-413">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-413">August 31, 2017</span></span>

<span data-ttu-id="3c015-414">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="3c015-414">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c015-415">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="3c015-415">Keyvault</span></span>

* <span data-ttu-id="3c015-416">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="3c015-416">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="3c015-417">Sf</span><span class="sxs-lookup"><span data-stu-id="3c015-417">Sf</span></span>

* <span data-ttu-id="3c015-418">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="3c015-418">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="3c015-419">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3c015-419">Storage</span></span>

* <span data-ttu-id="3c015-420">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="3c015-420">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="3c015-421">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="3c015-421">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="3c015-422">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-422">August 28, 2017</span></span>

<span data-ttu-id="3c015-423">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="3c015-423">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="3c015-424">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="3c015-424">CLI</span></span>

* <span data-ttu-id="3c015-425">К параметру `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="3c015-425">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="3c015-426">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-426">ACS</span></span>

* <span data-ttu-id="3c015-427">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="3c015-427">Corrected preview regions.</span></span>
* <span data-ttu-id="3c015-428">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="3c015-428">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="3c015-429">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="3c015-429">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-430">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3c015-430">Appservice</span></span>

* <span data-ttu-id="3c015-431">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="3c015-431">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="3c015-432">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="3c015-432">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="3c015-433">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="3c015-433">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="3c015-434">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="3c015-434">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="3c015-435">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="3c015-435">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="3c015-436">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="3c015-436">IoT</span></span>

* <span data-ttu-id="3c015-437">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="3c015-437">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="3c015-438">Сеть</span><span class="sxs-lookup"><span data-stu-id="3c015-438">Network</span></span>

* <span data-ttu-id="3c015-439">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="3c015-439">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="3c015-440">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3c015-440">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="3c015-441">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3c015-441">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="3c015-442">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-442">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="3c015-443">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-443">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="3c015-444">Профиль</span><span class="sxs-lookup"><span data-stu-id="3c015-444">Profile</span></span>

* <span data-ttu-id="3c015-445">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="3c015-445">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3c015-446">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3c015-446">Service Fabric</span></span>

* <span data-ttu-id="3c015-447">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="3c015-447">Preview release</span></span>
* <span data-ttu-id="3c015-448">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="3c015-448">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="3c015-449">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="3c015-449">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="3c015-450">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="3c015-450">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="3c015-451">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3c015-451">Storage</span></span>

* <span data-ttu-id="3c015-452">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="3c015-452">Enabled setting blob tier</span></span>
* <span data-ttu-id="3c015-453">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="3c015-453">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="3c015-454">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="3c015-454">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="3c015-455">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="3c015-455">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="3c015-456">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-456">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="3c015-457">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="3c015-457">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-458">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-458">VM</span></span>

* <span data-ttu-id="3c015-459">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="3c015-459">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="3c015-460">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-460">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="3c015-461">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="3c015-461">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="3c015-462">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="3c015-462">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="3c015-463">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="3c015-463">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="3c015-464">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-464">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="3c015-465">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-465">August 15, 2017</span></span>

<span data-ttu-id="3c015-466">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="3c015-466">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="3c015-467">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-467">ACS</span></span>

* <span data-ttu-id="3c015-468">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="3c015-468">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-469">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3c015-469">Appservice</span></span>

* <span data-ttu-id="3c015-470">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="3c015-470">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="3c015-471">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="3c015-471">Event Grid</span></span>

* <span data-ttu-id="3c015-472">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="3c015-472">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="3c015-473">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-473">August 11, 2017</span></span>

<span data-ttu-id="3c015-474">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="3c015-474">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="3c015-475">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-475">ACS</span></span>

* <span data-ttu-id="3c015-476">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="3c015-476">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="3c015-477">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="3c015-477">Batch</span></span>

* <span data-ttu-id="3c015-478">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="3c015-478">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="3c015-479">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="3c015-479">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="3c015-480">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3c015-480">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="3c015-481">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="3c015-481">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="3c015-482">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="3c015-482">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="3c015-483">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="3c015-483">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="3c015-484">Компонент</span><span class="sxs-lookup"><span data-stu-id="3c015-484">Component</span></span>

* <span data-ttu-id="3c015-485">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="3c015-485">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="3c015-486">Контейнер</span><span class="sxs-lookup"><span data-stu-id="3c015-486">Container</span></span>

* <span data-ttu-id="3c015-487">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="3c015-487">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="3c015-488">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3c015-488">Data Lake Store</span></span>

* <span data-ttu-id="3c015-489">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="3c015-489">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="3c015-490">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="3c015-490">Event Grid</span></span>

* <span data-ttu-id="3c015-491">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="3c015-491">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="3c015-492">Сеть</span><span class="sxs-lookup"><span data-stu-id="3c015-492">Network</span></span>

* <span data-ttu-id="3c015-493">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="3c015-493">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="3c015-494">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="3c015-494">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="3c015-495">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="3c015-495">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="3c015-496">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="3c015-496">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="3c015-497">Профиль</span><span class="sxs-lookup"><span data-stu-id="3c015-497">Profile</span></span>

* <span data-ttu-id="3c015-498">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="3c015-498">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="3c015-499">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3c015-499">Storage</span></span>

* <span data-ttu-id="3c015-500">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="3c015-500">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-501">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-501">VM</span></span>

* <span data-ttu-id="3c015-502">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="3c015-502">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="3c015-503">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="3c015-503">Exposed `list-skus` command</span></span>
* <span data-ttu-id="3c015-504">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="3c015-504">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="3c015-505">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="3c015-505">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="3c015-506">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="3c015-506">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="3c015-507">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-507">July 28, 2017</span></span>

<span data-ttu-id="3c015-508">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="3c015-508">Version 2.0.12</span></span>

* <span data-ttu-id="3c015-509">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="3c015-509">Added container commands</span></span>
* <span data-ttu-id="3c015-510">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3c015-510">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="3c015-511">Core</span><span class="sxs-lookup"><span data-stu-id="3c015-511">Core</span></span>

* <span data-ttu-id="3c015-512">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="3c015-512">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="3c015-513">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="3c015-513">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="3c015-514">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="3c015-514">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="3c015-515">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="3c015-515">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="3c015-516">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="3c015-516">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="3c015-517">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="3c015-517">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="3c015-518">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="3c015-518">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="3c015-519">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="3c015-519">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="3c015-520">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="3c015-520">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="3c015-521">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="3c015-521">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="3c015-522">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="3c015-522">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="3c015-523">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="3c015-523">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="3c015-524">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="3c015-524">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="3c015-525">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="3c015-525">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="3c015-526">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3c015-526">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="3c015-527">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="3c015-527">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="3c015-528">ACR</span><span class="sxs-lookup"><span data-stu-id="3c015-528">ACR</span></span>

* <span data-ttu-id="3c015-529">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="3c015-529">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="3c015-530">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="3c015-530">Support SKU update for managed registries</span></span>
* <span data-ttu-id="3c015-531">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="3c015-531">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="3c015-532">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="3c015-532">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="3c015-533">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="3c015-533">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="3c015-534">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="3c015-534">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="3c015-535">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-535">ACS</span></span>

* <span data-ttu-id="3c015-536">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="3c015-536">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-537">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3c015-537">Appservice</span></span>

* <span data-ttu-id="3c015-538">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="3c015-538">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="3c015-539">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="3c015-539">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="3c015-540">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="3c015-540">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="3c015-541">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="3c015-541">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="3c015-542">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="3c015-542">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="3c015-543">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="3c015-543">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="3c015-544">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="3c015-544">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="3c015-545">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="3c015-545">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="3c015-546">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="3c015-546">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="3c015-547">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="3c015-547">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="3c015-548">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="3c015-548">Batch</span></span>

* <span data-ttu-id="3c015-549">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="3c015-549">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="3c015-550">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="3c015-550">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="3c015-551">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="3c015-551">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="3c015-552">CDN</span><span class="sxs-lookup"><span data-stu-id="3c015-552">CDN</span></span>

* <span data-ttu-id="3c015-553">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="3c015-553">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="3c015-554">Облако</span><span class="sxs-lookup"><span data-stu-id="3c015-554">Cloud</span></span>

* <span data-ttu-id="3c015-555">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="3c015-555">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="3c015-556">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="3c015-556">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="3c015-557">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="3c015-557">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="3c015-558">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="3c015-558">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="3c015-559">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="3c015-559">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c015-560">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c015-560">CosmosDB</span></span>

* <span data-ttu-id="3c015-561">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="3c015-561">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="3c015-562">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="3c015-562">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3c015-563">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3c015-563">Data Lake Analytics</span></span>

* <span data-ttu-id="3c015-564">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="3c015-564">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="3c015-565">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="3c015-565">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="3c015-566">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="3c015-566">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3c015-567">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3c015-567">Data Lake Store</span></span>

* <span data-ttu-id="3c015-568">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-568">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="3c015-569">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="3c015-569">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="3c015-570">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="3c015-570">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="3c015-571">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="3c015-571">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="3c015-572">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="3c015-572">Interactive</span></span>

* <span data-ttu-id="3c015-573">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="3c015-573">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="3c015-574">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="3c015-574">Increased test coverage</span></span>
* <span data-ttu-id="3c015-575">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="3c015-575">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="3c015-576">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="3c015-576">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="3c015-577">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="3c015-577">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="3c015-578">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="3c015-578">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="3c015-579">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="3c015-579">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="3c015-580">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="3c015-580">Added `--progress` flag</span></span>
* <span data-ttu-id="3c015-581">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="3c015-581">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="3c015-582">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="3c015-582">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="3c015-583">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="3c015-583">IoT</span></span>

* <span data-ttu-id="3c015-584">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="3c015-584">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="3c015-585">(3934).</span><span class="sxs-lookup"><span data-stu-id="3c015-585">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="3c015-586">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="3c015-586">Key vault</span></span>

* <span data-ttu-id="3c015-587">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="3c015-587">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="3c015-588">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="3c015-588">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="3c015-589">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="3c015-589">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="3c015-590">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="3c015-590">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="3c015-591">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="3c015-591">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="3c015-592">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="3c015-592">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="3c015-593">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="3c015-593">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="3c015-594">(3307).</span><span class="sxs-lookup"><span data-stu-id="3c015-594">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="3c015-595">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="3c015-595">Lab</span></span>

* <span data-ttu-id="3c015-596">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="3c015-596">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="3c015-597">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="3c015-597">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="3c015-598">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="3c015-598">Monitor</span></span>

* <span data-ttu-id="3c015-599">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="3c015-599">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="3c015-600">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="3c015-600">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="3c015-601">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="3c015-601">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="3c015-602">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="3c015-602">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="3c015-603">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="3c015-603">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="3c015-604">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="3c015-604">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="3c015-605">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="3c015-605">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="3c015-606">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="3c015-606">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="3c015-607">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="3c015-607">`location` no longer required</span></span>
  * <span data-ttu-id="3c015-608">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="3c015-608">Add name and ID support for target</span></span>
  * <span data-ttu-id="3c015-609">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="3c015-609">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="3c015-610">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="3c015-610">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="3c015-611">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="3c015-611">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="3c015-612">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="3c015-612">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="3c015-613">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="3c015-613">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="3c015-614">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-614">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="3c015-615">Сеть</span><span class="sxs-lookup"><span data-stu-id="3c015-615">Network</span></span>

* <span data-ttu-id="3c015-616">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="3c015-616">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="3c015-617">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-617">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="3c015-618">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="3c015-618">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="3c015-619">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="3c015-619">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="3c015-620">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-620">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="3c015-621">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="3c015-621">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="3c015-622">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="3c015-622">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="3c015-623">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="3c015-623">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="3c015-624">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="3c015-624">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="3c015-625">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="3c015-625">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="3c015-626">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-626">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="3c015-627">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="3c015-627">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="3c015-628">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="3c015-628">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="3c015-629">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-629">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="3c015-630">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-630">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="3c015-631">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-631">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="3c015-632">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="3c015-632">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="3c015-633">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="3c015-633">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="3c015-634">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-634">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="3c015-635">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-635">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="3c015-636">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-636">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="3c015-637">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="3c015-637">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="3c015-638">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="3c015-638">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="3c015-639">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="3c015-639">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="3c015-640">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="3c015-640">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="3c015-641">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="3c015-641">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="3c015-642">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="3c015-642">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="3c015-643">Профиль</span><span class="sxs-lookup"><span data-stu-id="3c015-643">Profile</span></span>

* <span data-ttu-id="3c015-644">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3c015-644">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="3c015-645">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="3c015-645">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="3c015-646">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="3c015-646">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="3c015-647">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="3c015-647">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="3c015-648">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="3c015-648">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="3c015-649">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="3c015-649">RDBMS</span></span>

* <span data-ttu-id="3c015-650">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="3c015-650">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="3c015-651">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="3c015-651">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="3c015-652">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="3c015-652">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="3c015-653">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="3c015-653">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="3c015-654">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3c015-654">Resource</span></span>

* <span data-ttu-id="3c015-655">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-655">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="3c015-656">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="3c015-656">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="3c015-657">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="3c015-657">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="3c015-658">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="3c015-658">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="3c015-659">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="3c015-659">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="3c015-660">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="3c015-660">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="3c015-661">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="3c015-661">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="3c015-662">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="3c015-662">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="3c015-663">Роль</span><span class="sxs-lookup"><span data-stu-id="3c015-663">Role</span></span>

* <span data-ttu-id="3c015-664">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="3c015-664">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="3c015-665">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="3c015-665">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="3c015-666">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="3c015-666">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="3c015-667">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="3c015-667">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="3c015-668">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="3c015-668">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3c015-669">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3c015-669">Service Fabric</span></span>
* <span data-ttu-id="3c015-670">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="3c015-670">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="3c015-671">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="3c015-671">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="3c015-672">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="3c015-672">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="3c015-673">SQL</span><span class="sxs-lookup"><span data-stu-id="3c015-673">SQL</span></span>

* <span data-ttu-id="3c015-674">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-674">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="3c015-675">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="3c015-675">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="3c015-676">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="3c015-676">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="3c015-677">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3c015-677">Storage</span></span>

* <span data-ttu-id="3c015-678">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="3c015-678">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="3c015-679">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="3c015-679">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="3c015-680">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="3c015-680">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="3c015-681">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="3c015-681">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="3c015-682">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="3c015-682">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="3c015-683">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="3c015-683">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-684">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-684">VM</span></span>

* <span data-ttu-id="3c015-685">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="3c015-685">Support configuring nsg</span></span>
* <span data-ttu-id="3c015-686">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="3c015-686">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="3c015-687">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="3c015-687">Support managed service identities</span></span>
* <span data-ttu-id="3c015-688">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="3c015-688">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="3c015-689">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="3c015-689">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="3c015-690">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-690">May 10, 2017</span></span>

<span data-ttu-id="3c015-691">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="3c015-691">Version 2.0.6</span></span>

* <span data-ttu-id="3c015-692">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="3c015-692">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="3c015-693">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="3c015-693">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="3c015-694">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="3c015-694">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="3c015-695">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="3c015-695">Include Cognitive Services module.</span></span>
* <span data-ttu-id="3c015-696">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="3c015-696">Include Service Fabric module.</span></span>
* <span data-ttu-id="3c015-697">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="3c015-697">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="3c015-698">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="3c015-698">Add support for CDN commands.</span></span>
* <span data-ttu-id="3c015-699">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="3c015-699">Remove Container module.</span></span>
* <span data-ttu-id="3c015-700">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="3c015-700">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="3c015-701">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="3c015-701">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="3c015-702">Core</span><span class="sxs-lookup"><span data-stu-id="3c015-702">Core</span></span>

* <span data-ttu-id="3c015-703">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="3c015-703">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="3c015-704">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="3c015-704">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="3c015-705">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="3c015-705">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="3c015-706">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="3c015-706">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="3c015-707">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="3c015-707">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="3c015-708">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="3c015-708">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="3c015-709">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="3c015-709">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="3c015-710">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="3c015-710">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="3c015-711">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="3c015-711">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="3c015-712">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="3c015-712">core: Improved performance</span></span>
* <span data-ttu-id="3c015-713">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="3c015-713">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="3c015-714">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="3c015-714">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="3c015-715">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-715">ACS</span></span>

* <span data-ttu-id="3c015-716">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="3c015-716">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="3c015-717">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="3c015-717">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="3c015-718">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="3c015-718">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="3c015-719">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="3c015-719">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-720">AppService</span><span class="sxs-lookup"><span data-stu-id="3c015-720">AppService</span></span>

* <span data-ttu-id="3c015-721">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="3c015-721">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="3c015-722">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="3c015-722">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="3c015-723">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="3c015-723">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="3c015-724">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="3c015-724">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="3c015-725">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="3c015-725">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="3c015-726">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="3c015-726">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="3c015-727">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="3c015-727">support slot swap with preview</span></span>
* <span data-ttu-id="3c015-728">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="3c015-728">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="3c015-729">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="3c015-729">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3c015-730">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3c015-730">CosmosDB</span></span>

* <span data-ttu-id="3c015-731">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="3c015-731">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="3c015-732">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="3c015-732">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="3c015-733">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="3c015-733">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="3c015-734">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="3c015-734">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3c015-735">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3c015-735">Data Lake Analytics</span></span>

* <span data-ttu-id="3c015-736">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="3c015-736">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="3c015-737">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="3c015-737">Add support for new catalog item type: package.</span></span> <span data-ttu-id="3c015-738">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="3c015-738">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="3c015-739">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="3c015-739">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="3c015-740">Таблица</span><span class="sxs-lookup"><span data-stu-id="3c015-740">Table</span></span>
  * <span data-ttu-id="3c015-741">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="3c015-741">Table valued function</span></span>
  * <span data-ttu-id="3c015-742">Просмотр</span><span class="sxs-lookup"><span data-stu-id="3c015-742">View</span></span>
  * <span data-ttu-id="3c015-743">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="3c015-743">Table Statistics.</span></span> <span data-ttu-id="3c015-744">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="3c015-744">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3c015-745">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3c015-745">Data Lake Store</span></span>

* <span data-ttu-id="3c015-746">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="3c015-746">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="3c015-747">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="3c015-747">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="3c015-748">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="3c015-748">missed help for access show.</span></span> <span data-ttu-id="3c015-749">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="3c015-749">adding it.</span></span> <span data-ttu-id="3c015-750">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="3c015-750">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="3c015-751">Поиск</span><span class="sxs-lookup"><span data-stu-id="3c015-751">Find</span></span>

* <span data-ttu-id="3c015-752">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="3c015-752">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="3c015-753">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="3c015-753">KeyVault</span></span>

* <span data-ttu-id="3c015-754">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="3c015-754">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="3c015-755">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="3c015-755">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="3c015-756">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="3c015-756">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="3c015-757">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="3c015-757">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="3c015-758">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="3c015-758">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="3c015-759">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="3c015-759">Lab</span></span>

* <span data-ttu-id="3c015-760">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="3c015-760">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="3c015-761">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="3c015-761">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="3c015-762">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="3c015-762">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="3c015-763">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="3c015-763">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="3c015-764">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="3c015-764">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="3c015-765">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="3c015-765">Monitor</span></span>

* <span data-ttu-id="3c015-766">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="3c015-766">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="3c015-767">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="3c015-767">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="3c015-768">Сеть</span><span class="sxs-lookup"><span data-stu-id="3c015-768">Network</span></span>

* <span data-ttu-id="3c015-769">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="3c015-769">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="3c015-770">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-770">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="3c015-771">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="3c015-771">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="3c015-772">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="3c015-772">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="3c015-773">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="3c015-773">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="3c015-774">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="3c015-774">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="3c015-775">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="3c015-775">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="3c015-776">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="3c015-776">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="3c015-777">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="3c015-777">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="3c015-778">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="3c015-778">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="3c015-779">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="3c015-779">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="3c015-780">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-780">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="3c015-781">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="3c015-781">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="3c015-782">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="3c015-782">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="3c015-783">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="3c015-783">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="3c015-784">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="3c015-784">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="3c015-785">Профиль</span><span class="sxs-lookup"><span data-stu-id="3c015-785">Profile</span></span>

* <span data-ttu-id="3c015-786">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="3c015-786">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="3c015-787">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="3c015-787">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="3c015-788">Redis</span><span class="sxs-lookup"><span data-stu-id="3c015-788">Redis</span></span>

* <span data-ttu-id="3c015-789">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="3c015-789">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="3c015-790">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="3c015-790">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="3c015-791">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3c015-791">Resource</span></span>

* <span data-ttu-id="3c015-792">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="3c015-792">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="3c015-793">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="3c015-793">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="3c015-794">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="3c015-794">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="3c015-795">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="3c015-795">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="3c015-796">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="3c015-796">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="3c015-797">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="3c015-797">Add docs for az lock update.</span></span> <span data-ttu-id="3c015-798">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="3c015-798">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="3c015-799">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="3c015-799">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="3c015-800">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="3c015-800">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="3c015-801">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="3c015-801">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="3c015-802">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="3c015-802">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="3c015-803">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="3c015-803">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="3c015-804">Роль</span><span class="sxs-lookup"><span data-stu-id="3c015-804">Role</span></span>

* <span data-ttu-id="3c015-805">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="3c015-805">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="3c015-806">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="3c015-806">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="3c015-807">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="3c015-807">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="3c015-808">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="3c015-808">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="3c015-809">SQL</span><span class="sxs-lookup"><span data-stu-id="3c015-809">SQL</span></span>

* <span data-ttu-id="3c015-810">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="3c015-810">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="3c015-811">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="3c015-811">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="3c015-812">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3c015-812">Storage</span></span>

* <span data-ttu-id="3c015-813">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="3c015-813">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="3c015-814">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="3c015-814">Add support for incremental blob copy</span></span>
* <span data-ttu-id="3c015-815">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="3c015-815">Add support for large block blob upload</span></span>
* <span data-ttu-id="3c015-816">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="3c015-816">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-817">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-817">VM</span></span>

* <span data-ttu-id="3c015-818">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="3c015-818">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="3c015-819">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="3c015-819">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="3c015-820">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="3c015-820">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="3c015-821">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="3c015-821">az vm/vmss disk</span></span>
  3. <span data-ttu-id="3c015-822">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="3c015-822">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="3c015-823">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="3c015-823">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="3c015-824">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="3c015-824">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="3c015-825">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-825">April 3, 2017</span></span>

<span data-ttu-id="3c015-826">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="3c015-826">Version 2.0.2</span></span>

<span data-ttu-id="3c015-827">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="3c015-827">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="3c015-828">Core</span><span class="sxs-lookup"><span data-stu-id="3c015-828">Core</span></span>

* <span data-ttu-id="3c015-829">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3c015-829">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="3c015-830">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="3c015-830">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="3c015-831">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="3c015-831">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="3c015-832">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="3c015-832">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="3c015-833">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="3c015-833">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="3c015-834">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="3c015-834">Add prompting for missing template parameters.</span></span> <span data-ttu-id="3c015-835">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="3c015-835">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="3c015-836">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3c015-836">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="3c015-837">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="3c015-837">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="3c015-838">ACS</span><span class="sxs-lookup"><span data-stu-id="3c015-838">ACS</span></span>

* <span data-ttu-id="3c015-839">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="3c015-839">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="3c015-840">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="3c015-840">Add support for ssh key password prompting.</span></span> <span data-ttu-id="3c015-841">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="3c015-841">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="3c015-842">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="3c015-842">Add support for windows clusters.</span></span> <span data-ttu-id="3c015-843">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="3c015-843">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="3c015-844">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="3c015-844">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="3c015-845">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="3c015-845">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="3c015-846">AppService</span><span class="sxs-lookup"><span data-stu-id="3c015-846">AppService</span></span>

* <span data-ttu-id="3c015-847">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="3c015-847">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="3c015-848">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="3c015-848">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="3c015-849">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="3c015-849">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="3c015-850">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="3c015-850">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="3c015-851">DataLake</span><span class="sxs-lookup"><span data-stu-id="3c015-851">DataLake</span></span>

* <span data-ttu-id="3c015-852">Первоначальный выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="3c015-852">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="3c015-853">Первоначальный выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="3c015-853">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="3c015-854">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="3c015-854">DocuemntDB</span></span>

* <span data-ttu-id="3c015-855">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="3c015-855">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="3c015-856">ВМ</span><span class="sxs-lookup"><span data-stu-id="3c015-856">VM</span></span>

* <span data-ttu-id="3c015-857">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="3c015-857">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="3c015-858">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="3c015-858">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="3c015-859">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="3c015-859">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="3c015-860">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="3c015-860">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="3c015-861">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="3c015-861">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="3c015-862">Добавлена команда --secrets для виртуальных машин и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="3c015-862">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="3c015-863">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="3c015-863">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="3c015-864">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3c015-864">February 27, 2017</span></span>

<span data-ttu-id="3c015-865">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="3c015-865">Version 2.0.0</span></span>

<span data-ttu-id="3c015-866">Этот первый общедоступный выпуск Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="3c015-866">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="3c015-867">Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="3c015-867">General availability applies to these command modules:</span></span>
- <span data-ttu-id="3c015-868">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="3c015-868">Container Service (acs)</span></span>
- <span data-ttu-id="3c015-869">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="3c015-869">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="3c015-870">Сеть</span><span class="sxs-lookup"><span data-stu-id="3c015-870">Networking</span></span>
- <span data-ttu-id="3c015-871">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3c015-871">Storage</span></span>

<span data-ttu-id="3c015-872">Эти командные модули могут использоваться в рабочих средах и поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания.</span><span class="sxs-lookup"><span data-stu-id="3c015-872">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="3c015-873">Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="3c015-873">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="3c015-874">Вы можете задавать вопросы на сайте [StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="3c015-874">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="3c015-875">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="3c015-875">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="3c015-876">Чтобы проверить версию интерфейса командной строки, используйте `az --version`.</span><span class="sxs-lookup"><span data-stu-id="3c015-876">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="3c015-877">В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="3c015-877">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="3c015-878">Некоторые командные модули имеют постфикс b*n* или rc*n*.</span><span class="sxs-lookup"><span data-stu-id="3c015-878">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="3c015-879">Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="3c015-879">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="3c015-880">У нас также есть предварительные ежедневные сборки интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="3c015-880">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="3c015-881">Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="3c015-881">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="3c015-882">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="3c015-882">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="3c015-883">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="3c015-883">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="3c015-884">обратившись к специалистам группы разработчиков продукта по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com);</span><span class="sxs-lookup"><span data-stu-id="3c015-884">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="3c015-885">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="3c015-885">Provide feedback from the command line with the `az feedback` command.</span></span>

