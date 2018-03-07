---
title: "Заметки о выпуске Azure CLI 2.0"
description: "Узнайте о последних обновлениях в Azure CLI 2.0"
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 02/27/2018
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.openlocfilehash: 01078b7a3665f563f0a6b1d809c9a41f18d136d6
ms.sourcegitcommit: f3ab5da6019083ef2482b62c7355817e6170dcfb
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/28/2018
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="8d32e-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="8d32e-103">Azure CLI 2.0 release notes</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="8d32e-104">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="8d32e-104">February 27, 2018</span></span>

<span data-ttu-id="8d32e-105">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="8d32e-105">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="8d32e-106">Core</span><span class="sxs-lookup"><span data-stu-id="8d32e-106">Core</span></span>

* <span data-ttu-id="8d32e-107">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="8d32e-107">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="8d32e-108">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="8d32e-108">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="8d32e-109">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-109">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-110">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-110">ACS</span></span>

* <span data-ttu-id="8d32e-111">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8d32e-111">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="8d32e-112">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="8d32e-112">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="8d32e-113">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-113">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="8d32e-114">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-114">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-115">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-115">Appservice</span></span>

* <span data-ttu-id="8d32e-116">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="8d32e-116">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="8d32e-117">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="8d32e-117">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8d32e-118">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="8d32e-118">Cognitive Services</span></span>

* <span data-ttu-id="8d32e-119">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="8d32e-119">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="8d32e-120">Потребление</span><span class="sxs-lookup"><span data-stu-id="8d32e-120">Consumption</span></span>

* <span data-ttu-id="8d32e-121">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="8d32e-121">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="8d32e-122">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="8d32e-122">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="8d32e-123">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8d32e-123">Container</span></span>

* <span data-ttu-id="8d32e-124">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="8d32e-124">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-125">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-125">Network</span></span>

* <span data-ttu-id="8d32e-126">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="8d32e-126">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="8d32e-127">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8d32e-127">Resource</span></span>

* <span data-ttu-id="8d32e-128">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="8d32e-128">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="8d32e-129">Роль</span><span class="sxs-lookup"><span data-stu-id="8d32e-129">Role</span></span>

* <span data-ttu-id="8d32e-130">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="8d32e-130">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="8d32e-131">SQL</span><span class="sxs-lookup"><span data-stu-id="8d32e-131">SQL</span></span>

* <span data-ttu-id="8d32e-132">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-132">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-133">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-133">Storage</span></span>

* <span data-ttu-id="8d32e-134">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-134">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-135">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-135">VM</span></span>

* <span data-ttu-id="8d32e-136">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="8d32e-136">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="8d32e-137">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-137">February 13, 2018</span></span>

<span data-ttu-id="8d32e-138">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="8d32e-138">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="8d32e-139">Core</span><span class="sxs-lookup"><span data-stu-id="8d32e-139">Core</span></span>

* <span data-ttu-id="8d32e-140">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="8d32e-140">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-141">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-141">ACS</span></span>

* <span data-ttu-id="8d32e-142">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="8d32e-142">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="8d32e-143">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-143">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="8d32e-144">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="8d32e-144">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="8d32e-145">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="8d32e-145">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="8d32e-146">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="8d32e-146">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="8d32e-147">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-147">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="8d32e-148">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="8d32e-148">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="8d32e-149">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-149">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-150">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-150">Appservice</span></span>

* <span data-ttu-id="8d32e-151">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="8d32e-151">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="8d32e-152">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-152">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="8d32e-153">CDN</span><span class="sxs-lookup"><span data-stu-id="8d32e-153">CDN</span></span>

* <span data-ttu-id="8d32e-154">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-154">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="8d32e-155">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8d32e-155">Container</span></span>

* <span data-ttu-id="8d32e-156">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="8d32e-156">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="8d32e-157">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8d32e-157">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8d32e-158">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8d32e-158">CosmosDB</span></span>

* <span data-ttu-id="8d32e-159">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="8d32e-159">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="8d32e-160">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="8d32e-160">Extension</span></span>

* <span data-ttu-id="8d32e-161">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-161">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="8d32e-162">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-162">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="8d32e-163">Отзыв</span><span class="sxs-lookup"><span data-stu-id="8d32e-163">Feedback</span></span>

* <span data-ttu-id="8d32e-164">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="8d32e-164">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="8d32e-165">Interactive</span><span class="sxs-lookup"><span data-stu-id="8d32e-165">Interactive</span></span>

* <span data-ttu-id="8d32e-166">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="8d32e-166">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="8d32e-167">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="8d32e-167">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="8d32e-168">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8d32e-168">IoT</span></span>

* <span data-ttu-id="8d32e-169">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="8d32e-169">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="8d32e-170">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="8d32e-170">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success.</span></span>
* <span data-ttu-id="8d32e-171">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-171">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="8d32e-172">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="8d32e-172">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="8d32e-173">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="8d32e-173">Monitor</span></span>

* <span data-ttu-id="8d32e-174">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-174">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-175">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-175">Network</span></span>

* <span data-ttu-id="8d32e-176">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="8d32e-176">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="8d32e-177">Профиль</span><span class="sxs-lookup"><span data-stu-id="8d32e-177">Profile</span></span>

* <span data-ttu-id="8d32e-178">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="8d32e-178">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="8d32e-179">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8d32e-179">Resource</span></span>

* <span data-ttu-id="8d32e-180">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-180">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="8d32e-181">Роль</span><span class="sxs-lookup"><span data-stu-id="8d32e-181">Role</span></span>

* <span data-ttu-id="8d32e-182">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="8d32e-182">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="8d32e-183">SQL</span><span class="sxs-lookup"><span data-stu-id="8d32e-183">SQL</span></span>

* <span data-ttu-id="8d32e-184">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-184">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="8d32e-185">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-185">Added `sql db rename`</span></span>
* <span data-ttu-id="8d32e-186">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="8d32e-186">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-187">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-187">Storage</span></span>

* <span data-ttu-id="8d32e-188">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="8d32e-188">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-189">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-189">VM</span></span>

* <span data-ttu-id="8d32e-190">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="8d32e-190">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="8d32e-191">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="8d32e-191">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="8d32e-192">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="8d32e-192">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="8d32e-193">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-193">January 31, 2018</span></span>

<span data-ttu-id="8d32e-194">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="8d32e-194">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="8d32e-195">Core</span><span class="sxs-lookup"><span data-stu-id="8d32e-195">Core</span></span>

* <span data-ttu-id="8d32e-196">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="8d32e-196">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="8d32e-197">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="8d32e-197">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="8d32e-198">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="8d32e-198">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="8d32e-199">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="8d32e-199">Use `--verbose` to see</span></span>
* <span data-ttu-id="8d32e-200">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="8d32e-200">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-201">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-201">ACS</span></span>

* <span data-ttu-id="8d32e-202">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-202">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="8d32e-203">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-203">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-204">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-204">Appservice</span></span>

* <span data-ttu-id="8d32e-205">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="8d32e-205">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="8d32e-206">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="8d32e-206">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="8d32e-207">CDN</span><span class="sxs-lookup"><span data-stu-id="8d32e-207">CDN</span></span>

* <span data-ttu-id="8d32e-208">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-208">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8d32e-209">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8d32e-209">CosmosDB</span></span>

* <span data-ttu-id="8d32e-210">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="8d32e-210">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="8d32e-211">Interactive</span><span class="sxs-lookup"><span data-stu-id="8d32e-211">Interactive</span></span>

* <span data-ttu-id="8d32e-212">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="8d32e-212">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-213">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-213">Network</span></span>

* <span data-ttu-id="8d32e-214">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-214">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="8d32e-215">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8d32e-215">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="8d32e-216">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-216">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="8d32e-217">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-217">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="8d32e-218">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-218">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="8d32e-219">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="8d32e-219">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="8d32e-220">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="8d32e-220">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="8d32e-221">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="8d32e-221">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="8d32e-222">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-222">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="8d32e-223">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-223">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="8d32e-224">Профиль</span><span class="sxs-lookup"><span data-stu-id="8d32e-224">Profile</span></span>

* <span data-ttu-id="8d32e-225">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="8d32e-225">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="8d32e-226">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8d32e-226">Resource</span></span>

* <span data-ttu-id="8d32e-227">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="8d32e-227">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-228">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-228">Storage</span></span>

* <span data-ttu-id="8d32e-229">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="8d32e-229">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="8d32e-230">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="8d32e-230">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="8d32e-231">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-231">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="8d32e-232">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-232">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="8d32e-233">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="8d32e-233">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-234">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-234">VM</span></span>

* <span data-ttu-id="8d32e-235">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="8d32e-235">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="8d32e-236">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-236">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="8d32e-237">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="8d32e-237">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="8d32e-238">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-238">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="8d32e-239">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-239">January 17, 2018</span></span>

<span data-ttu-id="8d32e-240">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="8d32e-240">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="8d32e-241">ACR</span><span class="sxs-lookup"><span data-stu-id="8d32e-241">ACR</span></span>

* <span data-ttu-id="8d32e-242">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="8d32e-242">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="8d32e-243">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="8d32e-243">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-244">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-244">ACS</span></span>

* <span data-ttu-id="8d32e-245">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-245">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="8d32e-246">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="8d32e-246">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-247">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-247">Appservice</span></span>

* <span data-ttu-id="8d32e-248">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="8d32e-248">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="8d32e-249">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-249">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="8d32e-250">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-250">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="8d32e-251">Архивация</span><span class="sxs-lookup"><span data-stu-id="8d32e-251">Backup</span></span>

* <span data-ttu-id="8d32e-252">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="8d32e-252">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="8d32e-253">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="8d32e-253">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="8d32e-254">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="8d32e-254">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="8d32e-255">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="8d32e-255">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="8d32e-256">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="8d32e-256">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="8d32e-257">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="8d32e-257">Batch</span></span>

* <span data-ttu-id="8d32e-258">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="8d32e-258">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="8d32e-259">Облако</span><span class="sxs-lookup"><span data-stu-id="8d32e-259">Cloud</span></span>

* <span data-ttu-id="8d32e-260">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="8d32e-260">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="8d32e-261">Потребление</span><span class="sxs-lookup"><span data-stu-id="8d32e-261">Consumption</span></span>

* <span data-ttu-id="8d32e-262">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-262">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="8d32e-263">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="8d32e-263">Event Grid</span></span>

* <span data-ttu-id="8d32e-264">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-264">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="8d32e-265">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-265">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="8d32e-266">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-266">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="8d32e-267">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-267">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="8d32e-268">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-268">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="8d32e-269">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-269">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="8d32e-270">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-270">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="8d32e-271">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-271">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="8d32e-272">Interactive</span><span class="sxs-lookup"><span data-stu-id="8d32e-272">Interactive</span></span>

* <span data-ttu-id="8d32e-273">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="8d32e-273">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="8d32e-274">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="8d32e-274">Fixed errors on startup</span></span>
* <span data-ttu-id="8d32e-275">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="8d32e-275">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="8d32e-276">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8d32e-276">IoT</span></span>

* <span data-ttu-id="8d32e-277">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="8d32e-277">Added support for device provisioning service</span></span>
* <span data-ttu-id="8d32e-278">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="8d32e-278">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="8d32e-279">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="8d32e-279">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="8d32e-280">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="8d32e-280">Monitor</span></span>

* <span data-ttu-id="8d32e-281">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="8d32e-281">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="8d32e-282">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-282">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="8d32e-283">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="8d32e-283">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-284">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-284">Network</span></span>

* <span data-ttu-id="8d32e-285">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="8d32e-285">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="8d32e-286">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="8d32e-286">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="8d32e-287">Профиль</span><span class="sxs-lookup"><span data-stu-id="8d32e-287">Profile</span></span>

* <span data-ttu-id="8d32e-288">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="8d32e-288">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="8d32e-289">Роль</span><span class="sxs-lookup"><span data-stu-id="8d32e-289">Role</span></span>

* <span data-ttu-id="8d32e-290">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-290">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8d32e-291">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8d32e-291">Service Fabric</span></span>

* <span data-ttu-id="8d32e-292">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="8d32e-292">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="8d32e-293">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="8d32e-293">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-294">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-294">VM</span></span>

* <span data-ttu-id="8d32e-295">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-295">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="8d32e-296">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Значение по умолчанию `vmss` для одной зоны заменено на данные подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="8d32e-296">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="8d32e-297">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-297">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="8d32e-298">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="8d32e-298">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="8d32e-299">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="8d32e-299">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="8d32e-300">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-300">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="8d32e-301">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-301">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="8d32e-302">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-302">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="8d32e-303">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-303">December 19, 2017</span></span>

<span data-ttu-id="8d32e-304">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="8d32e-304">Version 2.0.23</span></span>

* <span data-ttu-id="8d32e-305">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="8d32e-305">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="8d32e-306">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8d32e-306">Container</span></span>

* <span data-ttu-id="8d32e-307">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8d32e-307">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-308">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-308">Network</span></span>

* <span data-ttu-id="8d32e-309">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8d32e-309">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="8d32e-310">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8d32e-310">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-311">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-311">Storage</span></span>

* <span data-ttu-id="8d32e-312">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="8d32e-312">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-313">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-313">VM</span></span>

* <span data-ttu-id="8d32e-314">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="8d32e-314">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="8d32e-315">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-315">December 5, 2017</span></span>

<span data-ttu-id="8d32e-316">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="8d32e-316">Version 2.0.22</span></span>

* <span data-ttu-id="8d32e-317">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-317">Removed `az component` commands.</span></span> <span data-ttu-id="8d32e-318">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-318">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="8d32e-319">Core</span><span class="sxs-lookup"><span data-stu-id="8d32e-319">Core</span></span>
* <span data-ttu-id="8d32e-320">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="8d32e-320">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="8d32e-321">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="8d32e-321">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-322">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-322">ACS</span></span>

* <span data-ttu-id="8d32e-323">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-323">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="8d32e-324">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-324">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="8d32e-325">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="8d32e-325">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="8d32e-326">Помощник</span><span class="sxs-lookup"><span data-stu-id="8d32e-326">Advisor</span></span>

* <span data-ttu-id="8d32e-327">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="8d32e-327">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-328">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-328">Appservice</span></span>

* <span data-ttu-id="8d32e-329">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-329">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="8d32e-330">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="8d32e-330">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="8d32e-331">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-331">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="8d32e-332">Потребление</span><span class="sxs-lookup"><span data-stu-id="8d32e-332">Consumption</span></span>

* <span data-ttu-id="8d32e-333">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="8d32e-333">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="8d32e-334">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8d32e-334">Container</span></span>

* <span data-ttu-id="8d32e-335">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="8d32e-335">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="8d32e-336">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="8d32e-336">Monitor</span></span>

* <span data-ttu-id="8d32e-337">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="8d32e-337">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="8d32e-338">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8d32e-338">Resource</span></span>

* <span data-ttu-id="8d32e-339">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="8d32e-339">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="8d32e-340">Роль</span><span class="sxs-lookup"><span data-stu-id="8d32e-340">Role</span></span>

* <span data-ttu-id="8d32e-341">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-341">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="8d32e-342">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="8d32e-342">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="8d32e-343">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-343">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="8d32e-344">SQL</span><span class="sxs-lookup"><span data-stu-id="8d32e-344">SQL</span></span>

* <span data-ttu-id="8d32e-345">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-345">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="8d32e-346">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-346">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-347">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-347">VM</span></span>

* <span data-ttu-id="8d32e-348">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-348">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="8d32e-349">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-349">November 14, 2017</span></span>

<span data-ttu-id="8d32e-350">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="8d32e-350">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="8d32e-351">ACR</span><span class="sxs-lookup"><span data-stu-id="8d32e-351">ACR</span></span>

* <span data-ttu-id="8d32e-352">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="8d32e-352">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="8d32e-353">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-353">ACS</span></span>

* <span data-ttu-id="8d32e-354">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="8d32e-354">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="8d32e-355">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="8d32e-355">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="8d32e-356">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-356">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="8d32e-357">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="8d32e-357">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="8d32e-358">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="8d32e-358">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-359">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-359">Appservice</span></span>

* <span data-ttu-id="8d32e-360">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="8d32e-360">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="8d32e-361">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-361">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="8d32e-362">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-362">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="8d32e-363">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-363">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="8d32e-364">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="8d32e-364">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="8d32e-365">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="8d32e-365">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="8d32e-366">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="8d32e-366">Batch</span></span>

* <span data-ttu-id="8d32e-367">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-367">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="8d32e-368">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="8d32e-368">Batchai</span></span>

* <span data-ttu-id="8d32e-369">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-369">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="8d32e-370">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-370">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="8d32e-371">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-371">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="8d32e-372">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-372">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="8d32e-373">Облако</span><span class="sxs-lookup"><span data-stu-id="8d32e-373">Cloud</span></span>

* <span data-ttu-id="8d32e-374">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="8d32e-374">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="8d32e-375">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8d32e-375">Container</span></span>

* <span data-ttu-id="8d32e-376">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-376">Added support to open multiple ports</span></span>
* <span data-ttu-id="8d32e-377">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8d32e-377">Added container group restart policy</span></span>
* <span data-ttu-id="8d32e-378">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="8d32e-378">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="8d32e-379">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="8d32e-379">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8d32e-380">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8d32e-380">Data Lake Analytics</span></span>

* <span data-ttu-id="8d32e-381">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="8d32e-381">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8d32e-382">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8d32e-382">Data Lake Store</span></span>

* <span data-ttu-id="8d32e-383">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="8d32e-383">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="8d32e-384">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="8d32e-384">Extension</span></span>

* <span data-ttu-id="8d32e-385">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="8d32e-385">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="8d32e-386">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="8d32e-386">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="8d32e-387">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8d32e-387">IoT</span></span>

* <span data-ttu-id="8d32e-388">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-388">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="8d32e-389">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="8d32e-389">Monitor</span></span>

* <span data-ttu-id="8d32e-390">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-390">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-391">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-391">Network</span></span>

* <span data-ttu-id="8d32e-392">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="8d32e-392">Added support for CAA DNS records</span></span>
* <span data-ttu-id="8d32e-393">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-393">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="8d32e-394">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="8d32e-394">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="8d32e-395">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-395">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="8d32e-396">Резервирование</span><span class="sxs-lookup"><span data-stu-id="8d32e-396">Reservations</span></span>

* <span data-ttu-id="8d32e-397">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="8d32e-397">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="8d32e-398">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8d32e-398">Resource</span></span>

* <span data-ttu-id="8d32e-399">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-399">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="8d32e-400">SQL</span><span class="sxs-lookup"><span data-stu-id="8d32e-400">SQL</span></span>

* <span data-ttu-id="8d32e-401">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-401">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-402">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-402">Storage</span></span>

* <span data-ttu-id="8d32e-403">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8d32e-403">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="8d32e-404">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="8d32e-404">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="8d32e-405">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-405">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="8d32e-406">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-406">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="8d32e-407">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-407">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="8d32e-408">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-408">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="8d32e-409">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-409">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-410">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-410">VM</span></span>

* <span data-ttu-id="8d32e-411">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-411">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="8d32e-412">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-412">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="8d32e-413">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-413">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="8d32e-414">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-414">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="8d32e-415">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="8d32e-415">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="8d32e-416">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-416">October 24, 2017</span></span>

<span data-ttu-id="8d32e-417">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="8d32e-417">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="8d32e-418">Core</span><span class="sxs-lookup"><span data-stu-id="8d32e-418">Core</span></span>

* <span data-ttu-id="8d32e-419">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="8d32e-419">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="8d32e-420">ACR</span><span class="sxs-lookup"><span data-stu-id="8d32e-420">ACR</span></span>

* <span data-ttu-id="8d32e-421">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="8d32e-421">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="8d32e-422">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="8d32e-422">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="8d32e-423">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="8d32e-423">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-424">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-424">ACS</span></span>

* <span data-ttu-id="8d32e-425">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="8d32e-425">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="8d32e-426">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="8d32e-426">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-427">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-427">Appservice</span></span>

* <span data-ttu-id="8d32e-428">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="8d32e-428">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="8d32e-429">Компонент</span><span class="sxs-lookup"><span data-stu-id="8d32e-429">Component</span></span>

* <span data-ttu-id="8d32e-430">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="8d32e-430">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="8d32e-431">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="8d32e-431">Monitor</span></span>

* <span data-ttu-id="8d32e-432">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-432">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="8d32e-433">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8d32e-433">Resource</span></span>

* <span data-ttu-id="8d32e-434">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="8d32e-434">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="8d32e-435">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="8d32e-435">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-436">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-436">VM</span></span>

* <span data-ttu-id="8d32e-437">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="8d32e-437">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="8d32e-438">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-438">October 9, 2017</span></span>

<span data-ttu-id="8d32e-439">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="8d32e-439">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="8d32e-440">Core</span><span class="sxs-lookup"><span data-stu-id="8d32e-440">Core</span></span>

* <span data-ttu-id="8d32e-441">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="8d32e-441">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-442">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-442">Appservice</span></span>

* <span data-ttu-id="8d32e-443">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-443">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="8d32e-444">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="8d32e-444">Batch</span></span>

* <span data-ttu-id="8d32e-445">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="8d32e-445">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="8d32e-446">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="8d32e-446">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="8d32e-447">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="8d32e-447">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="8d32e-448">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-448">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="8d32e-449">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="8d32e-449">Batchai</span></span>

* <span data-ttu-id="8d32e-450">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="8d32e-450">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="8d32e-451">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8d32e-451">Keyvault</span></span>

* <span data-ttu-id="8d32e-452">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8d32e-452">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="8d32e-453">(#4448)</span><span class="sxs-lookup"><span data-stu-id="8d32e-453">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="8d32e-454">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-454">Network</span></span>

* <span data-ttu-id="8d32e-455">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="8d32e-455">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="8d32e-456">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="8d32e-456">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="8d32e-457">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8d32e-457">Resource</span></span>

* <span data-ttu-id="8d32e-458">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-458">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="8d32e-459">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="8d32e-459">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="8d32e-460">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="8d32e-460">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="8d32e-461">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="8d32e-461">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="8d32e-462">SQL</span><span class="sxs-lookup"><span data-stu-id="8d32e-462">Sql</span></span>

* <span data-ttu-id="8d32e-463">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="8d32e-463">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="8d32e-464">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="8d32e-464">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="8d32e-465">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="8d32e-465">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-466">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-466">Storage</span></span>

* <span data-ttu-id="8d32e-467">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-467">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-468">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="8d32e-468">Vm</span></span>

* <span data-ttu-id="8d32e-469">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-469">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="8d32e-470">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-470">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="8d32e-471">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-471">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="8d32e-472">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-472">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="8d32e-473">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="8d32e-473">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="8d32e-474">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-474">September 22, 2017</span></span>

<span data-ttu-id="8d32e-475">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="8d32e-475">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="8d32e-476">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8d32e-476">Resource</span></span>

* <span data-ttu-id="8d32e-477">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="8d32e-477">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="8d32e-478">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="8d32e-478">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="8d32e-479">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="8d32e-479">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="8d32e-480">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="8d32e-480">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-481">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-481">Network</span></span>

* <span data-ttu-id="8d32e-482">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="8d32e-482">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="8d32e-483">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="8d32e-483">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="8d32e-484">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="8d32e-484">Added `asg` application security group commands</span></span>
* <span data-ttu-id="8d32e-485">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="8d32e-485">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="8d32e-486">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8d32e-486">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="8d32e-487">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8d32e-487">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="8d32e-488">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-488">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-489">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-489">Storage</span></span>

* <span data-ttu-id="8d32e-490">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="8d32e-490">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="8d32e-491">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="8d32e-491">Eventgrid</span></span>

* <span data-ttu-id="8d32e-492">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="8d32e-492">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="8d32e-493">SQL</span><span class="sxs-lookup"><span data-stu-id="8d32e-493">SQL</span></span>

* <span data-ttu-id="8d32e-494">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="8d32e-494">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="8d32e-495">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="8d32e-495">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="8d32e-496">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8d32e-496">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="8d32e-497">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8d32e-497">Keyvault</span></span>

* <span data-ttu-id="8d32e-498">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="8d32e-498">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-499">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-499">VM</span></span>

* <span data-ttu-id="8d32e-500">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="8d32e-500">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="8d32e-501">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="8d32e-501">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="8d32e-502">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="8d32e-502">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="8d32e-503">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="8d32e-503">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="8d32e-504">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="8d32e-504">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="8d32e-505">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="8d32e-505">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-506">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-506">ACS</span></span>

* <span data-ttu-id="8d32e-507">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="8d32e-507">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-508">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-508">Appservice</span></span>

* <span data-ttu-id="8d32e-509">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="8d32e-509">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="8d32e-510">Архивация</span><span class="sxs-lookup"><span data-stu-id="8d32e-510">Backup</span></span>

* <span data-ttu-id="8d32e-511">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="8d32e-511">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="8d32e-512">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-512">September 11, 2017</span></span>

<span data-ttu-id="8d32e-513">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="8d32e-513">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="8d32e-514">Core</span><span class="sxs-lookup"><span data-stu-id="8d32e-514">Core</span></span>

* <span data-ttu-id="8d32e-515">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="8d32e-515">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="8d32e-516">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="8d32e-516">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-517">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-517">Acs</span></span>

* <span data-ttu-id="8d32e-518">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-518">Added `acs list-locations` command</span></span>
* <span data-ttu-id="8d32e-519">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8d32e-519">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-520">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-520">Appservice</span></span>

* <span data-ttu-id="8d32e-521">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="8d32e-521">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="8d32e-522">CDN</span><span class="sxs-lookup"><span data-stu-id="8d32e-522">CDN</span></span>

* <span data-ttu-id="8d32e-523">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-523">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="8d32e-524">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="8d32e-524">Extension</span></span>

* <span data-ttu-id="8d32e-525">Первый выпуск.</span><span class="sxs-lookup"><span data-stu-id="8d32e-525">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="8d32e-526">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8d32e-526">Keyvault</span></span>

* <span data-ttu-id="8d32e-527">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-527">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-528">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-528">Network</span></span>

* <span data-ttu-id="8d32e-529">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-529">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="8d32e-530">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-530">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="8d32e-531">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-531">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="8d32e-532">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-532">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="8d32e-533">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-533">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="8d32e-534">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8d32e-534">Resource</span></span>

* <span data-ttu-id="8d32e-535">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-535">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="8d32e-536">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-536">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="8d32e-537">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="8d32e-537">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="8d32e-538">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="8d32e-538">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="8d32e-539">SQL</span><span class="sxs-lookup"><span data-stu-id="8d32e-539">SQL</span></span>

* <span data-ttu-id="8d32e-540">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-540">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-541">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-541">VM</span></span>

* <span data-ttu-id="8d32e-542">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="8d32e-542">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="8d32e-543">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="8d32e-543">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="8d32e-544">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-544">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="8d32e-545">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="8d32e-545">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="8d32e-546">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="8d32e-546">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="8d32e-547">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-547">August 31, 2017</span></span>

<span data-ttu-id="8d32e-548">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="8d32e-548">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="8d32e-549">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8d32e-549">Keyvault</span></span>

* <span data-ttu-id="8d32e-550">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-550">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="8d32e-551">Sf</span><span class="sxs-lookup"><span data-stu-id="8d32e-551">Sf</span></span>

* <span data-ttu-id="8d32e-552">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="8d32e-552">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-553">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-553">Storage</span></span>

* <span data-ttu-id="8d32e-554">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="8d32e-554">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="8d32e-555">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="8d32e-555">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="8d32e-556">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-556">August 28, 2017</span></span>

<span data-ttu-id="8d32e-557">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="8d32e-557">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="8d32e-558">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="8d32e-558">CLI</span></span>

* <span data-ttu-id="8d32e-559">К параметру `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="8d32e-559">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-560">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-560">ACS</span></span>

* <span data-ttu-id="8d32e-561">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="8d32e-561">Corrected preview regions.</span></span>
* <span data-ttu-id="8d32e-562">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-562">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="8d32e-563">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="8d32e-563">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-564">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-564">Appservice</span></span>

* <span data-ttu-id="8d32e-565">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-565">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="8d32e-566">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-566">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="8d32e-567">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-567">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="8d32e-568">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="8d32e-568">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="8d32e-569">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="8d32e-569">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="8d32e-570">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8d32e-570">IoT</span></span>

* <span data-ttu-id="8d32e-571">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="8d32e-571">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-572">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-572">Network</span></span>

* <span data-ttu-id="8d32e-573">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-573">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="8d32e-574">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-574">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="8d32e-575">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-575">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="8d32e-576">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-576">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="8d32e-577">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-577">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="8d32e-578">Профиль</span><span class="sxs-lookup"><span data-stu-id="8d32e-578">Profile</span></span>

* <span data-ttu-id="8d32e-579">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="8d32e-579">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8d32e-580">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8d32e-580">Service Fabric</span></span>

* <span data-ttu-id="8d32e-581">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="8d32e-581">Preview release</span></span>
* <span data-ttu-id="8d32e-582">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="8d32e-582">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="8d32e-583">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="8d32e-583">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="8d32e-584">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-584">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-585">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-585">Storage</span></span>

* <span data-ttu-id="8d32e-586">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="8d32e-586">Enabled setting blob tier</span></span>
* <span data-ttu-id="8d32e-587">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="8d32e-587">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="8d32e-588">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-588">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="8d32e-589">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="8d32e-589">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="8d32e-590">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-590">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="8d32e-591">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-591">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-592">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-592">VM</span></span>

* <span data-ttu-id="8d32e-593">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-593">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="8d32e-594">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-594">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="8d32e-595">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="8d32e-595">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="8d32e-596">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="8d32e-596">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="8d32e-597">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="8d32e-597">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="8d32e-598">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-598">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="8d32e-599">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-599">August 15, 2017</span></span>

<span data-ttu-id="8d32e-600">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="8d32e-600">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-601">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-601">ACS</span></span>

* <span data-ttu-id="8d32e-602">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="8d32e-602">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-603">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-603">Appservice</span></span>

* <span data-ttu-id="8d32e-604">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="8d32e-604">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="8d32e-605">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="8d32e-605">Event Grid</span></span>

* <span data-ttu-id="8d32e-606">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="8d32e-606">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="8d32e-607">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-607">August 11, 2017</span></span>

<span data-ttu-id="8d32e-608">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="8d32e-608">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-609">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-609">ACS</span></span>

* <span data-ttu-id="8d32e-610">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="8d32e-610">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="8d32e-611">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="8d32e-611">Batch</span></span>

* <span data-ttu-id="8d32e-612">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="8d32e-612">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="8d32e-613">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="8d32e-613">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="8d32e-614">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-614">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="8d32e-615">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="8d32e-615">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="8d32e-616">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="8d32e-616">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="8d32e-617">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="8d32e-617">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="8d32e-618">Компонент</span><span class="sxs-lookup"><span data-stu-id="8d32e-618">Component</span></span>

* <span data-ttu-id="8d32e-619">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="8d32e-619">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="8d32e-620">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8d32e-620">Container</span></span>

* <span data-ttu-id="8d32e-621">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="8d32e-621">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="8d32e-622">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8d32e-622">Data Lake Store</span></span>

* <span data-ttu-id="8d32e-623">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="8d32e-623">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="8d32e-624">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="8d32e-624">Event Grid</span></span>

* <span data-ttu-id="8d32e-625">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="8d32e-625">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-626">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-626">Network</span></span>

* <span data-ttu-id="8d32e-627">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="8d32e-627">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="8d32e-628">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-628">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="8d32e-629">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-629">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="8d32e-630">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-630">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="8d32e-631">Профиль</span><span class="sxs-lookup"><span data-stu-id="8d32e-631">Profile</span></span>

* <span data-ttu-id="8d32e-632">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="8d32e-632">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-633">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-633">Storage</span></span>

* <span data-ttu-id="8d32e-634">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="8d32e-634">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-635">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-635">VM</span></span>

* <span data-ttu-id="8d32e-636">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="8d32e-636">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="8d32e-637">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-637">Exposed `list-skus` command</span></span>
* <span data-ttu-id="8d32e-638">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="8d32e-638">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="8d32e-639">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="8d32e-639">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="8d32e-640">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="8d32e-640">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="8d32e-641">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-641">July 28, 2017</span></span>

<span data-ttu-id="8d32e-642">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="8d32e-642">Version 2.0.12</span></span>

* <span data-ttu-id="8d32e-643">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8d32e-643">Added container commands</span></span>
* <span data-ttu-id="8d32e-644">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-644">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="8d32e-645">Core</span><span class="sxs-lookup"><span data-stu-id="8d32e-645">Core</span></span>

* <span data-ttu-id="8d32e-646">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-646">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="8d32e-647">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="8d32e-647">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="8d32e-648">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="8d32e-648">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="8d32e-649">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="8d32e-649">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="8d32e-650">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="8d32e-650">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="8d32e-651">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="8d32e-651">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="8d32e-652">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="8d32e-652">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="8d32e-653">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="8d32e-653">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="8d32e-654">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="8d32e-654">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="8d32e-655">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="8d32e-655">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="8d32e-656">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="8d32e-656">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="8d32e-657">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="8d32e-657">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="8d32e-658">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="8d32e-658">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="8d32e-659">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="8d32e-659">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="8d32e-660">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8d32e-660">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="8d32e-661">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="8d32e-661">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="8d32e-662">ACR</span><span class="sxs-lookup"><span data-stu-id="8d32e-662">ACR</span></span>

* <span data-ttu-id="8d32e-663">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="8d32e-663">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="8d32e-664">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="8d32e-664">Support SKU update for managed registries</span></span>
* <span data-ttu-id="8d32e-665">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="8d32e-665">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="8d32e-666">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="8d32e-666">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="8d32e-667">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="8d32e-667">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="8d32e-668">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="8d32e-668">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-669">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-669">ACS</span></span>

* <span data-ttu-id="8d32e-670">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="8d32e-670">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-671">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8d32e-671">Appservice</span></span>

* <span data-ttu-id="8d32e-672">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="8d32e-672">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="8d32e-673">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="8d32e-673">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="8d32e-674">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-674">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="8d32e-675">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="8d32e-675">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="8d32e-676">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="8d32e-676">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="8d32e-677">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="8d32e-677">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="8d32e-678">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="8d32e-678">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="8d32e-679">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="8d32e-679">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="8d32e-680">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="8d32e-680">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="8d32e-681">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-681">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="8d32e-682">пакетная служба;</span><span class="sxs-lookup"><span data-stu-id="8d32e-682">Batch</span></span>

* <span data-ttu-id="8d32e-683">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="8d32e-683">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="8d32e-684">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-684">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="8d32e-685">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-685">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="8d32e-686">CDN</span><span class="sxs-lookup"><span data-stu-id="8d32e-686">CDN</span></span>

* <span data-ttu-id="8d32e-687">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="8d32e-687">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="8d32e-688">Облако</span><span class="sxs-lookup"><span data-stu-id="8d32e-688">Cloud</span></span>

* <span data-ttu-id="8d32e-689">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="8d32e-689">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="8d32e-690">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="8d32e-690">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="8d32e-691">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="8d32e-691">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="8d32e-692">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="8d32e-692">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="8d32e-693">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-693">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8d32e-694">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8d32e-694">CosmosDB</span></span>

* <span data-ttu-id="8d32e-695">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="8d32e-695">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="8d32e-696">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="8d32e-696">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8d32e-697">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8d32e-697">Data Lake Analytics</span></span>

* <span data-ttu-id="8d32e-698">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-698">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="8d32e-699">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-699">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="8d32e-700">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-700">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8d32e-701">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8d32e-701">Data Lake Store</span></span>

* <span data-ttu-id="8d32e-702">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-702">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="8d32e-703">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="8d32e-703">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="8d32e-704">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-704">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="8d32e-705">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="8d32e-705">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="8d32e-706">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="8d32e-706">Interactive</span></span>

* <span data-ttu-id="8d32e-707">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="8d32e-707">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="8d32e-708">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="8d32e-708">Increased test coverage</span></span>
* <span data-ttu-id="8d32e-709">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="8d32e-709">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="8d32e-710">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="8d32e-710">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="8d32e-711">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="8d32e-711">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="8d32e-712">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="8d32e-712">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="8d32e-713">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="8d32e-713">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="8d32e-714">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-714">Added `--progress` flag</span></span>
* <span data-ttu-id="8d32e-715">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-715">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="8d32e-716">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="8d32e-716">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="8d32e-717">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8d32e-717">IoT</span></span>

* <span data-ttu-id="8d32e-718">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="8d32e-718">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="8d32e-719">(3934).</span><span class="sxs-lookup"><span data-stu-id="8d32e-719">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="8d32e-720">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8d32e-720">Key vault</span></span>

* <span data-ttu-id="8d32e-721">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="8d32e-721">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="8d32e-722">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-722">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="8d32e-723">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="8d32e-723">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="8d32e-724">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="8d32e-724">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="8d32e-725">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-725">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="8d32e-726">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="8d32e-726">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="8d32e-727">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="8d32e-727">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="8d32e-728">(3307).</span><span class="sxs-lookup"><span data-stu-id="8d32e-728">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="8d32e-729">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="8d32e-729">Lab</span></span>

* <span data-ttu-id="8d32e-730">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-730">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="8d32e-731">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-731">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="8d32e-732">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="8d32e-732">Monitor</span></span>

* <span data-ttu-id="8d32e-733">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="8d32e-733">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="8d32e-734">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-734">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="8d32e-735">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-735">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="8d32e-736">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-736">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="8d32e-737">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-737">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="8d32e-738">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="8d32e-738">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="8d32e-739">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="8d32e-739">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="8d32e-740">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="8d32e-740">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="8d32e-741">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="8d32e-741">`location` no longer required</span></span>
  * <span data-ttu-id="8d32e-742">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="8d32e-742">Add name and ID support for target</span></span>
  * <span data-ttu-id="8d32e-743">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="8d32e-743">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="8d32e-744">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="8d32e-744">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="8d32e-745">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="8d32e-745">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="8d32e-746">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="8d32e-746">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="8d32e-747">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-747">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="8d32e-748">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-748">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-749">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-749">Network</span></span>

* <span data-ttu-id="8d32e-750">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-750">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="8d32e-751">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-751">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="8d32e-752">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="8d32e-752">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="8d32e-753">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-753">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="8d32e-754">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-754">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="8d32e-755">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-755">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="8d32e-756">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-756">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="8d32e-757">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-757">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="8d32e-758">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-758">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="8d32e-759">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-759">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="8d32e-760">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-760">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="8d32e-761">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-761">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="8d32e-762">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-762">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="8d32e-763">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-763">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="8d32e-764">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-764">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="8d32e-765">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-765">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="8d32e-766">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="8d32e-766">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="8d32e-767">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-767">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="8d32e-768">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-768">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="8d32e-769">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-769">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="8d32e-770">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-770">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="8d32e-771">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-771">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="8d32e-772">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-772">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="8d32e-773">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="8d32e-773">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="8d32e-774">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="8d32e-774">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="8d32e-775">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="8d32e-775">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="8d32e-776">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="8d32e-776">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="8d32e-777">Профиль</span><span class="sxs-lookup"><span data-stu-id="8d32e-777">Profile</span></span>

* <span data-ttu-id="8d32e-778">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="8d32e-778">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="8d32e-779">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="8d32e-779">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="8d32e-780">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="8d32e-780">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="8d32e-781">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="8d32e-781">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="8d32e-782">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="8d32e-782">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="8d32e-783">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="8d32e-783">RDBMS</span></span>

* <span data-ttu-id="8d32e-784">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="8d32e-784">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="8d32e-785">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="8d32e-785">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="8d32e-786">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="8d32e-786">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="8d32e-787">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="8d32e-787">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="8d32e-788">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8d32e-788">Resource</span></span>

* <span data-ttu-id="8d32e-789">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-789">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="8d32e-790">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-790">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="8d32e-791">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-791">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="8d32e-792">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-792">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="8d32e-793">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="8d32e-793">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="8d32e-794">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-794">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="8d32e-795">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="8d32e-795">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="8d32e-796">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-796">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="8d32e-797">Роль</span><span class="sxs-lookup"><span data-stu-id="8d32e-797">Role</span></span>

* <span data-ttu-id="8d32e-798">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="8d32e-798">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="8d32e-799">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="8d32e-799">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="8d32e-800">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="8d32e-800">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="8d32e-801">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="8d32e-801">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="8d32e-802">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-802">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8d32e-803">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8d32e-803">Service Fabric</span></span>
* <span data-ttu-id="8d32e-804">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="8d32e-804">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="8d32e-805">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="8d32e-805">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="8d32e-806">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="8d32e-806">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="8d32e-807">SQL</span><span class="sxs-lookup"><span data-stu-id="8d32e-807">SQL</span></span>

* <span data-ttu-id="8d32e-808">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-808">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="8d32e-809">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-809">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="8d32e-810">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-810">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-811">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-811">Storage</span></span>

* <span data-ttu-id="8d32e-812">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="8d32e-812">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="8d32e-813">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="8d32e-813">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="8d32e-814">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="8d32e-814">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="8d32e-815">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="8d32e-815">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="8d32e-816">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="8d32e-816">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="8d32e-817">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="8d32e-817">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-818">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-818">VM</span></span>

* <span data-ttu-id="8d32e-819">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="8d32e-819">Support configuring nsg</span></span>
* <span data-ttu-id="8d32e-820">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="8d32e-820">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="8d32e-821">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="8d32e-821">Support managed service identities</span></span>
* <span data-ttu-id="8d32e-822">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-822">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="8d32e-823">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="8d32e-823">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="8d32e-824">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-824">May 10, 2017</span></span>

<span data-ttu-id="8d32e-825">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="8d32e-825">Version 2.0.6</span></span>

* <span data-ttu-id="8d32e-826">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="8d32e-826">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="8d32e-827">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="8d32e-827">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="8d32e-828">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="8d32e-828">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="8d32e-829">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="8d32e-829">Include Cognitive Services module.</span></span>
* <span data-ttu-id="8d32e-830">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="8d32e-830">Include Service Fabric module.</span></span>
* <span data-ttu-id="8d32e-831">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="8d32e-831">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="8d32e-832">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="8d32e-832">Add support for CDN commands.</span></span>
* <span data-ttu-id="8d32e-833">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="8d32e-833">Remove Container module.</span></span>
* <span data-ttu-id="8d32e-834">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-834">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="8d32e-835">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-835">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="8d32e-836">Core</span><span class="sxs-lookup"><span data-stu-id="8d32e-836">Core</span></span>

* <span data-ttu-id="8d32e-837">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="8d32e-837">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="8d32e-838">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-838">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="8d32e-839">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-839">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="8d32e-840">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-840">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="8d32e-841">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-841">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="8d32e-842">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-842">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="8d32e-843">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-843">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="8d32e-844">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-844">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="8d32e-845">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-845">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="8d32e-846">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="8d32e-846">core: Improved performance</span></span>
* <span data-ttu-id="8d32e-847">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="8d32e-847">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="8d32e-848">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="8d32e-848">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-849">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-849">ACS</span></span>

* <span data-ttu-id="8d32e-850">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="8d32e-850">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="8d32e-851">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="8d32e-851">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="8d32e-852">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="8d32e-852">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="8d32e-853">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-853">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-854">AppService</span><span class="sxs-lookup"><span data-stu-id="8d32e-854">AppService</span></span>

* <span data-ttu-id="8d32e-855">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="8d32e-855">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="8d32e-856">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="8d32e-856">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="8d32e-857">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="8d32e-857">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="8d32e-858">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="8d32e-858">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="8d32e-859">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="8d32e-859">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="8d32e-860">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-860">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="8d32e-861">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="8d32e-861">support slot swap with preview</span></span>
* <span data-ttu-id="8d32e-862">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-862">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="8d32e-863">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-863">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8d32e-864">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8d32e-864">CosmosDB</span></span>

* <span data-ttu-id="8d32e-865">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="8d32e-865">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="8d32e-866">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="8d32e-866">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="8d32e-867">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="8d32e-867">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="8d32e-868">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="8d32e-868">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8d32e-869">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8d32e-869">Data Lake Analytics</span></span>

* <span data-ttu-id="8d32e-870">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="8d32e-870">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="8d32e-871">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="8d32e-871">Add support for new catalog item type: package.</span></span> <span data-ttu-id="8d32e-872">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-872">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="8d32e-873">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="8d32e-873">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="8d32e-874">Таблица</span><span class="sxs-lookup"><span data-stu-id="8d32e-874">Table</span></span>
  * <span data-ttu-id="8d32e-875">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="8d32e-875">Table valued function</span></span>
  * <span data-ttu-id="8d32e-876">Просмотр</span><span class="sxs-lookup"><span data-stu-id="8d32e-876">View</span></span>
  * <span data-ttu-id="8d32e-877">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="8d32e-877">Table Statistics.</span></span> <span data-ttu-id="8d32e-878">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="8d32e-878">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8d32e-879">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="8d32e-879">Data Lake Store</span></span>

* <span data-ttu-id="8d32e-880">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="8d32e-880">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="8d32e-881">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-881">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="8d32e-882">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="8d32e-882">missed help for access show.</span></span> <span data-ttu-id="8d32e-883">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="8d32e-883">adding it.</span></span> <span data-ttu-id="8d32e-884">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="8d32e-884">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="8d32e-885">Поиск</span><span class="sxs-lookup"><span data-stu-id="8d32e-885">Find</span></span>

* <span data-ttu-id="8d32e-886">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="8d32e-886">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="8d32e-887">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8d32e-887">KeyVault</span></span>

* <span data-ttu-id="8d32e-888">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="8d32e-888">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="8d32e-889">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="8d32e-889">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="8d32e-890">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="8d32e-890">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="8d32e-891">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="8d32e-891">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="8d32e-892">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-892">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="8d32e-893">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="8d32e-893">Lab</span></span>

* <span data-ttu-id="8d32e-894">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="8d32e-894">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="8d32e-895">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="8d32e-895">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="8d32e-896">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="8d32e-896">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="8d32e-897">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="8d32e-897">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="8d32e-898">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="8d32e-898">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="8d32e-899">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="8d32e-899">Monitor</span></span>

* <span data-ttu-id="8d32e-900">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-900">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="8d32e-901">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-901">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="8d32e-902">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-902">Network</span></span>

* <span data-ttu-id="8d32e-903">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-903">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="8d32e-904">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-904">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="8d32e-905">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="8d32e-905">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="8d32e-906">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="8d32e-906">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="8d32e-907">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="8d32e-907">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="8d32e-908">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="8d32e-908">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="8d32e-909">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="8d32e-909">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="8d32e-910">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="8d32e-910">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="8d32e-911">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-911">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="8d32e-912">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="8d32e-912">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="8d32e-913">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-913">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="8d32e-914">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-914">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="8d32e-915">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="8d32e-915">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="8d32e-916">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="8d32e-916">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="8d32e-917">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="8d32e-917">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="8d32e-918">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="8d32e-918">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="8d32e-919">Профиль</span><span class="sxs-lookup"><span data-stu-id="8d32e-919">Profile</span></span>

* <span data-ttu-id="8d32e-920">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-920">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="8d32e-921">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-921">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="8d32e-922">Redis</span><span class="sxs-lookup"><span data-stu-id="8d32e-922">Redis</span></span>

* <span data-ttu-id="8d32e-923">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="8d32e-923">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="8d32e-924">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="8d32e-924">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="8d32e-925">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8d32e-925">Resource</span></span>

* <span data-ttu-id="8d32e-926">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-926">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="8d32e-927">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-927">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="8d32e-928">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-928">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="8d32e-929">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="8d32e-929">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="8d32e-930">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="8d32e-930">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="8d32e-931">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="8d32e-931">Add docs for az lock update.</span></span> <span data-ttu-id="8d32e-932">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="8d32e-932">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="8d32e-933">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="8d32e-933">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="8d32e-934">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="8d32e-934">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="8d32e-935">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="8d32e-935">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="8d32e-936">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="8d32e-936">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="8d32e-937">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-937">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="8d32e-938">Роль</span><span class="sxs-lookup"><span data-stu-id="8d32e-938">Role</span></span>

* <span data-ttu-id="8d32e-939">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-939">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="8d32e-940">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-940">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="8d32e-941">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-941">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="8d32e-942">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="8d32e-942">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="8d32e-943">SQL</span><span class="sxs-lookup"><span data-stu-id="8d32e-943">SQL</span></span>

* <span data-ttu-id="8d32e-944">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="8d32e-944">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="8d32e-945">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-945">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="8d32e-946">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-946">Storage</span></span>

* <span data-ttu-id="8d32e-947">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-947">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="8d32e-948">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-948">Add support for incremental blob copy</span></span>
* <span data-ttu-id="8d32e-949">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="8d32e-949">Add support for large block blob upload</span></span>
* <span data-ttu-id="8d32e-950">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="8d32e-950">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-951">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-951">VM</span></span>

* <span data-ttu-id="8d32e-952">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="8d32e-952">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="8d32e-953">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="8d32e-953">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="8d32e-954">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="8d32e-954">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="8d32e-955">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="8d32e-955">az vm/vmss disk</span></span>
  3. <span data-ttu-id="8d32e-956">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="8d32e-956">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="8d32e-957">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="8d32e-957">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="8d32e-958">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-958">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="8d32e-959">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-959">April 3, 2017</span></span>

<span data-ttu-id="8d32e-960">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="8d32e-960">Version 2.0.2</span></span>

<span data-ttu-id="8d32e-961">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="8d32e-961">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="8d32e-962">Core</span><span class="sxs-lookup"><span data-stu-id="8d32e-962">Core</span></span>

* <span data-ttu-id="8d32e-963">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8d32e-963">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="8d32e-964">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-964">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="8d32e-965">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-965">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="8d32e-966">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-966">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="8d32e-967">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-967">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="8d32e-968">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="8d32e-968">Add prompting for missing template parameters.</span></span> <span data-ttu-id="8d32e-969">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-969">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="8d32e-970">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8d32e-970">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="8d32e-971">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="8d32e-971">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="8d32e-972">ACS</span><span class="sxs-lookup"><span data-stu-id="8d32e-972">ACS</span></span>

* <span data-ttu-id="8d32e-973">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-973">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="8d32e-974">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="8d32e-974">Add support for ssh key password prompting.</span></span> <span data-ttu-id="8d32e-975">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-975">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="8d32e-976">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="8d32e-976">Add support for windows clusters.</span></span> <span data-ttu-id="8d32e-977">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-977">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="8d32e-978">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="8d32e-978">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="8d32e-979">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-979">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="8d32e-980">AppService</span><span class="sxs-lookup"><span data-stu-id="8d32e-980">AppService</span></span>

* <span data-ttu-id="8d32e-981">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-981">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="8d32e-982">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-982">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="8d32e-983">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-983">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="8d32e-984">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-984">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="8d32e-985">DataLake</span><span class="sxs-lookup"><span data-stu-id="8d32e-985">DataLake</span></span>

* <span data-ttu-id="8d32e-986">Первоначальный выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="8d32e-986">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="8d32e-987">Первоначальный выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="8d32e-987">Initial release of Data Lake Store module.</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="8d32e-988">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="8d32e-988">DocuemntDB</span></span>

* <span data-ttu-id="8d32e-989">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-989">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="8d32e-990">ВМ</span><span class="sxs-lookup"><span data-stu-id="8d32e-990">VM</span></span>

* <span data-ttu-id="8d32e-991">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-991">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="8d32e-992">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-992">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="8d32e-993">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-993">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="8d32e-994">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-994">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="8d32e-995">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-995">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="8d32e-996">Добавлена команда --secrets для виртуальных машин и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-996">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="8d32e-997">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="8d32e-997">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="8d32e-998">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8d32e-998">February 27, 2017</span></span>

<span data-ttu-id="8d32e-999">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="8d32e-999">Version 2.0.0</span></span>

<span data-ttu-id="8d32e-1000">Этот первый общедоступный выпуск Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="8d32e-1000">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="8d32e-1001">Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="8d32e-1001">General availability applies to these command modules:</span></span>
- <span data-ttu-id="8d32e-1002">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="8d32e-1002">Container Service (acs)</span></span>
- <span data-ttu-id="8d32e-1003">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="8d32e-1003">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="8d32e-1004">Сеть</span><span class="sxs-lookup"><span data-stu-id="8d32e-1004">Networking</span></span>
- <span data-ttu-id="8d32e-1005">Хранилище</span><span class="sxs-lookup"><span data-stu-id="8d32e-1005">Storage</span></span>

<span data-ttu-id="8d32e-1006">Эти командные модули могут использоваться в рабочих средах и поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания.</span><span class="sxs-lookup"><span data-stu-id="8d32e-1006">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="8d32e-1007">Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="8d32e-1007">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="8d32e-1008">Вы можете задавать вопросы на сайте [StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-1008">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="8d32e-1009">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="8d32e-1009">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="8d32e-1010">Чтобы проверить версию интерфейса командной строки, используйте `az --version`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-1010">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="8d32e-1011">В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="8d32e-1011">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="8d32e-1012">Некоторые командные модули имеют постфикс b*n* или rc*n*.</span><span class="sxs-lookup"><span data-stu-id="8d32e-1012">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="8d32e-1013">Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="8d32e-1013">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="8d32e-1014">У нас также есть предварительные ежедневные сборки интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="8d32e-1014">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="8d32e-1015">Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="8d32e-1015">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="8d32e-1016">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="8d32e-1016">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="8d32e-1017">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="8d32e-1017">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="8d32e-1018">обратившись к специалистам группы разработчиков продукта по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com);</span><span class="sxs-lookup"><span data-stu-id="8d32e-1018">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="8d32e-1019">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="8d32e-1019">Provide feedback from the command line with the `az feedback` command.</span></span>

