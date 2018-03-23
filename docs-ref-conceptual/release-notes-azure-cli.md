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
ms.openlocfilehash: 116fa95e51399b9b97c1b35c38445f30db7efc94
ms.sourcegitcommit: fefb5bb6a21cab30c44592c0577408a8d1a2ccc7
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/17/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="7552e-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="7552e-103">Azure CLI 2.0 release notes</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="7552e-104">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-104">March 13, 2018</span></span>

<span data-ttu-id="7552e-105">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="7552e-105">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="7552e-106">ACR</span><span class="sxs-lookup"><span data-stu-id="7552e-106">ACR</span></span>

* <span data-ttu-id="7552e-107">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="7552e-107">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="7552e-108">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="7552e-108">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="7552e-109">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="7552e-109">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-110">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-110">ACS</span></span>

* <span data-ttu-id="7552e-111">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="7552e-111">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="7552e-112">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="7552e-112">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="7552e-113">Помощник</span><span class="sxs-lookup"><span data-stu-id="7552e-113">Advisor</span></span>

* <span data-ttu-id="7552e-114">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="7552e-114">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="7552e-115">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-115">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="7552e-116">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="7552e-116">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="7552e-117">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="7552e-117">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="7552e-118">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="7552e-118">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-119">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-119">Appservice</span></span>

* <span data-ttu-id="7552e-120">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="7552e-120">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="7552e-121">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-121">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="7552e-122">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="7552e-122">Eventhubs</span></span>

* <span data-ttu-id="7552e-123">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="7552e-123">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="7552e-124">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="7552e-124">Extension</span></span>

* <span data-ttu-id="7552e-125">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="7552e-125">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="7552e-126">Interactive</span><span class="sxs-lookup"><span data-stu-id="7552e-126">Interactive</span></span>

* <span data-ttu-id="7552e-127">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="7552e-127">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="7552e-128">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="7552e-128">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="7552e-129">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="7552e-129">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="7552e-130">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="7552e-130">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="7552e-131">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="7552e-131">Monitor</span></span>

* <span data-ttu-id="7552e-132">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="7552e-132">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="7552e-133">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="7552e-133">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="7552e-134">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="7552e-134">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="7552e-135">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="7552e-135">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="7552e-136">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-136">Network</span></span>

* <span data-ttu-id="7552e-137">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-137">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="7552e-138">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="7552e-138">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="7552e-139">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="7552e-139">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="7552e-140">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="7552e-140">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="7552e-141">Профиль</span><span class="sxs-lookup"><span data-stu-id="7552e-141">Profile</span></span>

* <span data-ttu-id="7552e-142">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="7552e-142">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="7552e-143">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="7552e-143">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="7552e-144">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="7552e-144">RDBMS</span></span>

* <span data-ttu-id="7552e-145">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="7552e-145">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="7552e-146">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="7552e-146">Service Bus</span></span>

* <span data-ttu-id="7552e-147">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="7552e-147">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-148">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-148">Storage</span></span>

* <span data-ttu-id="7552e-149">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="7552e-149">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds.</span></span>
* <span data-ttu-id="7552e-150">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="7552e-150">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-151">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-151">VM</span></span>

* <span data-ttu-id="7552e-152">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="7552e-152">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="7552e-153">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="7552e-153">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="7552e-154">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-154">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="7552e-155">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="7552e-155">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="7552e-156">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="7552e-156">February 27, 2018</span></span>

<span data-ttu-id="7552e-157">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="7552e-157">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="7552e-158">Core</span><span class="sxs-lookup"><span data-stu-id="7552e-158">Core</span></span>

* <span data-ttu-id="7552e-159">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="7552e-159">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="7552e-160">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="7552e-160">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="7552e-161">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="7552e-161">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-162">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-162">ACS</span></span>

* <span data-ttu-id="7552e-163">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7552e-163">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="7552e-164">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="7552e-164">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="7552e-165">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="7552e-165">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="7552e-166">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="7552e-166">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-167">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-167">Appservice</span></span>

* <span data-ttu-id="7552e-168">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="7552e-168">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="7552e-169">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="7552e-169">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="7552e-170">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="7552e-170">Cognitive Services</span></span>

* <span data-ttu-id="7552e-171">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="7552e-171">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="7552e-172">Потребление</span><span class="sxs-lookup"><span data-stu-id="7552e-172">Consumption</span></span>

* <span data-ttu-id="7552e-173">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="7552e-173">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="7552e-174">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="7552e-174">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="7552e-175">Контейнер</span><span class="sxs-lookup"><span data-stu-id="7552e-175">Container</span></span>

* <span data-ttu-id="7552e-176">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="7552e-176">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="7552e-177">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-177">Network</span></span>

* <span data-ttu-id="7552e-178">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="7552e-178">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="7552e-179">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7552e-179">Resource</span></span>

* <span data-ttu-id="7552e-180">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="7552e-180">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="7552e-181">Роль</span><span class="sxs-lookup"><span data-stu-id="7552e-181">Role</span></span>

* <span data-ttu-id="7552e-182">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="7552e-182">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="7552e-183">SQL</span><span class="sxs-lookup"><span data-stu-id="7552e-183">SQL</span></span>

* <span data-ttu-id="7552e-184">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="7552e-184">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-185">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-185">Storage</span></span>

* <span data-ttu-id="7552e-186">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-186">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-187">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-187">VM</span></span>

* <span data-ttu-id="7552e-188">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="7552e-188">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="7552e-189">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-189">February 13, 2018</span></span>

<span data-ttu-id="7552e-190">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="7552e-190">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="7552e-191">Core</span><span class="sxs-lookup"><span data-stu-id="7552e-191">Core</span></span>

* <span data-ttu-id="7552e-192">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="7552e-192">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-193">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-193">ACS</span></span>

* <span data-ttu-id="7552e-194">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="7552e-194">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="7552e-195">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-195">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="7552e-196">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="7552e-196">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="7552e-197">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="7552e-197">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="7552e-198">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="7552e-198">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="7552e-199">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="7552e-199">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="7552e-200">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="7552e-200">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="7552e-201">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="7552e-201">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-202">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-202">Appservice</span></span>

* <span data-ttu-id="7552e-203">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="7552e-203">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="7552e-204">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="7552e-204">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="7552e-205">CDN</span><span class="sxs-lookup"><span data-stu-id="7552e-205">CDN</span></span>

* <span data-ttu-id="7552e-206">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-206">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="7552e-207">Контейнер</span><span class="sxs-lookup"><span data-stu-id="7552e-207">Container</span></span>

* <span data-ttu-id="7552e-208">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="7552e-208">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="7552e-209">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="7552e-209">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7552e-210">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7552e-210">CosmosDB</span></span>

* <span data-ttu-id="7552e-211">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="7552e-211">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="7552e-212">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="7552e-212">Extension</span></span>

* <span data-ttu-id="7552e-213">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-213">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="7552e-214">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-214">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="7552e-215">Отзыв</span><span class="sxs-lookup"><span data-stu-id="7552e-215">Feedback</span></span>

* <span data-ttu-id="7552e-216">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="7552e-216">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="7552e-217">Interactive</span><span class="sxs-lookup"><span data-stu-id="7552e-217">Interactive</span></span>

* <span data-ttu-id="7552e-218">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="7552e-218">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="7552e-219">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="7552e-219">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="7552e-220">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="7552e-220">IoT</span></span>

* <span data-ttu-id="7552e-221">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="7552e-221">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="7552e-222">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="7552e-222">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="7552e-223">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-223">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="7552e-224">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="7552e-224">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="7552e-225">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="7552e-225">Monitor</span></span>

* <span data-ttu-id="7552e-226">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-226">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="7552e-227">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-227">Network</span></span>

* <span data-ttu-id="7552e-228">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="7552e-228">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="7552e-229">Профиль</span><span class="sxs-lookup"><span data-stu-id="7552e-229">Profile</span></span>

* <span data-ttu-id="7552e-230">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="7552e-230">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="7552e-231">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7552e-231">Resource</span></span>

* <span data-ttu-id="7552e-232">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="7552e-232">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="7552e-233">Роль</span><span class="sxs-lookup"><span data-stu-id="7552e-233">Role</span></span>

* <span data-ttu-id="7552e-234">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="7552e-234">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="7552e-235">SQL</span><span class="sxs-lookup"><span data-stu-id="7552e-235">SQL</span></span>

* <span data-ttu-id="7552e-236">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="7552e-236">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="7552e-237">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="7552e-237">Added `sql db rename`</span></span>
* <span data-ttu-id="7552e-238">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="7552e-238">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-239">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-239">Storage</span></span>

* <span data-ttu-id="7552e-240">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="7552e-240">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-241">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-241">VM</span></span>

* <span data-ttu-id="7552e-242">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="7552e-242">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="7552e-243">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="7552e-243">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="7552e-244">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="7552e-244">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="7552e-245">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-245">January 31, 2018</span></span>

<span data-ttu-id="7552e-246">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="7552e-246">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="7552e-247">Core</span><span class="sxs-lookup"><span data-stu-id="7552e-247">Core</span></span>

* <span data-ttu-id="7552e-248">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="7552e-248">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="7552e-249">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="7552e-249">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="7552e-250">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="7552e-250">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="7552e-251">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="7552e-251">Use `--verbose` to see</span></span>
* <span data-ttu-id="7552e-252">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="7552e-252">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-253">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-253">ACS</span></span>

* <span data-ttu-id="7552e-254">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="7552e-254">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="7552e-255">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="7552e-255">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-256">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-256">Appservice</span></span>

* <span data-ttu-id="7552e-257">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="7552e-257">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="7552e-258">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="7552e-258">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="7552e-259">CDN</span><span class="sxs-lookup"><span data-stu-id="7552e-259">CDN</span></span>

* <span data-ttu-id="7552e-260">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-260">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7552e-261">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7552e-261">CosmosDB</span></span>

* <span data-ttu-id="7552e-262">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="7552e-262">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="7552e-263">Interactive</span><span class="sxs-lookup"><span data-stu-id="7552e-263">Interactive</span></span>

* <span data-ttu-id="7552e-264">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="7552e-264">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="7552e-265">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-265">Network</span></span>

* <span data-ttu-id="7552e-266">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-266">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="7552e-267">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7552e-267">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="7552e-268">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-268">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="7552e-269">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-269">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="7552e-270">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="7552e-270">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="7552e-271">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="7552e-271">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="7552e-272">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="7552e-272">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="7552e-273">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="7552e-273">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="7552e-274">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="7552e-274">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="7552e-275">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="7552e-275">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="7552e-276">Профиль</span><span class="sxs-lookup"><span data-stu-id="7552e-276">Profile</span></span>

* <span data-ttu-id="7552e-277">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="7552e-277">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="7552e-278">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7552e-278">Resource</span></span>

* <span data-ttu-id="7552e-279">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="7552e-279">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-280">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-280">Storage</span></span>

* <span data-ttu-id="7552e-281">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="7552e-281">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="7552e-282">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="7552e-282">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="7552e-283">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="7552e-283">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="7552e-284">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-284">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="7552e-285">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="7552e-285">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-286">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-286">VM</span></span>

* <span data-ttu-id="7552e-287">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="7552e-287">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="7552e-288">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="7552e-288">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="7552e-289">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="7552e-289">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="7552e-290">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-290">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="7552e-291">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-291">January 17, 2018</span></span>

<span data-ttu-id="7552e-292">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="7552e-292">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="7552e-293">ACR</span><span class="sxs-lookup"><span data-stu-id="7552e-293">ACR</span></span>

* <span data-ttu-id="7552e-294">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="7552e-294">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="7552e-295">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="7552e-295">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-296">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-296">ACS</span></span>

* <span data-ttu-id="7552e-297">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="7552e-297">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="7552e-298">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="7552e-298">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-299">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-299">Appservice</span></span>

* <span data-ttu-id="7552e-300">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="7552e-300">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="7552e-301">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="7552e-301">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="7552e-302">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="7552e-302">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="7552e-303">Архивация</span><span class="sxs-lookup"><span data-stu-id="7552e-303">Backup</span></span>

* <span data-ttu-id="7552e-304">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7552e-304">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="7552e-305">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="7552e-305">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="7552e-306">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="7552e-306">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="7552e-307">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="7552e-307">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="7552e-308">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="7552e-308">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="7552e-309">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="7552e-309">Batch</span></span>

* <span data-ttu-id="7552e-310">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="7552e-310">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="7552e-311">Облако</span><span class="sxs-lookup"><span data-stu-id="7552e-311">Cloud</span></span>

* <span data-ttu-id="7552e-312">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="7552e-312">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="7552e-313">Потребление</span><span class="sxs-lookup"><span data-stu-id="7552e-313">Consumption</span></span>

* <span data-ttu-id="7552e-314">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="7552e-314">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="7552e-315">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="7552e-315">Event Grid</span></span>

* <span data-ttu-id="7552e-316">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="7552e-316">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7552e-317">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="7552e-317">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="7552e-318">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="7552e-318">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="7552e-319">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="7552e-319">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="7552e-320">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-320">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="7552e-321">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-321">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="7552e-322">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="7552e-322">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="7552e-323">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="7552e-323">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="7552e-324">Interactive</span><span class="sxs-lookup"><span data-stu-id="7552e-324">Interactive</span></span>

* <span data-ttu-id="7552e-325">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="7552e-325">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="7552e-326">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="7552e-326">Fixed errors on startup</span></span>
* <span data-ttu-id="7552e-327">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="7552e-327">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="7552e-328">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="7552e-328">IoT</span></span>

* <span data-ttu-id="7552e-329">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="7552e-329">Added support for device provisioning service</span></span>
* <span data-ttu-id="7552e-330">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="7552e-330">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="7552e-331">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="7552e-331">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="7552e-332">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="7552e-332">Monitor</span></span>

* <span data-ttu-id="7552e-333">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="7552e-333">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="7552e-334">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-334">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="7552e-335">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="7552e-335">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="7552e-336">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-336">Network</span></span>

* <span data-ttu-id="7552e-337">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="7552e-337">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="7552e-338">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="7552e-338">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="7552e-339">Профиль</span><span class="sxs-lookup"><span data-stu-id="7552e-339">Profile</span></span>

* <span data-ttu-id="7552e-340">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="7552e-340">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="7552e-341">Роль</span><span class="sxs-lookup"><span data-stu-id="7552e-341">Role</span></span>

* <span data-ttu-id="7552e-342">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="7552e-342">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7552e-343">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7552e-343">Service Fabric</span></span>

* <span data-ttu-id="7552e-344">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="7552e-344">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="7552e-345">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="7552e-345">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-346">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-346">VM</span></span>

* <span data-ttu-id="7552e-347">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="7552e-347">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="7552e-348">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Значение по умолчанию `vmss` для одной зоны заменено на данные подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="7552e-348">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="7552e-349">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="7552e-349">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="7552e-350">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="7552e-350">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="7552e-351">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="7552e-351">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="7552e-352">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="7552e-352">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="7552e-353">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-353">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="7552e-354">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="7552e-354">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="7552e-355">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-355">December 19, 2017</span></span>

<span data-ttu-id="7552e-356">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="7552e-356">Version 2.0.23</span></span>

* <span data-ttu-id="7552e-357">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="7552e-357">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="7552e-358">Контейнер</span><span class="sxs-lookup"><span data-stu-id="7552e-358">Container</span></span>

* <span data-ttu-id="7552e-359">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="7552e-359">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="7552e-360">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-360">Network</span></span>

* <span data-ttu-id="7552e-361">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7552e-361">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="7552e-362">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7552e-362">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-363">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-363">Storage</span></span>

* <span data-ttu-id="7552e-364">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="7552e-364">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-365">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-365">VM</span></span>

* <span data-ttu-id="7552e-366">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="7552e-366">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="7552e-367">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-367">December 5, 2017</span></span>

<span data-ttu-id="7552e-368">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="7552e-368">Version 2.0.22</span></span>

* <span data-ttu-id="7552e-369">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="7552e-369">Removed `az component` commands.</span></span> <span data-ttu-id="7552e-370">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="7552e-370">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="7552e-371">Core</span><span class="sxs-lookup"><span data-stu-id="7552e-371">Core</span></span>
* <span data-ttu-id="7552e-372">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="7552e-372">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="7552e-373">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="7552e-373">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-374">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-374">ACS</span></span>

* <span data-ttu-id="7552e-375">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="7552e-375">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="7552e-376">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-376">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="7552e-377">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="7552e-377">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="7552e-378">Помощник</span><span class="sxs-lookup"><span data-stu-id="7552e-378">Advisor</span></span>

* <span data-ttu-id="7552e-379">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="7552e-379">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-380">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-380">Appservice</span></span>

* <span data-ttu-id="7552e-381">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="7552e-381">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="7552e-382">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="7552e-382">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="7552e-383">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="7552e-383">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="7552e-384">Потребление</span><span class="sxs-lookup"><span data-stu-id="7552e-384">Consumption</span></span>

* <span data-ttu-id="7552e-385">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="7552e-385">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="7552e-386">Контейнер</span><span class="sxs-lookup"><span data-stu-id="7552e-386">Container</span></span>

* <span data-ttu-id="7552e-387">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="7552e-387">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="7552e-388">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="7552e-388">Monitor</span></span>

* <span data-ttu-id="7552e-389">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="7552e-389">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="7552e-390">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7552e-390">Resource</span></span>

* <span data-ttu-id="7552e-391">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="7552e-391">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="7552e-392">Роль</span><span class="sxs-lookup"><span data-stu-id="7552e-392">Role</span></span>

* <span data-ttu-id="7552e-393">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="7552e-393">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="7552e-394">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="7552e-394">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="7552e-395">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="7552e-395">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="7552e-396">SQL</span><span class="sxs-lookup"><span data-stu-id="7552e-396">SQL</span></span>

* <span data-ttu-id="7552e-397">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="7552e-397">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="7552e-398">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-398">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-399">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-399">VM</span></span>

* <span data-ttu-id="7552e-400">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="7552e-400">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="7552e-401">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-401">November 14, 2017</span></span>

<span data-ttu-id="7552e-402">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="7552e-402">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="7552e-403">ACR</span><span class="sxs-lookup"><span data-stu-id="7552e-403">ACR</span></span>

* <span data-ttu-id="7552e-404">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="7552e-404">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="7552e-405">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-405">ACS</span></span>

* <span data-ttu-id="7552e-406">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="7552e-406">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="7552e-407">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="7552e-407">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="7552e-408">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="7552e-408">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="7552e-409">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="7552e-409">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="7552e-410">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="7552e-410">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-411">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-411">Appservice</span></span>

* <span data-ttu-id="7552e-412">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="7552e-412">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="7552e-413">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="7552e-413">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="7552e-414">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="7552e-414">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="7552e-415">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="7552e-415">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="7552e-416">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="7552e-416">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="7552e-417">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="7552e-417">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="7552e-418">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="7552e-418">Batch</span></span>

* <span data-ttu-id="7552e-419">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="7552e-419">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="7552e-420">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="7552e-420">Batchai</span></span>

* <span data-ttu-id="7552e-421">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-421">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="7552e-422">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-422">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="7552e-423">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="7552e-423">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="7552e-424">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-424">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="7552e-425">Облако</span><span class="sxs-lookup"><span data-stu-id="7552e-425">Cloud</span></span>

* <span data-ttu-id="7552e-426">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="7552e-426">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="7552e-427">Контейнер</span><span class="sxs-lookup"><span data-stu-id="7552e-427">Container</span></span>

* <span data-ttu-id="7552e-428">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="7552e-428">Added support to open multiple ports</span></span>
* <span data-ttu-id="7552e-429">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="7552e-429">Added container group restart policy</span></span>
* <span data-ttu-id="7552e-430">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="7552e-430">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="7552e-431">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="7552e-431">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7552e-432">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7552e-432">Data Lake Analytics</span></span>

* <span data-ttu-id="7552e-433">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="7552e-433">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7552e-434">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7552e-434">Data Lake Store</span></span>

* <span data-ttu-id="7552e-435">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="7552e-435">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="7552e-436">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="7552e-436">Extension</span></span>

* <span data-ttu-id="7552e-437">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="7552e-437">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="7552e-438">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="7552e-438">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="7552e-439">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="7552e-439">IoT</span></span>

* <span data-ttu-id="7552e-440">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="7552e-440">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="7552e-441">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="7552e-441">Monitor</span></span>

* <span data-ttu-id="7552e-442">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="7552e-442">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="7552e-443">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-443">Network</span></span>

* <span data-ttu-id="7552e-444">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="7552e-444">Added support for CAA DNS records</span></span>
* <span data-ttu-id="7552e-445">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-445">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="7552e-446">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="7552e-446">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="7552e-447">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="7552e-447">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="7552e-448">Резервирование</span><span class="sxs-lookup"><span data-stu-id="7552e-448">Reservations</span></span>

* <span data-ttu-id="7552e-449">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="7552e-449">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="7552e-450">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7552e-450">Resource</span></span>

* <span data-ttu-id="7552e-451">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="7552e-451">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7552e-452">SQL</span><span class="sxs-lookup"><span data-stu-id="7552e-452">SQL</span></span>

* <span data-ttu-id="7552e-453">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-453">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-454">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-454">Storage</span></span>

* <span data-ttu-id="7552e-455">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7552e-455">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="7552e-456">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="7552e-456">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="7552e-457">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="7552e-457">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="7552e-458">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="7552e-458">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="7552e-459">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-459">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="7552e-460">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="7552e-460">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="7552e-461">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-461">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-462">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-462">VM</span></span>

* <span data-ttu-id="7552e-463">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="7552e-463">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="7552e-464">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="7552e-464">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="7552e-465">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="7552e-465">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="7552e-466">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="7552e-466">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="7552e-467">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="7552e-467">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="7552e-468">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-468">October 24, 2017</span></span>

<span data-ttu-id="7552e-469">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="7552e-469">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="7552e-470">Core</span><span class="sxs-lookup"><span data-stu-id="7552e-470">Core</span></span>

* <span data-ttu-id="7552e-471">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="7552e-471">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="7552e-472">ACR</span><span class="sxs-lookup"><span data-stu-id="7552e-472">ACR</span></span>

* <span data-ttu-id="7552e-473">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="7552e-473">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="7552e-474">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="7552e-474">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="7552e-475">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="7552e-475">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-476">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-476">ACS</span></span>

* <span data-ttu-id="7552e-477">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="7552e-477">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="7552e-478">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="7552e-478">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-479">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-479">Appservice</span></span>

* <span data-ttu-id="7552e-480">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="7552e-480">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="7552e-481">Компонент</span><span class="sxs-lookup"><span data-stu-id="7552e-481">Component</span></span>

* <span data-ttu-id="7552e-482">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="7552e-482">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="7552e-483">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="7552e-483">Monitor</span></span>

* <span data-ttu-id="7552e-484">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="7552e-484">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="7552e-485">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7552e-485">Resource</span></span>

* <span data-ttu-id="7552e-486">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="7552e-486">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="7552e-487">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="7552e-487">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-488">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-488">VM</span></span>

* <span data-ttu-id="7552e-489">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="7552e-489">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="7552e-490">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-490">October 9, 2017</span></span>

<span data-ttu-id="7552e-491">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="7552e-491">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="7552e-492">Core</span><span class="sxs-lookup"><span data-stu-id="7552e-492">Core</span></span>

* <span data-ttu-id="7552e-493">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="7552e-493">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-494">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-494">Appservice</span></span>

* <span data-ttu-id="7552e-495">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-495">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="7552e-496">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="7552e-496">Batch</span></span>

* <span data-ttu-id="7552e-497">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="7552e-497">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="7552e-498">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="7552e-498">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="7552e-499">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="7552e-499">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="7552e-500">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="7552e-500">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="7552e-501">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="7552e-501">Batchai</span></span>

* <span data-ttu-id="7552e-502">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="7552e-502">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="7552e-503">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="7552e-503">Keyvault</span></span>

* <span data-ttu-id="7552e-504">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7552e-504">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="7552e-505">(#4448)</span><span class="sxs-lookup"><span data-stu-id="7552e-505">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="7552e-506">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-506">Network</span></span>

* <span data-ttu-id="7552e-507">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="7552e-507">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="7552e-508">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="7552e-508">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="7552e-509">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7552e-509">Resource</span></span>

* <span data-ttu-id="7552e-510">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="7552e-510">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="7552e-511">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="7552e-511">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="7552e-512">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="7552e-512">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="7552e-513">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="7552e-513">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="7552e-514">SQL</span><span class="sxs-lookup"><span data-stu-id="7552e-514">Sql</span></span>

* <span data-ttu-id="7552e-515">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="7552e-515">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="7552e-516">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="7552e-516">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="7552e-517">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="7552e-517">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-518">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-518">Storage</span></span>

* <span data-ttu-id="7552e-519">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7552e-519">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-520">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="7552e-520">Vm</span></span>

* <span data-ttu-id="7552e-521">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="7552e-521">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="7552e-522">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-522">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="7552e-523">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="7552e-523">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="7552e-524">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-524">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="7552e-525">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="7552e-525">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="7552e-526">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-526">September 22, 2017</span></span>

<span data-ttu-id="7552e-527">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="7552e-527">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="7552e-528">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7552e-528">Resource</span></span>

* <span data-ttu-id="7552e-529">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="7552e-529">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="7552e-530">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="7552e-530">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="7552e-531">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="7552e-531">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="7552e-532">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="7552e-532">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="7552e-533">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-533">Network</span></span>

* <span data-ttu-id="7552e-534">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="7552e-534">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="7552e-535">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="7552e-535">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="7552e-536">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="7552e-536">Added `asg` application security group commands</span></span>
* <span data-ttu-id="7552e-537">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="7552e-537">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="7552e-538">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7552e-538">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7552e-539">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7552e-539">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="7552e-540">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-540">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-541">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-541">Storage</span></span>

* <span data-ttu-id="7552e-542">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="7552e-542">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="7552e-543">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="7552e-543">Eventgrid</span></span>

* <span data-ttu-id="7552e-544">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="7552e-544">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="7552e-545">SQL</span><span class="sxs-lookup"><span data-stu-id="7552e-545">SQL</span></span>

* <span data-ttu-id="7552e-546">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="7552e-546">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="7552e-547">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="7552e-547">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="7552e-548">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="7552e-548">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="7552e-549">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="7552e-549">Keyvault</span></span>

* <span data-ttu-id="7552e-550">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="7552e-550">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-551">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-551">VM</span></span>

* <span data-ttu-id="7552e-552">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="7552e-552">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="7552e-553">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="7552e-553">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="7552e-554">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="7552e-554">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="7552e-555">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="7552e-555">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="7552e-556">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="7552e-556">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="7552e-557">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="7552e-557">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-558">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-558">ACS</span></span>

* <span data-ttu-id="7552e-559">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="7552e-559">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-560">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-560">Appservice</span></span>

* <span data-ttu-id="7552e-561">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="7552e-561">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="7552e-562">Архивация</span><span class="sxs-lookup"><span data-stu-id="7552e-562">Backup</span></span>

* <span data-ttu-id="7552e-563">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="7552e-563">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="7552e-564">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-564">September 11, 2017</span></span>

<span data-ttu-id="7552e-565">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="7552e-565">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="7552e-566">Core</span><span class="sxs-lookup"><span data-stu-id="7552e-566">Core</span></span>

* <span data-ttu-id="7552e-567">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="7552e-567">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="7552e-568">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="7552e-568">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-569">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-569">Acs</span></span>

* <span data-ttu-id="7552e-570">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="7552e-570">Added `acs list-locations` command</span></span>
* <span data-ttu-id="7552e-571">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7552e-571">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-572">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-572">Appservice</span></span>

* <span data-ttu-id="7552e-573">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="7552e-573">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="7552e-574">CDN</span><span class="sxs-lookup"><span data-stu-id="7552e-574">CDN</span></span>

* <span data-ttu-id="7552e-575">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-575">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="7552e-576">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="7552e-576">Extension</span></span>

* <span data-ttu-id="7552e-577">Первый выпуск.</span><span class="sxs-lookup"><span data-stu-id="7552e-577">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="7552e-578">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="7552e-578">Keyvault</span></span>

* <span data-ttu-id="7552e-579">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="7552e-579">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="7552e-580">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-580">Network</span></span>

* <span data-ttu-id="7552e-581">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="7552e-581">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7552e-582">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-582">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="7552e-583">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-583">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="7552e-584">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-584">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7552e-585">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-585">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="7552e-586">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7552e-586">Resource</span></span>

* <span data-ttu-id="7552e-587">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-587">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="7552e-588">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-588">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="7552e-589">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="7552e-589">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="7552e-590">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="7552e-590">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="7552e-591">SQL</span><span class="sxs-lookup"><span data-stu-id="7552e-591">SQL</span></span>

* <span data-ttu-id="7552e-592">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="7552e-592">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-593">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-593">VM</span></span>

* <span data-ttu-id="7552e-594">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="7552e-594">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="7552e-595">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="7552e-595">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="7552e-596">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-596">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="7552e-597">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="7552e-597">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="7552e-598">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="7552e-598">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="7552e-599">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-599">August 31, 2017</span></span>

<span data-ttu-id="7552e-600">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="7552e-600">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="7552e-601">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="7552e-601">Keyvault</span></span>

* <span data-ttu-id="7552e-602">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="7552e-602">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="7552e-603">Sf</span><span class="sxs-lookup"><span data-stu-id="7552e-603">Sf</span></span>

* <span data-ttu-id="7552e-604">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="7552e-604">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-605">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-605">Storage</span></span>

* <span data-ttu-id="7552e-606">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="7552e-606">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="7552e-607">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="7552e-607">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="7552e-608">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-608">August 28, 2017</span></span>

<span data-ttu-id="7552e-609">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="7552e-609">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="7552e-610">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="7552e-610">CLI</span></span>

* <span data-ttu-id="7552e-611">К параметру `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="7552e-611">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-612">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-612">ACS</span></span>

* <span data-ttu-id="7552e-613">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="7552e-613">Corrected preview regions.</span></span>
* <span data-ttu-id="7552e-614">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="7552e-614">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="7552e-615">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="7552e-615">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-616">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-616">Appservice</span></span>

* <span data-ttu-id="7552e-617">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-617">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="7552e-618">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="7552e-618">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="7552e-619">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="7552e-619">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="7552e-620">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="7552e-620">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="7552e-621">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="7552e-621">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="7552e-622">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="7552e-622">IoT</span></span>

* <span data-ttu-id="7552e-623">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="7552e-623">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="7552e-624">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-624">Network</span></span>

* <span data-ttu-id="7552e-625">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="7552e-625">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="7552e-626">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-626">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="7552e-627">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="7552e-627">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="7552e-628">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-628">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="7552e-629">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-629">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="7552e-630">Профиль</span><span class="sxs-lookup"><span data-stu-id="7552e-630">Profile</span></span>

* <span data-ttu-id="7552e-631">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="7552e-631">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7552e-632">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7552e-632">Service Fabric</span></span>

* <span data-ttu-id="7552e-633">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="7552e-633">Preview release</span></span>
* <span data-ttu-id="7552e-634">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="7552e-634">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="7552e-635">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="7552e-635">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="7552e-636">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="7552e-636">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-637">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-637">Storage</span></span>

* <span data-ttu-id="7552e-638">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="7552e-638">Enabled setting blob tier</span></span>
* <span data-ttu-id="7552e-639">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="7552e-639">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="7552e-640">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="7552e-640">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="7552e-641">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="7552e-641">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="7552e-642">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-642">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="7552e-643">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="7552e-643">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-644">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-644">VM</span></span>

* <span data-ttu-id="7552e-645">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="7552e-645">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="7552e-646">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-646">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="7552e-647">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="7552e-647">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="7552e-648">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="7552e-648">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="7552e-649">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="7552e-649">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="7552e-650">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-650">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="7552e-651">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-651">August 15, 2017</span></span>

<span data-ttu-id="7552e-652">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="7552e-652">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-653">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-653">ACS</span></span>

* <span data-ttu-id="7552e-654">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="7552e-654">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-655">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-655">Appservice</span></span>

* <span data-ttu-id="7552e-656">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="7552e-656">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="7552e-657">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="7552e-657">Event Grid</span></span>

* <span data-ttu-id="7552e-658">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="7552e-658">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="7552e-659">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-659">August 11, 2017</span></span>

<span data-ttu-id="7552e-660">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="7552e-660">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-661">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-661">ACS</span></span>

* <span data-ttu-id="7552e-662">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="7552e-662">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="7552e-663">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="7552e-663">Batch</span></span>

* <span data-ttu-id="7552e-664">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="7552e-664">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="7552e-665">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="7552e-665">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="7552e-666">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7552e-666">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="7552e-667">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="7552e-667">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="7552e-668">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="7552e-668">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="7552e-669">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="7552e-669">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="7552e-670">Компонент</span><span class="sxs-lookup"><span data-stu-id="7552e-670">Component</span></span>

* <span data-ttu-id="7552e-671">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="7552e-671">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="7552e-672">Контейнер</span><span class="sxs-lookup"><span data-stu-id="7552e-672">Container</span></span>

* <span data-ttu-id="7552e-673">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="7552e-673">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="7552e-674">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7552e-674">Data Lake Store</span></span>

* <span data-ttu-id="7552e-675">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="7552e-675">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="7552e-676">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="7552e-676">Event Grid</span></span>

* <span data-ttu-id="7552e-677">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="7552e-677">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="7552e-678">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-678">Network</span></span>

* <span data-ttu-id="7552e-679">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="7552e-679">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="7552e-680">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="7552e-680">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="7552e-681">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="7552e-681">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="7552e-682">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="7552e-682">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="7552e-683">Профиль</span><span class="sxs-lookup"><span data-stu-id="7552e-683">Profile</span></span>

* <span data-ttu-id="7552e-684">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="7552e-684">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-685">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-685">Storage</span></span>

* <span data-ttu-id="7552e-686">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="7552e-686">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-687">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-687">VM</span></span>

* <span data-ttu-id="7552e-688">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="7552e-688">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="7552e-689">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="7552e-689">Exposed `list-skus` command</span></span>
* <span data-ttu-id="7552e-690">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="7552e-690">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="7552e-691">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="7552e-691">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="7552e-692">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="7552e-692">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="7552e-693">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-693">July 28, 2017</span></span>

<span data-ttu-id="7552e-694">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="7552e-694">Version 2.0.12</span></span>

* <span data-ttu-id="7552e-695">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="7552e-695">Added container commands</span></span>
* <span data-ttu-id="7552e-696">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="7552e-696">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="7552e-697">Core</span><span class="sxs-lookup"><span data-stu-id="7552e-697">Core</span></span>

* <span data-ttu-id="7552e-698">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="7552e-698">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="7552e-699">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="7552e-699">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="7552e-700">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="7552e-700">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="7552e-701">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="7552e-701">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="7552e-702">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="7552e-702">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="7552e-703">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="7552e-703">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="7552e-704">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="7552e-704">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7552e-705">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="7552e-705">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="7552e-706">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="7552e-706">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="7552e-707">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="7552e-707">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="7552e-708">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="7552e-708">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="7552e-709">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="7552e-709">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="7552e-710">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="7552e-710">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="7552e-711">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="7552e-711">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="7552e-712">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="7552e-712">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="7552e-713">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="7552e-713">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="7552e-714">ACR</span><span class="sxs-lookup"><span data-stu-id="7552e-714">ACR</span></span>

* <span data-ttu-id="7552e-715">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="7552e-715">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="7552e-716">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="7552e-716">Support SKU update for managed registries</span></span>
* <span data-ttu-id="7552e-717">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="7552e-717">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="7552e-718">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="7552e-718">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="7552e-719">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="7552e-719">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="7552e-720">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="7552e-720">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-721">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-721">ACS</span></span>

* <span data-ttu-id="7552e-722">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="7552e-722">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-723">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="7552e-723">Appservice</span></span>

* <span data-ttu-id="7552e-724">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="7552e-724">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="7552e-725">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="7552e-725">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="7552e-726">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="7552e-726">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="7552e-727">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="7552e-727">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="7552e-728">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="7552e-728">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="7552e-729">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="7552e-729">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="7552e-730">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="7552e-730">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="7552e-731">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="7552e-731">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="7552e-732">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="7552e-732">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="7552e-733">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="7552e-733">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="7552e-734">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="7552e-734">Batch</span></span>

* <span data-ttu-id="7552e-735">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="7552e-735">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="7552e-736">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="7552e-736">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="7552e-737">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="7552e-737">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="7552e-738">CDN</span><span class="sxs-lookup"><span data-stu-id="7552e-738">CDN</span></span>

* <span data-ttu-id="7552e-739">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="7552e-739">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="7552e-740">Облако</span><span class="sxs-lookup"><span data-stu-id="7552e-740">Cloud</span></span>

* <span data-ttu-id="7552e-741">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="7552e-741">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="7552e-742">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="7552e-742">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="7552e-743">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="7552e-743">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="7552e-744">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="7552e-744">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="7552e-745">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="7552e-745">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7552e-746">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7552e-746">CosmosDB</span></span>

* <span data-ttu-id="7552e-747">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="7552e-747">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="7552e-748">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="7552e-748">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7552e-749">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7552e-749">Data Lake Analytics</span></span>

* <span data-ttu-id="7552e-750">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="7552e-750">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="7552e-751">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="7552e-751">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="7552e-752">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="7552e-752">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7552e-753">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7552e-753">Data Lake Store</span></span>

* <span data-ttu-id="7552e-754">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-754">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="7552e-755">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="7552e-755">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="7552e-756">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="7552e-756">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="7552e-757">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="7552e-757">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="7552e-758">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="7552e-758">Interactive</span></span>

* <span data-ttu-id="7552e-759">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="7552e-759">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="7552e-760">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="7552e-760">Increased test coverage</span></span>
* <span data-ttu-id="7552e-761">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="7552e-761">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="7552e-762">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="7552e-762">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="7552e-763">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="7552e-763">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="7552e-764">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="7552e-764">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="7552e-765">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="7552e-765">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="7552e-766">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="7552e-766">Added `--progress` flag</span></span>
* <span data-ttu-id="7552e-767">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="7552e-767">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="7552e-768">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="7552e-768">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="7552e-769">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="7552e-769">IoT</span></span>

* <span data-ttu-id="7552e-770">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="7552e-770">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="7552e-771">(3934).</span><span class="sxs-lookup"><span data-stu-id="7552e-771">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="7552e-772">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="7552e-772">Key vault</span></span>

* <span data-ttu-id="7552e-773">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="7552e-773">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="7552e-774">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="7552e-774">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="7552e-775">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="7552e-775">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7552e-776">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="7552e-776">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="7552e-777">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="7552e-777">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="7552e-778">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="7552e-778">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="7552e-779">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="7552e-779">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="7552e-780">(3307).</span><span class="sxs-lookup"><span data-stu-id="7552e-780">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="7552e-781">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="7552e-781">Lab</span></span>

* <span data-ttu-id="7552e-782">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="7552e-782">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="7552e-783">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="7552e-783">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="7552e-784">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="7552e-784">Monitor</span></span>

* <span data-ttu-id="7552e-785">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="7552e-785">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="7552e-786">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="7552e-786">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="7552e-787">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="7552e-787">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="7552e-788">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="7552e-788">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="7552e-789">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="7552e-789">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="7552e-790">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="7552e-790">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="7552e-791">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="7552e-791">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="7552e-792">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="7552e-792">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="7552e-793">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="7552e-793">`location` no longer required</span></span>
  * <span data-ttu-id="7552e-794">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="7552e-794">Add name and ID support for target</span></span>
  * <span data-ttu-id="7552e-795">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="7552e-795">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="7552e-796">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="7552e-796">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="7552e-797">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="7552e-797">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="7552e-798">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="7552e-798">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="7552e-799">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="7552e-799">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="7552e-800">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-800">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="7552e-801">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-801">Network</span></span>

* <span data-ttu-id="7552e-802">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="7552e-802">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="7552e-803">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-803">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="7552e-804">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="7552e-804">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="7552e-805">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="7552e-805">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="7552e-806">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-806">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="7552e-807">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="7552e-807">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="7552e-808">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="7552e-808">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="7552e-809">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="7552e-809">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="7552e-810">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="7552e-810">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="7552e-811">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="7552e-811">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="7552e-812">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-812">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="7552e-813">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="7552e-813">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="7552e-814">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="7552e-814">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="7552e-815">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-815">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="7552e-816">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-816">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="7552e-817">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-817">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="7552e-818">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="7552e-818">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="7552e-819">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="7552e-819">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="7552e-820">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-820">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="7552e-821">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-821">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="7552e-822">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-822">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="7552e-823">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="7552e-823">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="7552e-824">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="7552e-824">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="7552e-825">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="7552e-825">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="7552e-826">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="7552e-826">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="7552e-827">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="7552e-827">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="7552e-828">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="7552e-828">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="7552e-829">Профиль</span><span class="sxs-lookup"><span data-stu-id="7552e-829">Profile</span></span>

* <span data-ttu-id="7552e-830">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="7552e-830">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="7552e-831">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="7552e-831">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="7552e-832">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="7552e-832">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="7552e-833">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="7552e-833">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="7552e-834">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="7552e-834">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="7552e-835">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="7552e-835">RDBMS</span></span>

* <span data-ttu-id="7552e-836">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="7552e-836">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="7552e-837">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="7552e-837">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="7552e-838">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="7552e-838">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="7552e-839">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="7552e-839">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="7552e-840">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7552e-840">Resource</span></span>

* <span data-ttu-id="7552e-841">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-841">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="7552e-842">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="7552e-842">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="7552e-843">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="7552e-843">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="7552e-844">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="7552e-844">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="7552e-845">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="7552e-845">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="7552e-846">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="7552e-846">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="7552e-847">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="7552e-847">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="7552e-848">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="7552e-848">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="7552e-849">Роль</span><span class="sxs-lookup"><span data-stu-id="7552e-849">Role</span></span>

* <span data-ttu-id="7552e-850">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="7552e-850">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="7552e-851">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="7552e-851">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="7552e-852">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="7552e-852">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="7552e-853">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="7552e-853">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="7552e-854">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="7552e-854">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="7552e-855">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7552e-855">Service Fabric</span></span>
* <span data-ttu-id="7552e-856">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="7552e-856">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="7552e-857">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="7552e-857">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="7552e-858">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="7552e-858">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="7552e-859">SQL</span><span class="sxs-lookup"><span data-stu-id="7552e-859">SQL</span></span>

* <span data-ttu-id="7552e-860">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-860">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="7552e-861">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="7552e-861">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="7552e-862">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="7552e-862">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-863">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-863">Storage</span></span>

* <span data-ttu-id="7552e-864">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="7552e-864">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="7552e-865">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="7552e-865">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="7552e-866">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="7552e-866">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="7552e-867">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="7552e-867">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="7552e-868">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="7552e-868">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="7552e-869">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="7552e-869">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-870">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-870">VM</span></span>

* <span data-ttu-id="7552e-871">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="7552e-871">Support configuring nsg</span></span>
* <span data-ttu-id="7552e-872">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="7552e-872">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="7552e-873">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="7552e-873">Support managed service identities</span></span>
* <span data-ttu-id="7552e-874">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="7552e-874">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="7552e-875">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="7552e-875">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="7552e-876">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-876">May 10, 2017</span></span>

<span data-ttu-id="7552e-877">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="7552e-877">Version 2.0.6</span></span>

* <span data-ttu-id="7552e-878">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="7552e-878">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="7552e-879">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="7552e-879">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="7552e-880">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="7552e-880">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="7552e-881">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="7552e-881">Include Cognitive Services module.</span></span>
* <span data-ttu-id="7552e-882">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="7552e-882">Include Service Fabric module.</span></span>
* <span data-ttu-id="7552e-883">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="7552e-883">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="7552e-884">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="7552e-884">Add support for CDN commands.</span></span>
* <span data-ttu-id="7552e-885">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="7552e-885">Remove Container module.</span></span>
* <span data-ttu-id="7552e-886">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="7552e-886">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="7552e-887">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="7552e-887">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="7552e-888">Core</span><span class="sxs-lookup"><span data-stu-id="7552e-888">Core</span></span>

* <span data-ttu-id="7552e-889">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="7552e-889">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="7552e-890">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="7552e-890">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="7552e-891">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="7552e-891">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="7552e-892">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="7552e-892">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="7552e-893">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="7552e-893">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="7552e-894">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="7552e-894">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="7552e-895">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="7552e-895">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="7552e-896">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="7552e-896">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="7552e-897">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="7552e-897">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="7552e-898">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="7552e-898">core: Improved performance</span></span>
* <span data-ttu-id="7552e-899">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="7552e-899">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="7552e-900">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="7552e-900">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-901">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-901">ACS</span></span>

* <span data-ttu-id="7552e-902">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="7552e-902">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="7552e-903">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="7552e-903">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="7552e-904">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="7552e-904">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="7552e-905">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="7552e-905">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-906">AppService</span><span class="sxs-lookup"><span data-stu-id="7552e-906">AppService</span></span>

* <span data-ttu-id="7552e-907">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="7552e-907">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="7552e-908">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="7552e-908">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="7552e-909">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="7552e-909">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="7552e-910">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="7552e-910">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="7552e-911">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="7552e-911">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="7552e-912">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="7552e-912">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="7552e-913">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="7552e-913">support slot swap with preview</span></span>
* <span data-ttu-id="7552e-914">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="7552e-914">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="7552e-915">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="7552e-915">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="7552e-916">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="7552e-916">CosmosDB</span></span>

* <span data-ttu-id="7552e-917">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="7552e-917">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="7552e-918">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="7552e-918">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="7552e-919">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="7552e-919">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="7552e-920">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="7552e-920">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="7552e-921">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="7552e-921">Data Lake Analytics</span></span>

* <span data-ttu-id="7552e-922">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="7552e-922">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="7552e-923">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="7552e-923">Add support for new catalog item type: package.</span></span> <span data-ttu-id="7552e-924">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="7552e-924">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="7552e-925">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="7552e-925">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="7552e-926">Таблица</span><span class="sxs-lookup"><span data-stu-id="7552e-926">Table</span></span>
  * <span data-ttu-id="7552e-927">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="7552e-927">Table valued function</span></span>
  * <span data-ttu-id="7552e-928">Просмотр</span><span class="sxs-lookup"><span data-stu-id="7552e-928">View</span></span>
  * <span data-ttu-id="7552e-929">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="7552e-929">Table Statistics.</span></span> <span data-ttu-id="7552e-930">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="7552e-930">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="7552e-931">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="7552e-931">Data Lake Store</span></span>

* <span data-ttu-id="7552e-932">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="7552e-932">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="7552e-933">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="7552e-933">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="7552e-934">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="7552e-934">missed help for access show.</span></span> <span data-ttu-id="7552e-935">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="7552e-935">adding it.</span></span> <span data-ttu-id="7552e-936">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="7552e-936">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="7552e-937">Поиск</span><span class="sxs-lookup"><span data-stu-id="7552e-937">Find</span></span>

* <span data-ttu-id="7552e-938">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="7552e-938">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="7552e-939">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="7552e-939">KeyVault</span></span>

* <span data-ttu-id="7552e-940">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="7552e-940">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="7552e-941">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="7552e-941">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="7552e-942">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="7552e-942">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="7552e-943">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="7552e-943">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="7552e-944">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="7552e-944">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="7552e-945">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="7552e-945">Lab</span></span>

* <span data-ttu-id="7552e-946">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="7552e-946">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="7552e-947">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="7552e-947">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="7552e-948">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="7552e-948">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="7552e-949">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="7552e-949">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="7552e-950">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="7552e-950">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="7552e-951">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="7552e-951">Monitor</span></span>

* <span data-ttu-id="7552e-952">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="7552e-952">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="7552e-953">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="7552e-953">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="7552e-954">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-954">Network</span></span>

* <span data-ttu-id="7552e-955">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="7552e-955">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="7552e-956">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-956">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="7552e-957">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="7552e-957">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="7552e-958">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="7552e-958">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="7552e-959">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="7552e-959">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="7552e-960">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="7552e-960">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="7552e-961">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="7552e-961">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="7552e-962">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="7552e-962">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="7552e-963">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="7552e-963">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="7552e-964">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="7552e-964">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="7552e-965">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="7552e-965">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="7552e-966">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-966">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="7552e-967">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="7552e-967">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="7552e-968">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="7552e-968">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="7552e-969">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="7552e-969">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="7552e-970">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="7552e-970">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="7552e-971">Профиль</span><span class="sxs-lookup"><span data-stu-id="7552e-971">Profile</span></span>

* <span data-ttu-id="7552e-972">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="7552e-972">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="7552e-973">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="7552e-973">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="7552e-974">Redis</span><span class="sxs-lookup"><span data-stu-id="7552e-974">Redis</span></span>

* <span data-ttu-id="7552e-975">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="7552e-975">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="7552e-976">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="7552e-976">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="7552e-977">Ресурс</span><span class="sxs-lookup"><span data-stu-id="7552e-977">Resource</span></span>

* <span data-ttu-id="7552e-978">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="7552e-978">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="7552e-979">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="7552e-979">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="7552e-980">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="7552e-980">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="7552e-981">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="7552e-981">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="7552e-982">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="7552e-982">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="7552e-983">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="7552e-983">Add docs for az lock update.</span></span> <span data-ttu-id="7552e-984">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="7552e-984">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="7552e-985">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="7552e-985">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="7552e-986">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="7552e-986">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="7552e-987">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="7552e-987">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="7552e-988">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="7552e-988">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="7552e-989">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="7552e-989">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="7552e-990">Роль</span><span class="sxs-lookup"><span data-stu-id="7552e-990">Role</span></span>

* <span data-ttu-id="7552e-991">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="7552e-991">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="7552e-992">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="7552e-992">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="7552e-993">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="7552e-993">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="7552e-994">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="7552e-994">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="7552e-995">SQL</span><span class="sxs-lookup"><span data-stu-id="7552e-995">SQL</span></span>

* <span data-ttu-id="7552e-996">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="7552e-996">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="7552e-997">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="7552e-997">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="7552e-998">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-998">Storage</span></span>

* <span data-ttu-id="7552e-999">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="7552e-999">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="7552e-1000">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="7552e-1000">Add support for incremental blob copy</span></span>
* <span data-ttu-id="7552e-1001">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="7552e-1001">Add support for large block blob upload</span></span>
* <span data-ttu-id="7552e-1002">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="7552e-1002">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-1003">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-1003">VM</span></span>

* <span data-ttu-id="7552e-1004">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="7552e-1004">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="7552e-1005">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="7552e-1005">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="7552e-1006">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="7552e-1006">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="7552e-1007">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="7552e-1007">az vm/vmss disk</span></span>
  3. <span data-ttu-id="7552e-1008">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="7552e-1008">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="7552e-1009">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="7552e-1009">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="7552e-1010">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1010">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="7552e-1011">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-1011">April 3, 2017</span></span>

<span data-ttu-id="7552e-1012">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="7552e-1012">Version 2.0.2</span></span>

<span data-ttu-id="7552e-1013">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="7552e-1013">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="7552e-1014">Core</span><span class="sxs-lookup"><span data-stu-id="7552e-1014">Core</span></span>

* <span data-ttu-id="7552e-1015">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7552e-1015">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="7552e-1016">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1016">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="7552e-1017">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1017">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="7552e-1018">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1018">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7552e-1019">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1019">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="7552e-1020">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="7552e-1020">Add prompting for missing template parameters.</span></span> <span data-ttu-id="7552e-1021">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1021">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="7552e-1022">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="7552e-1022">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="7552e-1023">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="7552e-1023">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="7552e-1024">ACS</span><span class="sxs-lookup"><span data-stu-id="7552e-1024">ACS</span></span>

* <span data-ttu-id="7552e-1025">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1025">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="7552e-1026">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="7552e-1026">Add support for ssh key password prompting.</span></span> <span data-ttu-id="7552e-1027">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1027">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="7552e-1028">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="7552e-1028">Add support for windows clusters.</span></span> <span data-ttu-id="7552e-1029">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1029">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="7552e-1030">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="7552e-1030">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="7552e-1031">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1031">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="7552e-1032">AppService</span><span class="sxs-lookup"><span data-stu-id="7552e-1032">AppService</span></span>

* <span data-ttu-id="7552e-1033">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1033">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="7552e-1034">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1034">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="7552e-1035">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1035">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="7552e-1036">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1036">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="7552e-1037">DataLake</span><span class="sxs-lookup"><span data-stu-id="7552e-1037">DataLake</span></span>

* <span data-ttu-id="7552e-1038">Первоначальный выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="7552e-1038">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="7552e-1039">Первоначальный выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="7552e-1039">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="7552e-1040">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="7552e-1040">DocuemntDB</span></span>

* <span data-ttu-id="7552e-1041">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1041">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="7552e-1042">ВМ</span><span class="sxs-lookup"><span data-stu-id="7552e-1042">VM</span></span>

* <span data-ttu-id="7552e-1043">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1043">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="7552e-1044">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1044">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="7552e-1045">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1045">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="7552e-1046">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1046">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="7552e-1047">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1047">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="7552e-1048">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1048">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="7552e-1049">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="7552e-1049">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="7552e-1050">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="7552e-1050">February 27, 2017</span></span>

<span data-ttu-id="7552e-1051">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="7552e-1051">Version 2.0.0</span></span>

<span data-ttu-id="7552e-1052">Этот первый общедоступный выпуск Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="7552e-1052">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="7552e-1053">Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="7552e-1053">General availability applies to these command modules:</span></span>
- <span data-ttu-id="7552e-1054">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="7552e-1054">Container Service (acs)</span></span>
- <span data-ttu-id="7552e-1055">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="7552e-1055">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="7552e-1056">Сеть</span><span class="sxs-lookup"><span data-stu-id="7552e-1056">Networking</span></span>
- <span data-ttu-id="7552e-1057">Хранилище</span><span class="sxs-lookup"><span data-stu-id="7552e-1057">Storage</span></span>

<span data-ttu-id="7552e-1058">Эти командные модули могут использоваться в рабочих средах и поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания.</span><span class="sxs-lookup"><span data-stu-id="7552e-1058">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="7552e-1059">Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="7552e-1059">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="7552e-1060">Вы можете задавать вопросы на сайте [StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="7552e-1060">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="7552e-1061">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="7552e-1061">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="7552e-1062">Чтобы проверить версию интерфейса командной строки, используйте `az --version`.</span><span class="sxs-lookup"><span data-stu-id="7552e-1062">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="7552e-1063">В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="7552e-1063">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="7552e-1064">Некоторые командные модули имеют постфикс "b*n*" или "rc*n*".</span><span class="sxs-lookup"><span data-stu-id="7552e-1064">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="7552e-1065">Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="7552e-1065">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="7552e-1066">У нас также есть предварительные ежедневные сборки интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="7552e-1066">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="7552e-1067">Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="7552e-1067">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="7552e-1068">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="7552e-1068">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="7552e-1069">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="7552e-1069">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="7552e-1070">обратившись к специалистам группы разработчиков продукта по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com);</span><span class="sxs-lookup"><span data-stu-id="7552e-1070">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="7552e-1071">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="7552e-1071">Provide feedback from the command line with the `az feedback` command.</span></span>

