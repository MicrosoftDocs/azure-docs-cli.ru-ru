---
title: Заметки о выпуске Azure CLI 2.0
description: Узнайте о последних обновлениях в Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 0e81f5723af47242f908b854045deb7d74c50c17
ms.sourcegitcommit: b5a6296c006e3a44f66892729e47d7a967267d3e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="42a99-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="42a99-103">Azure CLI 2.0 release notes</span></span>

## <a name="march-27-2018"></a><span data-ttu-id="42a99-104">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-104">March 27, 2018</span></span>

<span data-ttu-id="42a99-105">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="42a99-105">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="42a99-106">Core</span><span class="sxs-lookup"><span data-stu-id="42a99-106">Core</span></span>

* <span data-ttu-id="42a99-107">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="42a99-107">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-108">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-108">ACS</span></span>

* <span data-ttu-id="42a99-109">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="42a99-109">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-110">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-110">Appservice</span></span>

* <span data-ttu-id="42a99-111">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-111">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="42a99-112">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-112">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="42a99-113">Архивация</span><span class="sxs-lookup"><span data-stu-id="42a99-113">Backup</span></span>

* <span data-ttu-id="42a99-114">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="42a99-114">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="42a99-115">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="42a99-115">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="42a99-116">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="42a99-116">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="42a99-117">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="42a99-117">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="42a99-118">Контейнер</span><span class="sxs-lookup"><span data-stu-id="42a99-118">Container</span></span>

* <span data-ttu-id="42a99-119">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="42a99-119">Added `container exec` command.</span></span> <span data-ttu-id="42a99-120">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="42a99-120">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="42a99-121">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="42a99-121">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="42a99-122">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="42a99-122">Extension</span></span>

* <span data-ttu-id="42a99-123">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="42a99-123">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="42a99-124">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="42a99-124">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="42a99-125">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="42a99-125">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="42a99-126">Interactive</span><span class="sxs-lookup"><span data-stu-id="42a99-126">Interactive</span></span>

* <span data-ttu-id="42a99-127">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="42a99-127">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="42a99-128">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="42a99-128">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="42a99-129">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="42a99-129">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="42a99-130">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="42a99-130">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="42a99-131">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="42a99-131">Lab</span></span>

* <span data-ttu-id="42a99-132">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="42a99-132">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="42a99-133">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="42a99-133">Monitor</span></span>

* <span data-ttu-id="42a99-134">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="42a99-134">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="42a99-135">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="42a99-135">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="42a99-136">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="42a99-136">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="42a99-137">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-137">Network</span></span>

* <span data-ttu-id="42a99-138">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="42a99-138">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="42a99-139">Профиль</span><span class="sxs-lookup"><span data-stu-id="42a99-139">Profile</span></span>

* <span data-ttu-id="42a99-140">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="42a99-140">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="42a99-141">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="42a99-141">RDBMS</span></span>

* <span data-ttu-id="42a99-142">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="42a99-142">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-143">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-143">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="42a99-145">Роль</span><span class="sxs-lookup"><span data-stu-id="42a99-145">Role</span></span>

* <span data-ttu-id="42a99-146">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-146">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="42a99-147">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="42a99-147">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="42a99-148">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="42a99-148">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="42a99-149">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-149">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="42a99-150">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="42a99-150">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-151">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-151">Storage</span></span>

* <span data-ttu-id="42a99-152">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="42a99-152">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="42a99-153">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="42a99-153">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-154">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-154">VM</span></span>

* <span data-ttu-id="42a99-155">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="42a99-155">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="42a99-156">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-156">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="42a99-157">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="42a99-157">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="42a99-158">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="42a99-158">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="42a99-159">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-159">March 13, 2018</span></span>

<span data-ttu-id="42a99-160">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="42a99-160">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="42a99-161">ACR</span><span class="sxs-lookup"><span data-stu-id="42a99-161">ACR</span></span>

* <span data-ttu-id="42a99-162">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="42a99-162">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="42a99-163">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="42a99-163">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="42a99-164">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="42a99-164">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-165">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-165">ACS</span></span>

* <span data-ttu-id="42a99-166">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="42a99-166">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="42a99-167">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="42a99-167">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="42a99-168">Помощник</span><span class="sxs-lookup"><span data-stu-id="42a99-168">Advisor</span></span>

* <span data-ttu-id="42a99-169">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="42a99-169">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="42a99-170">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-170">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="42a99-171">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="42a99-171">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="42a99-172">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="42a99-172">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="42a99-173">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="42a99-173">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-174">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-174">Appservice</span></span>

* <span data-ttu-id="42a99-175">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="42a99-175">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="42a99-176">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-176">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="42a99-177">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="42a99-177">Eventhubs</span></span>

* <span data-ttu-id="42a99-178">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="42a99-178">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="42a99-179">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="42a99-179">Extension</span></span>

* <span data-ttu-id="42a99-180">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="42a99-180">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="42a99-181">Interactive</span><span class="sxs-lookup"><span data-stu-id="42a99-181">Interactive</span></span>

* <span data-ttu-id="42a99-182">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="42a99-182">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="42a99-183">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="42a99-183">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="42a99-184">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="42a99-184">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="42a99-185">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="42a99-185">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="42a99-186">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="42a99-186">Monitor</span></span>

* <span data-ttu-id="42a99-187">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="42a99-187">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="42a99-188">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="42a99-188">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="42a99-189">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="42a99-189">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="42a99-190">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="42a99-190">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="42a99-191">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-191">Network</span></span>

* <span data-ttu-id="42a99-192">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-192">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="42a99-193">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="42a99-193">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="42a99-194">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="42a99-194">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="42a99-195">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="42a99-195">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="42a99-196">Профиль</span><span class="sxs-lookup"><span data-stu-id="42a99-196">Profile</span></span>

* <span data-ttu-id="42a99-197">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="42a99-197">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="42a99-198">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="42a99-198">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="42a99-199">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="42a99-199">RDBMS</span></span>

* <span data-ttu-id="42a99-200">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="42a99-200">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="42a99-201">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="42a99-201">Service Bus</span></span>

* <span data-ttu-id="42a99-202">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="42a99-202">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-203">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-203">Storage</span></span>

* <span data-ttu-id="42a99-204">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="42a99-204">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="42a99-205">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="42a99-205">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-206">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-206">VM</span></span>

* <span data-ttu-id="42a99-207">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="42a99-207">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="42a99-208">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="42a99-208">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="42a99-209">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-209">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="42a99-210">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="42a99-210">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="42a99-211">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="42a99-211">February 27, 2018</span></span>

<span data-ttu-id="42a99-212">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="42a99-212">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="42a99-213">Core</span><span class="sxs-lookup"><span data-stu-id="42a99-213">Core</span></span>

* <span data-ttu-id="42a99-214">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="42a99-214">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="42a99-215">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="42a99-215">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="42a99-216">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="42a99-216">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-217">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-217">ACS</span></span>

* <span data-ttu-id="42a99-218">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="42a99-218">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="42a99-219">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="42a99-219">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="42a99-220">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="42a99-220">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="42a99-221">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="42a99-221">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-222">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-222">Appservice</span></span>

* <span data-ttu-id="42a99-223">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="42a99-223">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="42a99-224">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="42a99-224">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="42a99-225">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="42a99-225">Cognitive Services</span></span>

* <span data-ttu-id="42a99-226">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="42a99-226">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="42a99-227">Потребление</span><span class="sxs-lookup"><span data-stu-id="42a99-227">Consumption</span></span>

* <span data-ttu-id="42a99-228">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="42a99-228">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="42a99-229">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="42a99-229">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="42a99-230">Контейнер</span><span class="sxs-lookup"><span data-stu-id="42a99-230">Container</span></span>

* <span data-ttu-id="42a99-231">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="42a99-231">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="42a99-232">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-232">Network</span></span>

* <span data-ttu-id="42a99-233">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="42a99-233">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-234">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-234">Resource</span></span>

* <span data-ttu-id="42a99-235">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="42a99-235">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="42a99-236">Роль</span><span class="sxs-lookup"><span data-stu-id="42a99-236">Role</span></span>

* <span data-ttu-id="42a99-237">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="42a99-237">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="42a99-238">SQL</span><span class="sxs-lookup"><span data-stu-id="42a99-238">SQL</span></span>

* <span data-ttu-id="42a99-239">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="42a99-239">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-240">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-240">Storage</span></span>

* <span data-ttu-id="42a99-241">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-241">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-242">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-242">VM</span></span>

* <span data-ttu-id="42a99-243">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="42a99-243">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="42a99-244">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-244">February 13, 2018</span></span>

<span data-ttu-id="42a99-245">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="42a99-245">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="42a99-246">Core</span><span class="sxs-lookup"><span data-stu-id="42a99-246">Core</span></span>

* <span data-ttu-id="42a99-247">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="42a99-247">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-248">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-248">ACS</span></span>

* <span data-ttu-id="42a99-249">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="42a99-249">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="42a99-250">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-250">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="42a99-251">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="42a99-251">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="42a99-252">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="42a99-252">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="42a99-253">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="42a99-253">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="42a99-254">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="42a99-254">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="42a99-255">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="42a99-255">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="42a99-256">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="42a99-256">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-257">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-257">Appservice</span></span>

* <span data-ttu-id="42a99-258">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="42a99-258">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="42a99-259">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="42a99-259">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="42a99-260">CDN</span><span class="sxs-lookup"><span data-stu-id="42a99-260">CDN</span></span>

* <span data-ttu-id="42a99-261">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-261">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="42a99-262">Контейнер</span><span class="sxs-lookup"><span data-stu-id="42a99-262">Container</span></span>

* <span data-ttu-id="42a99-263">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="42a99-263">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="42a99-264">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="42a99-264">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="42a99-265">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="42a99-265">CosmosDB</span></span>

* <span data-ttu-id="42a99-266">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="42a99-266">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="42a99-267">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="42a99-267">Extension</span></span>

* <span data-ttu-id="42a99-268">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-268">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="42a99-269">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-269">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="42a99-270">Отзыв</span><span class="sxs-lookup"><span data-stu-id="42a99-270">Feedback</span></span>

* <span data-ttu-id="42a99-271">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="42a99-271">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="42a99-272">Interactive</span><span class="sxs-lookup"><span data-stu-id="42a99-272">Interactive</span></span>

* <span data-ttu-id="42a99-273">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="42a99-273">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="42a99-274">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="42a99-274">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="42a99-275">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="42a99-275">IoT</span></span>

* <span data-ttu-id="42a99-276">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="42a99-276">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="42a99-277">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="42a99-277">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="42a99-278">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-278">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="42a99-279">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="42a99-279">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="42a99-280">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="42a99-280">Monitor</span></span>

* <span data-ttu-id="42a99-281">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-281">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="42a99-282">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-282">Network</span></span>

* <span data-ttu-id="42a99-283">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="42a99-283">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="42a99-284">Профиль</span><span class="sxs-lookup"><span data-stu-id="42a99-284">Profile</span></span>

* <span data-ttu-id="42a99-285">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="42a99-285">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-286">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-286">Resource</span></span>

* <span data-ttu-id="42a99-287">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="42a99-287">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="42a99-288">Роль</span><span class="sxs-lookup"><span data-stu-id="42a99-288">Role</span></span>

* <span data-ttu-id="42a99-289">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="42a99-289">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="42a99-290">SQL</span><span class="sxs-lookup"><span data-stu-id="42a99-290">SQL</span></span>

* <span data-ttu-id="42a99-291">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="42a99-291">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="42a99-292">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="42a99-292">Added `sql db rename`</span></span>
* <span data-ttu-id="42a99-293">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="42a99-293">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-294">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-294">Storage</span></span>

* <span data-ttu-id="42a99-295">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="42a99-295">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-296">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-296">VM</span></span>

* <span data-ttu-id="42a99-297">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="42a99-297">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="42a99-298">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="42a99-298">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="42a99-299">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="42a99-299">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="42a99-300">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-300">January 31, 2018</span></span>

<span data-ttu-id="42a99-301">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="42a99-301">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="42a99-302">Core</span><span class="sxs-lookup"><span data-stu-id="42a99-302">Core</span></span>

* <span data-ttu-id="42a99-303">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="42a99-303">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="42a99-304">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="42a99-304">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="42a99-305">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="42a99-305">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="42a99-306">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="42a99-306">Use `--verbose` to see</span></span>
* <span data-ttu-id="42a99-307">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="42a99-307">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-308">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-308">ACS</span></span>

* <span data-ttu-id="42a99-309">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="42a99-309">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="42a99-310">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="42a99-310">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-311">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-311">Appservice</span></span>

* <span data-ttu-id="42a99-312">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="42a99-312">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="42a99-313">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="42a99-313">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="42a99-314">CDN</span><span class="sxs-lookup"><span data-stu-id="42a99-314">CDN</span></span>

* <span data-ttu-id="42a99-315">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-315">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="42a99-316">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="42a99-316">CosmosDB</span></span>

* <span data-ttu-id="42a99-317">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="42a99-317">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="42a99-318">Interactive</span><span class="sxs-lookup"><span data-stu-id="42a99-318">Interactive</span></span>

* <span data-ttu-id="42a99-319">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="42a99-319">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="42a99-320">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-320">Network</span></span>

* <span data-ttu-id="42a99-321">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-321">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="42a99-322">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="42a99-322">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="42a99-323">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-323">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="42a99-324">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-324">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="42a99-325">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="42a99-325">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="42a99-326">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="42a99-326">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="42a99-327">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="42a99-327">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="42a99-328">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="42a99-328">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="42a99-329">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="42a99-329">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="42a99-330">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="42a99-330">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="42a99-331">Профиль</span><span class="sxs-lookup"><span data-stu-id="42a99-331">Profile</span></span>

* <span data-ttu-id="42a99-332">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="42a99-332">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-333">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-333">Resource</span></span>

* <span data-ttu-id="42a99-334">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="42a99-334">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-335">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-335">Storage</span></span>

* <span data-ttu-id="42a99-336">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="42a99-336">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="42a99-337">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="42a99-337">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="42a99-338">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="42a99-338">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="42a99-339">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-339">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="42a99-340">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="42a99-340">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-341">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-341">VM</span></span>

* <span data-ttu-id="42a99-342">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="42a99-342">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="42a99-343">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="42a99-343">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="42a99-344">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="42a99-344">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="42a99-345">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-345">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="42a99-346">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-346">January 17, 2018</span></span>

<span data-ttu-id="42a99-347">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="42a99-347">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="42a99-348">ACR</span><span class="sxs-lookup"><span data-stu-id="42a99-348">ACR</span></span>

* <span data-ttu-id="42a99-349">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="42a99-349">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="42a99-350">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="42a99-350">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-351">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-351">ACS</span></span>

* <span data-ttu-id="42a99-352">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="42a99-352">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="42a99-353">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="42a99-353">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-354">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-354">Appservice</span></span>

* <span data-ttu-id="42a99-355">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="42a99-355">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="42a99-356">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="42a99-356">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="42a99-357">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="42a99-357">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="42a99-358">Архивация</span><span class="sxs-lookup"><span data-stu-id="42a99-358">Backup</span></span>

* <span data-ttu-id="42a99-359">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="42a99-359">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="42a99-360">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="42a99-360">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="42a99-361">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="42a99-361">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="42a99-362">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="42a99-362">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="42a99-363">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="42a99-363">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="42a99-364">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="42a99-364">Batch</span></span>

* <span data-ttu-id="42a99-365">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="42a99-365">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="42a99-366">Облако</span><span class="sxs-lookup"><span data-stu-id="42a99-366">Cloud</span></span>

* <span data-ttu-id="42a99-367">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="42a99-367">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="42a99-368">Потребление</span><span class="sxs-lookup"><span data-stu-id="42a99-368">Consumption</span></span>

* <span data-ttu-id="42a99-369">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="42a99-369">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="42a99-370">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="42a99-370">Event Grid</span></span>

* <span data-ttu-id="42a99-371">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="42a99-371">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="42a99-372">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="42a99-372">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="42a99-373">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="42a99-373">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="42a99-374">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="42a99-374">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="42a99-375">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-375">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="42a99-376">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-376">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="42a99-377">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="42a99-377">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="42a99-378">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="42a99-378">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="42a99-379">Interactive</span><span class="sxs-lookup"><span data-stu-id="42a99-379">Interactive</span></span>

* <span data-ttu-id="42a99-380">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="42a99-380">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="42a99-381">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="42a99-381">Fixed errors on startup</span></span>
* <span data-ttu-id="42a99-382">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="42a99-382">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="42a99-383">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="42a99-383">IoT</span></span>

* <span data-ttu-id="42a99-384">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="42a99-384">Added support for device provisioning service</span></span>
* <span data-ttu-id="42a99-385">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="42a99-385">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="42a99-386">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="42a99-386">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="42a99-387">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="42a99-387">Monitor</span></span>

* <span data-ttu-id="42a99-388">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="42a99-388">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="42a99-389">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-389">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="42a99-390">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="42a99-390">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="42a99-391">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-391">Network</span></span>

* <span data-ttu-id="42a99-392">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="42a99-392">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="42a99-393">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="42a99-393">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="42a99-394">Профиль</span><span class="sxs-lookup"><span data-stu-id="42a99-394">Profile</span></span>

* <span data-ttu-id="42a99-395">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="42a99-395">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="42a99-396">Роль</span><span class="sxs-lookup"><span data-stu-id="42a99-396">Role</span></span>

* <span data-ttu-id="42a99-397">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="42a99-397">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="42a99-398">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="42a99-398">Service Fabric</span></span>

* <span data-ttu-id="42a99-399">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="42a99-399">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="42a99-400">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="42a99-400">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-401">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-401">VM</span></span>

* <span data-ttu-id="42a99-402">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="42a99-402">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="42a99-403">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="42a99-403">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="42a99-404">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="42a99-404">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="42a99-405">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="42a99-405">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="42a99-406">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="42a99-406">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="42a99-407">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="42a99-407">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="42a99-408">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-408">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="42a99-409">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="42a99-409">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="42a99-410">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-410">December 19, 2017</span></span>

<span data-ttu-id="42a99-411">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="42a99-411">Version 2.0.23</span></span>

* <span data-ttu-id="42a99-412">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="42a99-412">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="42a99-413">Контейнер</span><span class="sxs-lookup"><span data-stu-id="42a99-413">Container</span></span>

* <span data-ttu-id="42a99-414">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="42a99-414">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="42a99-415">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-415">Network</span></span>

* <span data-ttu-id="42a99-416">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="42a99-416">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="42a99-417">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="42a99-417">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-418">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-418">Storage</span></span>

* <span data-ttu-id="42a99-419">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="42a99-419">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-420">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-420">VM</span></span>

* <span data-ttu-id="42a99-421">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="42a99-421">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="42a99-422">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-422">December 5, 2017</span></span>

<span data-ttu-id="42a99-423">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="42a99-423">Version 2.0.22</span></span>

* <span data-ttu-id="42a99-424">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="42a99-424">Removed `az component` commands.</span></span> <span data-ttu-id="42a99-425">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="42a99-425">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="42a99-426">Core</span><span class="sxs-lookup"><span data-stu-id="42a99-426">Core</span></span>
* <span data-ttu-id="42a99-427">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="42a99-427">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="42a99-428">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="42a99-428">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-429">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-429">ACS</span></span>

* <span data-ttu-id="42a99-430">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="42a99-430">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="42a99-431">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-431">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="42a99-432">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="42a99-432">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="42a99-433">Помощник</span><span class="sxs-lookup"><span data-stu-id="42a99-433">Advisor</span></span>

* <span data-ttu-id="42a99-434">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="42a99-434">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-435">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-435">Appservice</span></span>

* <span data-ttu-id="42a99-436">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="42a99-436">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="42a99-437">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="42a99-437">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="42a99-438">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="42a99-438">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="42a99-439">Потребление</span><span class="sxs-lookup"><span data-stu-id="42a99-439">Consumption</span></span>

* <span data-ttu-id="42a99-440">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="42a99-440">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="42a99-441">Контейнер</span><span class="sxs-lookup"><span data-stu-id="42a99-441">Container</span></span>

* <span data-ttu-id="42a99-442">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="42a99-442">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="42a99-443">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="42a99-443">Monitor</span></span>

* <span data-ttu-id="42a99-444">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="42a99-444">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-445">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-445">Resource</span></span>

* <span data-ttu-id="42a99-446">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="42a99-446">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="42a99-447">Роль</span><span class="sxs-lookup"><span data-stu-id="42a99-447">Role</span></span>

* <span data-ttu-id="42a99-448">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="42a99-448">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="42a99-449">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="42a99-449">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="42a99-450">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="42a99-450">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="42a99-451">SQL</span><span class="sxs-lookup"><span data-stu-id="42a99-451">SQL</span></span>

* <span data-ttu-id="42a99-452">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="42a99-452">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="42a99-453">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-453">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-454">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-454">VM</span></span>

* <span data-ttu-id="42a99-455">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="42a99-455">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="42a99-456">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-456">November 14, 2017</span></span>

<span data-ttu-id="42a99-457">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="42a99-457">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="42a99-458">ACR</span><span class="sxs-lookup"><span data-stu-id="42a99-458">ACR</span></span>

* <span data-ttu-id="42a99-459">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="42a99-459">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="42a99-460">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-460">ACS</span></span>

* <span data-ttu-id="42a99-461">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="42a99-461">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="42a99-462">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="42a99-462">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="42a99-463">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="42a99-463">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="42a99-464">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="42a99-464">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="42a99-465">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="42a99-465">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-466">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-466">Appservice</span></span>

* <span data-ttu-id="42a99-467">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="42a99-467">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="42a99-468">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="42a99-468">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="42a99-469">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="42a99-469">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="42a99-470">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="42a99-470">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="42a99-471">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="42a99-471">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="42a99-472">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="42a99-472">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="42a99-473">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="42a99-473">Batch</span></span>

* <span data-ttu-id="42a99-474">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="42a99-474">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="42a99-475">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="42a99-475">Batchai</span></span>

* <span data-ttu-id="42a99-476">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-476">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="42a99-477">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-477">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="42a99-478">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="42a99-478">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="42a99-479">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-479">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="42a99-480">Облако</span><span class="sxs-lookup"><span data-stu-id="42a99-480">Cloud</span></span>

* <span data-ttu-id="42a99-481">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="42a99-481">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="42a99-482">Контейнер</span><span class="sxs-lookup"><span data-stu-id="42a99-482">Container</span></span>

* <span data-ttu-id="42a99-483">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="42a99-483">Added support to open multiple ports</span></span>
* <span data-ttu-id="42a99-484">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="42a99-484">Added container group restart policy</span></span>
* <span data-ttu-id="42a99-485">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="42a99-485">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="42a99-486">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="42a99-486">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="42a99-487">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="42a99-487">Data Lake Analytics</span></span>

* <span data-ttu-id="42a99-488">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="42a99-488">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="42a99-489">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="42a99-489">Data Lake Store</span></span>

* <span data-ttu-id="42a99-490">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="42a99-490">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="42a99-491">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="42a99-491">Extension</span></span>

* <span data-ttu-id="42a99-492">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="42a99-492">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="42a99-493">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="42a99-493">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="42a99-494">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="42a99-494">IoT</span></span>

* <span data-ttu-id="42a99-495">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="42a99-495">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="42a99-496">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="42a99-496">Monitor</span></span>

* <span data-ttu-id="42a99-497">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="42a99-497">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="42a99-498">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-498">Network</span></span>

* <span data-ttu-id="42a99-499">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="42a99-499">Added support for CAA DNS records</span></span>
* <span data-ttu-id="42a99-500">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-500">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="42a99-501">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="42a99-501">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="42a99-502">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="42a99-502">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="42a99-503">Резервирование</span><span class="sxs-lookup"><span data-stu-id="42a99-503">Reservations</span></span>

* <span data-ttu-id="42a99-504">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="42a99-504">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-505">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-505">Resource</span></span>

* <span data-ttu-id="42a99-506">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="42a99-506">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="42a99-507">SQL</span><span class="sxs-lookup"><span data-stu-id="42a99-507">SQL</span></span>

* <span data-ttu-id="42a99-508">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-508">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-509">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-509">Storage</span></span>

* <span data-ttu-id="42a99-510">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="42a99-510">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="42a99-511">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="42a99-511">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="42a99-512">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="42a99-512">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="42a99-513">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="42a99-513">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="42a99-514">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-514">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="42a99-515">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="42a99-515">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="42a99-516">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-516">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-517">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-517">VM</span></span>

* <span data-ttu-id="42a99-518">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="42a99-518">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="42a99-519">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="42a99-519">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="42a99-520">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="42a99-520">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="42a99-521">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="42a99-521">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="42a99-522">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="42a99-522">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="42a99-523">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-523">October 24, 2017</span></span>

<span data-ttu-id="42a99-524">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="42a99-524">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="42a99-525">Core</span><span class="sxs-lookup"><span data-stu-id="42a99-525">Core</span></span>

* <span data-ttu-id="42a99-526">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="42a99-526">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="42a99-527">ACR</span><span class="sxs-lookup"><span data-stu-id="42a99-527">ACR</span></span>

* <span data-ttu-id="42a99-528">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="42a99-528">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="42a99-529">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="42a99-529">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="42a99-530">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="42a99-530">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-531">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-531">ACS</span></span>

* <span data-ttu-id="42a99-532">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="42a99-532">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="42a99-533">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="42a99-533">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-534">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-534">Appservice</span></span>

* <span data-ttu-id="42a99-535">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="42a99-535">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="42a99-536">Компонент</span><span class="sxs-lookup"><span data-stu-id="42a99-536">Component</span></span>

* <span data-ttu-id="42a99-537">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="42a99-537">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="42a99-538">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="42a99-538">Monitor</span></span>

* <span data-ttu-id="42a99-539">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="42a99-539">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-540">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-540">Resource</span></span>

* <span data-ttu-id="42a99-541">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="42a99-541">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="42a99-542">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="42a99-542">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-543">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-543">VM</span></span>

* <span data-ttu-id="42a99-544">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="42a99-544">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="42a99-545">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-545">October 9, 2017</span></span>

<span data-ttu-id="42a99-546">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="42a99-546">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="42a99-547">Core</span><span class="sxs-lookup"><span data-stu-id="42a99-547">Core</span></span>

* <span data-ttu-id="42a99-548">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="42a99-548">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-549">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-549">Appservice</span></span>

* <span data-ttu-id="42a99-550">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-550">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="42a99-551">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="42a99-551">Batch</span></span>

* <span data-ttu-id="42a99-552">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="42a99-552">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="42a99-553">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="42a99-553">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="42a99-554">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="42a99-554">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="42a99-555">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="42a99-555">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="42a99-556">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="42a99-556">Batchai</span></span>

* <span data-ttu-id="42a99-557">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="42a99-557">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="42a99-558">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="42a99-558">Keyvault</span></span>

* <span data-ttu-id="42a99-559">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="42a99-559">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="42a99-560">(#4448)</span><span class="sxs-lookup"><span data-stu-id="42a99-560">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="42a99-561">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-561">Network</span></span>

* <span data-ttu-id="42a99-562">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="42a99-562">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="42a99-563">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="42a99-563">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-564">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-564">Resource</span></span>

* <span data-ttu-id="42a99-565">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="42a99-565">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="42a99-566">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="42a99-566">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="42a99-567">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="42a99-567">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="42a99-568">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="42a99-568">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="42a99-569">SQL</span><span class="sxs-lookup"><span data-stu-id="42a99-569">Sql</span></span>

* <span data-ttu-id="42a99-570">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="42a99-570">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="42a99-571">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="42a99-571">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="42a99-572">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="42a99-572">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-573">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-573">Storage</span></span>

* <span data-ttu-id="42a99-574">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="42a99-574">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-575">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="42a99-575">Vm</span></span>

* <span data-ttu-id="42a99-576">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="42a99-576">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="42a99-577">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-577">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="42a99-578">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="42a99-578">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="42a99-579">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-579">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="42a99-580">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="42a99-580">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="42a99-581">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-581">September 22, 2017</span></span>

<span data-ttu-id="42a99-582">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="42a99-582">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-583">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-583">Resource</span></span>

* <span data-ttu-id="42a99-584">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="42a99-584">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="42a99-585">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="42a99-585">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="42a99-586">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="42a99-586">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="42a99-587">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="42a99-587">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="42a99-588">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-588">Network</span></span>

* <span data-ttu-id="42a99-589">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="42a99-589">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="42a99-590">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="42a99-590">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="42a99-591">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="42a99-591">Added `asg` application security group commands</span></span>
* <span data-ttu-id="42a99-592">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="42a99-592">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="42a99-593">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="42a99-593">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="42a99-594">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="42a99-594">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="42a99-595">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-595">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-596">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-596">Storage</span></span>

* <span data-ttu-id="42a99-597">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="42a99-597">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="42a99-598">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="42a99-598">Eventgrid</span></span>

* <span data-ttu-id="42a99-599">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="42a99-599">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="42a99-600">SQL</span><span class="sxs-lookup"><span data-stu-id="42a99-600">SQL</span></span>

* <span data-ttu-id="42a99-601">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="42a99-601">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="42a99-602">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="42a99-602">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="42a99-603">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="42a99-603">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="42a99-604">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="42a99-604">Keyvault</span></span>

* <span data-ttu-id="42a99-605">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="42a99-605">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-606">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-606">VM</span></span>

* <span data-ttu-id="42a99-607">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="42a99-607">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="42a99-608">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="42a99-608">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="42a99-609">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="42a99-609">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="42a99-610">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="42a99-610">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="42a99-611">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="42a99-611">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="42a99-612">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="42a99-612">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-613">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-613">ACS</span></span>

* <span data-ttu-id="42a99-614">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="42a99-614">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-615">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-615">Appservice</span></span>

* <span data-ttu-id="42a99-616">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="42a99-616">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="42a99-617">Архивация</span><span class="sxs-lookup"><span data-stu-id="42a99-617">Backup</span></span>

* <span data-ttu-id="42a99-618">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="42a99-618">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="42a99-619">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-619">September 11, 2017</span></span>

<span data-ttu-id="42a99-620">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="42a99-620">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="42a99-621">Core</span><span class="sxs-lookup"><span data-stu-id="42a99-621">Core</span></span>

* <span data-ttu-id="42a99-622">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="42a99-622">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="42a99-623">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="42a99-623">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-624">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-624">Acs</span></span>

* <span data-ttu-id="42a99-625">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="42a99-625">Added `acs list-locations` command</span></span>
* <span data-ttu-id="42a99-626">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="42a99-626">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-627">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-627">Appservice</span></span>

* <span data-ttu-id="42a99-628">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="42a99-628">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="42a99-629">CDN</span><span class="sxs-lookup"><span data-stu-id="42a99-629">CDN</span></span>

* <span data-ttu-id="42a99-630">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-630">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="42a99-631">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="42a99-631">Extension</span></span>

* <span data-ttu-id="42a99-632">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="42a99-632">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="42a99-633">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="42a99-633">Keyvault</span></span>

* <span data-ttu-id="42a99-634">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="42a99-634">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="42a99-635">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-635">Network</span></span>

* <span data-ttu-id="42a99-636">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="42a99-636">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="42a99-637">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-637">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="42a99-638">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-638">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="42a99-639">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-639">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="42a99-640">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-640">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-641">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-641">Resource</span></span>

* <span data-ttu-id="42a99-642">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-642">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="42a99-643">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-643">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="42a99-644">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="42a99-644">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="42a99-645">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="42a99-645">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="42a99-646">SQL</span><span class="sxs-lookup"><span data-stu-id="42a99-646">SQL</span></span>

* <span data-ttu-id="42a99-647">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="42a99-647">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-648">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-648">VM</span></span>

* <span data-ttu-id="42a99-649">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="42a99-649">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="42a99-650">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="42a99-650">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="42a99-651">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-651">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="42a99-652">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="42a99-652">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="42a99-653">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="42a99-653">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="42a99-654">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-654">August 31, 2017</span></span>

<span data-ttu-id="42a99-655">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="42a99-655">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="42a99-656">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="42a99-656">Keyvault</span></span>

* <span data-ttu-id="42a99-657">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="42a99-657">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="42a99-658">Sf</span><span class="sxs-lookup"><span data-stu-id="42a99-658">Sf</span></span>

* <span data-ttu-id="42a99-659">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="42a99-659">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-660">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-660">Storage</span></span>

* <span data-ttu-id="42a99-661">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="42a99-661">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="42a99-662">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="42a99-662">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="42a99-663">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-663">August 28, 2017</span></span>

<span data-ttu-id="42a99-664">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="42a99-664">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="42a99-665">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="42a99-665">CLI</span></span>

* <span data-ttu-id="42a99-666">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="42a99-666">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-667">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-667">ACS</span></span>

* <span data-ttu-id="42a99-668">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="42a99-668">Corrected preview regions</span></span>
* <span data-ttu-id="42a99-669">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="42a99-669">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="42a99-670">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="42a99-670">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-671">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-671">Appservice</span></span>

* <span data-ttu-id="42a99-672">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-672">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="42a99-673">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="42a99-673">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="42a99-674">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="42a99-674">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="42a99-675">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="42a99-675">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="42a99-676">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="42a99-676">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="42a99-677">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="42a99-677">IoT</span></span>

* <span data-ttu-id="42a99-678">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="42a99-678">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="42a99-679">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-679">Network</span></span>

* <span data-ttu-id="42a99-680">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="42a99-680">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="42a99-681">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-681">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="42a99-682">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="42a99-682">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="42a99-683">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-683">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="42a99-684">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-684">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="42a99-685">Профиль</span><span class="sxs-lookup"><span data-stu-id="42a99-685">Profile</span></span>

* <span data-ttu-id="42a99-686">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="42a99-686">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="42a99-687">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="42a99-687">Service Fabric</span></span>

* <span data-ttu-id="42a99-688">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="42a99-688">Preview release</span></span>
* <span data-ttu-id="42a99-689">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="42a99-689">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="42a99-690">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="42a99-690">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="42a99-691">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="42a99-691">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-692">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-692">Storage</span></span>

* <span data-ttu-id="42a99-693">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="42a99-693">Enabled setting blob tier</span></span>
* <span data-ttu-id="42a99-694">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="42a99-694">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="42a99-695">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="42a99-695">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="42a99-696">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="42a99-696">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="42a99-697">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-697">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="42a99-698">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="42a99-698">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-699">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-699">VM</span></span>

* <span data-ttu-id="42a99-700">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="42a99-700">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="42a99-701">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-701">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="42a99-702">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="42a99-702">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="42a99-703">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="42a99-703">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="42a99-704">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="42a99-704">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="42a99-705">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-705">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="42a99-706">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-706">August 15, 2017</span></span>

<span data-ttu-id="42a99-707">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="42a99-707">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-708">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-708">ACS</span></span>

* <span data-ttu-id="42a99-709">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="42a99-709">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-710">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-710">Appservice</span></span>

* <span data-ttu-id="42a99-711">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="42a99-711">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="42a99-712">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="42a99-712">Event Grid</span></span>

* <span data-ttu-id="42a99-713">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="42a99-713">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="42a99-714">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-714">August 11, 2017</span></span>

<span data-ttu-id="42a99-715">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="42a99-715">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-716">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-716">ACS</span></span>

* <span data-ttu-id="42a99-717">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="42a99-717">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="42a99-718">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="42a99-718">Batch</span></span>

* <span data-ttu-id="42a99-719">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="42a99-719">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="42a99-720">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="42a99-720">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="42a99-721">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="42a99-721">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="42a99-722">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="42a99-722">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="42a99-723">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="42a99-723">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="42a99-724">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="42a99-724">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="42a99-725">Компонент</span><span class="sxs-lookup"><span data-stu-id="42a99-725">Component</span></span>

* <span data-ttu-id="42a99-726">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="42a99-726">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="42a99-727">Контейнер</span><span class="sxs-lookup"><span data-stu-id="42a99-727">Container</span></span>

* <span data-ttu-id="42a99-728">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="42a99-728">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="42a99-729">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="42a99-729">Data Lake Store</span></span>

* <span data-ttu-id="42a99-730">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="42a99-730">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="42a99-731">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="42a99-731">Event Grid</span></span>

* <span data-ttu-id="42a99-732">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="42a99-732">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="42a99-733">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-733">Network</span></span>

* <span data-ttu-id="42a99-734">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="42a99-734">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="42a99-735">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="42a99-735">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="42a99-736">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="42a99-736">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="42a99-737">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="42a99-737">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="42a99-738">Профиль</span><span class="sxs-lookup"><span data-stu-id="42a99-738">Profile</span></span>

* <span data-ttu-id="42a99-739">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="42a99-739">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-740">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-740">Storage</span></span>

* <span data-ttu-id="42a99-741">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="42a99-741">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-742">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-742">VM</span></span>

* <span data-ttu-id="42a99-743">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="42a99-743">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="42a99-744">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="42a99-744">Exposed `list-skus` command</span></span>
* <span data-ttu-id="42a99-745">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="42a99-745">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="42a99-746">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="42a99-746">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="42a99-747">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="42a99-747">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="42a99-748">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-748">July 28, 2017</span></span>

<span data-ttu-id="42a99-749">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="42a99-749">Version 2.0.12</span></span>

* <span data-ttu-id="42a99-750">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="42a99-750">Added container commands</span></span>
* <span data-ttu-id="42a99-751">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="42a99-751">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="42a99-752">Core</span><span class="sxs-lookup"><span data-stu-id="42a99-752">Core</span></span>

* <span data-ttu-id="42a99-753">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="42a99-753">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="42a99-754">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="42a99-754">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="42a99-755">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="42a99-755">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="42a99-756">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="42a99-756">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="42a99-757">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="42a99-757">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="42a99-758">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="42a99-758">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="42a99-759">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="42a99-759">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="42a99-760">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="42a99-760">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="42a99-761">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="42a99-761">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="42a99-762">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="42a99-762">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="42a99-763">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="42a99-763">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="42a99-764">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="42a99-764">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="42a99-765">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="42a99-765">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="42a99-766">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="42a99-766">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="42a99-767">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="42a99-767">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="42a99-768">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="42a99-768">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="42a99-769">ACR</span><span class="sxs-lookup"><span data-stu-id="42a99-769">ACR</span></span>

* <span data-ttu-id="42a99-770">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="42a99-770">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="42a99-771">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="42a99-771">Support SKU update for managed registries</span></span>
* <span data-ttu-id="42a99-772">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="42a99-772">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="42a99-773">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="42a99-773">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="42a99-774">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="42a99-774">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="42a99-775">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="42a99-775">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-776">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-776">ACS</span></span>

* <span data-ttu-id="42a99-777">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="42a99-777">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-778">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="42a99-778">Appservice</span></span>

* <span data-ttu-id="42a99-779">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="42a99-779">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="42a99-780">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="42a99-780">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="42a99-781">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="42a99-781">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="42a99-782">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="42a99-782">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="42a99-783">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="42a99-783">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="42a99-784">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="42a99-784">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="42a99-785">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="42a99-785">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="42a99-786">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="42a99-786">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="42a99-787">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="42a99-787">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="42a99-788">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="42a99-788">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="42a99-789">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="42a99-789">Batch</span></span>

* <span data-ttu-id="42a99-790">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="42a99-790">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="42a99-791">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="42a99-791">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="42a99-792">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="42a99-792">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="42a99-793">CDN</span><span class="sxs-lookup"><span data-stu-id="42a99-793">CDN</span></span>

* <span data-ttu-id="42a99-794">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="42a99-794">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="42a99-795">Облако</span><span class="sxs-lookup"><span data-stu-id="42a99-795">Cloud</span></span>

* <span data-ttu-id="42a99-796">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="42a99-796">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="42a99-797">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="42a99-797">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="42a99-798">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="42a99-798">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="42a99-799">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="42a99-799">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="42a99-800">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="42a99-800">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="42a99-801">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="42a99-801">CosmosDB</span></span>

* <span data-ttu-id="42a99-802">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="42a99-802">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="42a99-803">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="42a99-803">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="42a99-804">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="42a99-804">Data Lake Analytics</span></span>

* <span data-ttu-id="42a99-805">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="42a99-805">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="42a99-806">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="42a99-806">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="42a99-807">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="42a99-807">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="42a99-808">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="42a99-808">Data Lake Store</span></span>

* <span data-ttu-id="42a99-809">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-809">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="42a99-810">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="42a99-810">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="42a99-811">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="42a99-811">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="42a99-812">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="42a99-812">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="42a99-813">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="42a99-813">Interactive</span></span>

* <span data-ttu-id="42a99-814">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="42a99-814">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="42a99-815">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="42a99-815">Increased test coverage</span></span>
* <span data-ttu-id="42a99-816">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="42a99-816">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="42a99-817">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="42a99-817">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="42a99-818">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="42a99-818">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="42a99-819">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="42a99-819">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="42a99-820">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="42a99-820">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="42a99-821">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="42a99-821">Added `--progress` flag</span></span>
* <span data-ttu-id="42a99-822">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="42a99-822">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="42a99-823">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="42a99-823">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="42a99-824">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="42a99-824">IoT</span></span>

* <span data-ttu-id="42a99-825">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="42a99-825">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="42a99-826">(3934).</span><span class="sxs-lookup"><span data-stu-id="42a99-826">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="42a99-827">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="42a99-827">Key vault</span></span>

* <span data-ttu-id="42a99-828">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="42a99-828">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="42a99-829">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="42a99-829">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="42a99-830">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="42a99-830">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="42a99-831">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="42a99-831">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="42a99-832">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="42a99-832">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="42a99-833">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="42a99-833">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="42a99-834">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="42a99-834">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="42a99-835">(3307).</span><span class="sxs-lookup"><span data-stu-id="42a99-835">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="42a99-836">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="42a99-836">Lab</span></span>

* <span data-ttu-id="42a99-837">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="42a99-837">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="42a99-838">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="42a99-838">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="42a99-839">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="42a99-839">Monitor</span></span>

* <span data-ttu-id="42a99-840">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="42a99-840">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="42a99-841">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="42a99-841">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="42a99-842">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="42a99-842">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="42a99-843">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="42a99-843">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="42a99-844">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="42a99-844">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="42a99-845">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="42a99-845">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="42a99-846">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="42a99-846">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="42a99-847">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="42a99-847">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="42a99-848">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="42a99-848">`location` no longer required</span></span>
  * <span data-ttu-id="42a99-849">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="42a99-849">Add name and ID support for target</span></span>
  * <span data-ttu-id="42a99-850">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="42a99-850">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="42a99-851">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="42a99-851">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="42a99-852">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="42a99-852">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="42a99-853">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="42a99-853">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="42a99-854">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="42a99-854">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="42a99-855">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-855">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="42a99-856">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-856">Network</span></span>

* <span data-ttu-id="42a99-857">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="42a99-857">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="42a99-858">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-858">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="42a99-859">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="42a99-859">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="42a99-860">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="42a99-860">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="42a99-861">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-861">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="42a99-862">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="42a99-862">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="42a99-863">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="42a99-863">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="42a99-864">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="42a99-864">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="42a99-865">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="42a99-865">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="42a99-866">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="42a99-866">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="42a99-867">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-867">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="42a99-868">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="42a99-868">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="42a99-869">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="42a99-869">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="42a99-870">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-870">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="42a99-871">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-871">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="42a99-872">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-872">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="42a99-873">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="42a99-873">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="42a99-874">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="42a99-874">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="42a99-875">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-875">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="42a99-876">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-876">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="42a99-877">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-877">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="42a99-878">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="42a99-878">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="42a99-879">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="42a99-879">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="42a99-880">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="42a99-880">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="42a99-881">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="42a99-881">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="42a99-882">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="42a99-882">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="42a99-883">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="42a99-883">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="42a99-884">Профиль</span><span class="sxs-lookup"><span data-stu-id="42a99-884">Profile</span></span>

* <span data-ttu-id="42a99-885">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="42a99-885">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="42a99-886">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="42a99-886">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="42a99-887">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="42a99-887">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="42a99-888">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="42a99-888">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="42a99-889">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="42a99-889">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="42a99-890">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="42a99-890">RDBMS</span></span>

* <span data-ttu-id="42a99-891">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="42a99-891">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="42a99-892">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="42a99-892">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="42a99-893">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="42a99-893">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="42a99-894">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="42a99-894">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-895">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-895">Resource</span></span>

* <span data-ttu-id="42a99-896">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-896">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="42a99-897">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="42a99-897">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="42a99-898">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="42a99-898">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="42a99-899">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="42a99-899">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="42a99-900">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="42a99-900">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="42a99-901">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="42a99-901">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="42a99-902">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="42a99-902">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="42a99-903">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="42a99-903">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="42a99-904">Роль</span><span class="sxs-lookup"><span data-stu-id="42a99-904">Role</span></span>

* <span data-ttu-id="42a99-905">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="42a99-905">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="42a99-906">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="42a99-906">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="42a99-907">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="42a99-907">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="42a99-908">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="42a99-908">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="42a99-909">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="42a99-909">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="42a99-910">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="42a99-910">Service Fabric</span></span>
* <span data-ttu-id="42a99-911">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="42a99-911">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="42a99-912">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="42a99-912">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="42a99-913">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="42a99-913">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="42a99-914">SQL</span><span class="sxs-lookup"><span data-stu-id="42a99-914">SQL</span></span>

* <span data-ttu-id="42a99-915">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-915">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="42a99-916">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="42a99-916">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="42a99-917">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="42a99-917">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-918">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-918">Storage</span></span>

* <span data-ttu-id="42a99-919">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="42a99-919">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="42a99-920">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="42a99-920">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="42a99-921">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="42a99-921">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="42a99-922">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="42a99-922">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="42a99-923">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="42a99-923">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="42a99-924">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="42a99-924">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-925">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-925">VM</span></span>

* <span data-ttu-id="42a99-926">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="42a99-926">Support configuring nsg</span></span>
* <span data-ttu-id="42a99-927">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="42a99-927">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="42a99-928">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="42a99-928">Support managed service identities</span></span>
* <span data-ttu-id="42a99-929">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="42a99-929">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="42a99-930">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="42a99-930">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="42a99-931">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-931">May 10, 2017</span></span>

<span data-ttu-id="42a99-932">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="42a99-932">Version 2.0.6</span></span>

* <span data-ttu-id="42a99-933">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="42a99-933">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="42a99-934">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="42a99-934">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="42a99-935">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="42a99-935">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="42a99-936">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="42a99-936">Include Cognitive Services module</span></span>
* <span data-ttu-id="42a99-937">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="42a99-937">Include Service Fabric module</span></span>
* <span data-ttu-id="42a99-938">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="42a99-938">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="42a99-939">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="42a99-939">Add support for CDN commands</span></span>
* <span data-ttu-id="42a99-940">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="42a99-940">Remove Container module</span></span>
* <span data-ttu-id="42a99-941">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="42a99-941">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="42a99-942">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="42a99-942">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="42a99-943">Core</span><span class="sxs-lookup"><span data-stu-id="42a99-943">Core</span></span>

* <span data-ttu-id="42a99-944">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="42a99-944">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="42a99-945">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="42a99-945">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="42a99-946">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="42a99-946">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="42a99-947">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="42a99-947">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="42a99-948">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="42a99-948">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="42a99-949">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="42a99-949">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="42a99-950">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="42a99-950">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="42a99-951">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="42a99-951">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="42a99-952">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="42a99-952">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="42a99-953">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="42a99-953">core: Improved performance</span></span>
* <span data-ttu-id="42a99-954">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="42a99-954">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="42a99-955">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="42a99-955">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-956">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-956">ACS</span></span>

* <span data-ttu-id="42a99-957">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="42a99-957">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="42a99-958">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="42a99-958">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="42a99-959">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="42a99-959">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="42a99-960">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="42a99-960">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-961">AppService</span><span class="sxs-lookup"><span data-stu-id="42a99-961">AppService</span></span>

* <span data-ttu-id="42a99-962">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="42a99-962">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="42a99-963">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="42a99-963">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="42a99-964">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="42a99-964">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="42a99-965">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="42a99-965">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="42a99-966">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="42a99-966">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="42a99-967">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="42a99-967">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="42a99-968">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="42a99-968">support slot swap with preview</span></span>
* <span data-ttu-id="42a99-969">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="42a99-969">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="42a99-970">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="42a99-970">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="42a99-971">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="42a99-971">CosmosDB</span></span>

* <span data-ttu-id="42a99-972">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="42a99-972">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="42a99-973">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="42a99-973">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="42a99-974">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="42a99-974">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="42a99-975">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="42a99-975">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="42a99-976">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="42a99-976">Data Lake Analytics</span></span>

* <span data-ttu-id="42a99-977">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="42a99-977">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="42a99-978">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="42a99-978">Add support for new catalog item type: package.</span></span> <span data-ttu-id="42a99-979">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="42a99-979">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="42a99-980">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="42a99-980">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="42a99-981">Таблица</span><span class="sxs-lookup"><span data-stu-id="42a99-981">Table</span></span>
  * <span data-ttu-id="42a99-982">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="42a99-982">Table valued function</span></span>
  * <span data-ttu-id="42a99-983">Просмотр</span><span class="sxs-lookup"><span data-stu-id="42a99-983">View</span></span>
  * <span data-ttu-id="42a99-984">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="42a99-984">Table Statistics.</span></span> <span data-ttu-id="42a99-985">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="42a99-985">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="42a99-986">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="42a99-986">Data Lake Store</span></span>

* <span data-ttu-id="42a99-987">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="42a99-987">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="42a99-988">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="42a99-988">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="42a99-989">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="42a99-989">missed help for access show.</span></span> <span data-ttu-id="42a99-990">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="42a99-990">adding it.</span></span> <span data-ttu-id="42a99-991">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="42a99-991">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="42a99-992">Поиск</span><span class="sxs-lookup"><span data-stu-id="42a99-992">Find</span></span>

* <span data-ttu-id="42a99-993">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="42a99-993">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="42a99-994">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="42a99-994">KeyVault</span></span>

* <span data-ttu-id="42a99-995">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="42a99-995">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="42a99-996">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="42a99-996">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="42a99-997">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="42a99-997">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="42a99-998">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="42a99-998">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="42a99-999">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="42a99-999">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="42a99-1000">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="42a99-1000">Lab</span></span>

* <span data-ttu-id="42a99-1001">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="42a99-1001">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="42a99-1002">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="42a99-1002">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="42a99-1003">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="42a99-1003">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="42a99-1004">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="42a99-1004">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="42a99-1005">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="42a99-1005">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="42a99-1006">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="42a99-1006">Monitor</span></span>

* <span data-ttu-id="42a99-1007">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1007">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="42a99-1008">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1008">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="42a99-1009">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-1009">Network</span></span>

* <span data-ttu-id="42a99-1010">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="42a99-1010">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="42a99-1011">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-1011">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="42a99-1012">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="42a99-1012">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="42a99-1013">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="42a99-1013">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="42a99-1014">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="42a99-1014">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="42a99-1015">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="42a99-1015">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="42a99-1016">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="42a99-1016">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="42a99-1017">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="42a99-1017">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="42a99-1018">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="42a99-1018">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="42a99-1019">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="42a99-1019">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="42a99-1020">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="42a99-1020">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="42a99-1021">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-1021">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="42a99-1022">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="42a99-1022">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="42a99-1023">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="42a99-1023">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="42a99-1024">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="42a99-1024">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="42a99-1025">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="42a99-1025">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="42a99-1026">Профиль</span><span class="sxs-lookup"><span data-stu-id="42a99-1026">Profile</span></span>

* <span data-ttu-id="42a99-1027">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1027">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="42a99-1028">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1028">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="42a99-1029">Redis</span><span class="sxs-lookup"><span data-stu-id="42a99-1029">Redis</span></span>

* <span data-ttu-id="42a99-1030">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="42a99-1030">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="42a99-1031">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="42a99-1031">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="42a99-1032">Ресурс</span><span class="sxs-lookup"><span data-stu-id="42a99-1032">Resource</span></span>

* <span data-ttu-id="42a99-1033">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1033">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="42a99-1034">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1034">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="42a99-1035">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1035">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="42a99-1036">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="42a99-1036">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="42a99-1037">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="42a99-1037">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="42a99-1038">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="42a99-1038">Add docs for az lock update.</span></span> <span data-ttu-id="42a99-1039">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="42a99-1039">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="42a99-1040">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="42a99-1040">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="42a99-1041">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="42a99-1041">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="42a99-1042">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="42a99-1042">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="42a99-1043">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="42a99-1043">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="42a99-1044">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1044">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="42a99-1045">Роль</span><span class="sxs-lookup"><span data-stu-id="42a99-1045">Role</span></span>

* <span data-ttu-id="42a99-1046">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1046">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="42a99-1047">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1047">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="42a99-1048">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1048">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="42a99-1049">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="42a99-1049">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="42a99-1050">SQL</span><span class="sxs-lookup"><span data-stu-id="42a99-1050">SQL</span></span>

* <span data-ttu-id="42a99-1051">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="42a99-1051">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="42a99-1052">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1052">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="42a99-1053">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-1053">Storage</span></span>

* <span data-ttu-id="42a99-1054">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="42a99-1054">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="42a99-1055">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="42a99-1055">Add support for incremental blob copy</span></span>
* <span data-ttu-id="42a99-1056">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="42a99-1056">Add support for large block blob upload</span></span>
* <span data-ttu-id="42a99-1057">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="42a99-1057">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-1058">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-1058">VM</span></span>

* <span data-ttu-id="42a99-1059">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="42a99-1059">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="42a99-1060">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="42a99-1060">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="42a99-1061">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="42a99-1061">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="42a99-1062">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="42a99-1062">az vm/vmss disk</span></span>
  3. <span data-ttu-id="42a99-1063">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="42a99-1063">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="42a99-1064">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="42a99-1064">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="42a99-1065">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1065">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="42a99-1066">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-1066">April 3, 2017</span></span>

<span data-ttu-id="42a99-1067">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="42a99-1067">Version 2.0.2</span></span>

<span data-ttu-id="42a99-1068">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="42a99-1068">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="42a99-1069">Core</span><span class="sxs-lookup"><span data-stu-id="42a99-1069">Core</span></span>

* <span data-ttu-id="42a99-1070">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="42a99-1070">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="42a99-1071">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1071">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="42a99-1072">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1072">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="42a99-1073">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1073">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="42a99-1074">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1074">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="42a99-1075">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="42a99-1075">Add prompting for missing template parameters.</span></span> <span data-ttu-id="42a99-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1076">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="42a99-1077">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="42a99-1077">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="42a99-1078">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="42a99-1078">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="42a99-1079">ACS</span><span class="sxs-lookup"><span data-stu-id="42a99-1079">ACS</span></span>

* <span data-ttu-id="42a99-1080">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1080">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="42a99-1081">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="42a99-1081">Add support for ssh key password prompting.</span></span> <span data-ttu-id="42a99-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1082">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="42a99-1083">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="42a99-1083">Add support for windows clusters.</span></span> <span data-ttu-id="42a99-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1084">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="42a99-1085">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="42a99-1085">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="42a99-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1086">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="42a99-1087">AppService</span><span class="sxs-lookup"><span data-stu-id="42a99-1087">AppService</span></span>

* <span data-ttu-id="42a99-1088">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1088">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="42a99-1089">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1089">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="42a99-1090">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1090">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="42a99-1091">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1091">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="42a99-1092">Data Lake</span><span class="sxs-lookup"><span data-stu-id="42a99-1092">DataLake</span></span>

* <span data-ttu-id="42a99-1093">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="42a99-1093">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="42a99-1094">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="42a99-1094">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="42a99-1095">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="42a99-1095">DocuemntDB</span></span>

* <span data-ttu-id="42a99-1096">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1096">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="42a99-1097">ВМ</span><span class="sxs-lookup"><span data-stu-id="42a99-1097">VM</span></span>

* <span data-ttu-id="42a99-1098">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1098">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="42a99-1099">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1099">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="42a99-1100">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1100">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="42a99-1101">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1101">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="42a99-1102">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1102">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="42a99-1103">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1103">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="42a99-1104">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="42a99-1104">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="42a99-1105">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="42a99-1105">February 27, 2017</span></span>

<span data-ttu-id="42a99-1106">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="42a99-1106">Version 2.0.0</span></span>

<span data-ttu-id="42a99-1107">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="42a99-1107">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="42a99-1108">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="42a99-1108">Container Service (acs)</span></span>
- <span data-ttu-id="42a99-1109">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="42a99-1109">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="42a99-1110">Сеть</span><span class="sxs-lookup"><span data-stu-id="42a99-1110">Networking</span></span>
- <span data-ttu-id="42a99-1111">Хранилище</span><span class="sxs-lookup"><span data-stu-id="42a99-1111">Storage</span></span>

<span data-ttu-id="42a99-1112">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="42a99-1112">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="42a99-1113">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="42a99-1113">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="42a99-1114">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="42a99-1114">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="42a99-1115">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="42a99-1115">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="42a99-1116">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="42a99-1116">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="42a99-1117">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="42a99-1117">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="42a99-1118">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="42a99-1118">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="42a99-1119">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="42a99-1119">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="42a99-1120">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="42a99-1120">Provide feedback from the command line with the `az feedback` command</span></span>

