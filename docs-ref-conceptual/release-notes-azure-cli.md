---
title: Заметки о выпуске Azure CLI 2.0
description: Узнайте о последних обновлениях в Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 07/03/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 8d4f0879a18d2cf99ea7a284155bec86413406f8
ms.sourcegitcommit: da34d0eecf19c676826bd32ab254a92bd0976124
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/19/2018
ms.locfileid: "39138242"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="ad142-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="ad142-103">Azure CLI 2.0 release notes</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="ad142-104">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-104">July 18, 2018</span></span>

<span data-ttu-id="ad142-105">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="ad142-105">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="ad142-106">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-106">Core</span></span>

* <span data-ttu-id="ad142-107">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="ad142-107">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="ad142-108">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="ad142-108">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="ad142-109">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="ad142-109">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="ad142-110">ACR</span><span class="sxs-lookup"><span data-stu-id="ad142-110">ACR</span></span>

* <span data-ttu-id="ad142-111">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="ad142-111">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="ad142-112">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-112">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="ad142-113">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="ad142-113">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="ad142-114">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="ad142-114">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-115">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-115">ACS</span></span>

* <span data-ttu-id="ad142-116">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="ad142-116">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-117">AppService</span><span class="sxs-lookup"><span data-stu-id="ad142-117">AppService</span></span>

* <span data-ttu-id="ad142-118">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="ad142-118">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="ad142-119">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-119">Batch</span></span>

* <span data-ttu-id="ad142-120">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ad142-120">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="ad142-121">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="ad142-121">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ad142-122">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ad142-122">Batch AI</span></span>

* <span data-ttu-id="ad142-123">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="ad142-123">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="ad142-124">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-124">Container</span></span>

* <span data-ttu-id="ad142-125">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="ad142-125">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="ad142-126">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="ad142-126">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="ad142-127">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-127">Network</span></span>

* <span data-ttu-id="ad142-128">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ad142-128">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="ad142-129">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="ad142-129">Added `network nic wait`</span></span>
* <span data-ttu-id="ad142-130">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="ad142-130">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="ad142-131">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="ad142-131">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="ad142-132">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-132">Resource</span></span>

* <span data-ttu-id="ad142-133">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ad142-133">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="ad142-134">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ad142-134">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="ad142-135">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="ad142-135">Added `deployment wait` command</span></span>
* <span data-ttu-id="ad142-136">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="ad142-136">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-137">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-137">SQL</span></span>

* <span data-ttu-id="ad142-138">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-138">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="ad142-139">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="ad142-139">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="ad142-140">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="ad142-140">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-141">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-141">Storage</span></span>

* <span data-ttu-id="ad142-142">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="ad142-142">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-143">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-143">VM</span></span>

* <span data-ttu-id="ad142-144">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad142-144">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="ad142-145">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-145">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="ad142-146">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="ad142-146">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="ad142-147">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-147">July 3, 2018</span></span>

<span data-ttu-id="ad142-148">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="ad142-148">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="ad142-149">AKS</span><span class="sxs-lookup"><span data-stu-id="ad142-149">AKS</span></span>

* <span data-ttu-id="ad142-150">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="ad142-150">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="ad142-151">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-151">July 3, 2018</span></span>

<span data-ttu-id="ad142-152">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="ad142-152">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="ad142-153">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-153">Core</span></span>

* <span data-ttu-id="ad142-154">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="ad142-154">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="ad142-155">ACR</span><span class="sxs-lookup"><span data-stu-id="ad142-155">ACR</span></span>

* <span data-ttu-id="ad142-156">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="ad142-156">Added polling build status</span></span>
* <span data-ttu-id="ad142-157">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="ad142-157">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="ad142-158">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="ad142-158">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-159">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-159">ACS</span></span>

* <span data-ttu-id="ad142-160">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad142-160">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="ad142-161">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad142-161">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="ad142-162">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="ad142-162">Updated options for `aks browse` command.</span></span> <span data-ttu-id="ad142-163">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="ad142-163">Added `--listen-port` support</span></span>
* <span data-ttu-id="ad142-164">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ad142-164">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="ad142-165">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="ad142-165">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="ad142-166">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="ad142-166">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-167">AppService</span><span class="sxs-lookup"><span data-stu-id="ad142-167">AppService</span></span>

* <span data-ttu-id="ad142-168">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="ad142-168">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="ad142-169">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="ad142-169">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="ad142-170">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ad142-170">Backup</span></span>

* <span data-ttu-id="ad142-171">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="ad142-171">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="ad142-172">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ad142-172">BatchAI</span></span>

* <span data-ttu-id="ad142-173">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="ad142-173">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="ad142-174">Облако</span><span class="sxs-lookup"><span data-stu-id="ad142-174">Cloud</span></span>

* <span data-ttu-id="ad142-175">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="ad142-175">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="ad142-176">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-176">Container</span></span>

* <span data-ttu-id="ad142-177">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="ad142-177">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="ad142-178">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="ad142-178">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="ad142-179">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="ad142-179">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="ad142-180">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ad142-180">Extension</span></span>

* <span data-ttu-id="ad142-181">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="ad142-181">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="ad142-182">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-182">Network</span></span>

* <span data-ttu-id="ad142-183">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="ad142-183">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="ad142-184">Rdbms</span><span class="sxs-lookup"><span data-stu-id="ad142-184">Rdbms</span></span>

* <span data-ttu-id="ad142-185">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="ad142-185">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-186">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-186">Resource</span></span>

* <span data-ttu-id="ad142-187">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="ad142-187">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-188">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-188">VM</span></span>

* <span data-ttu-id="ad142-189">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="ad142-189">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="ad142-190">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-190">June 25, 2018</span></span>

<span data-ttu-id="ad142-191">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="ad142-191">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="ad142-192">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="ad142-192">CLI</span></span>

* <span data-ttu-id="ad142-193">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="ad142-193">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="ad142-194">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-194">June 19, 2018</span></span>

<span data-ttu-id="ad142-195">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="ad142-195">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="ad142-196">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-196">Core</span></span>

* <span data-ttu-id="ad142-197">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="ad142-197">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="ad142-198">ACR</span><span class="sxs-lookup"><span data-stu-id="ad142-198">ACR</span></span>

* <span data-ttu-id="ad142-199">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="ad142-199">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="ad142-200">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="ad142-200">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-201">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-201">ACS</span></span>

* <span data-ttu-id="ad142-202">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="ad142-202">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="ad142-203">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-203">Added `--update` support</span></span>
* <span data-ttu-id="ad142-204">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="ad142-204">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="ad142-205">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="ad142-205">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="ad142-206">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="ad142-206">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="ad142-207">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="ad142-207">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="ad142-208">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ad142-208">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="ad142-209">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ad142-209">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-210">AppService</span><span class="sxs-lookup"><span data-stu-id="ad142-210">AppService</span></span>

* <span data-ttu-id="ad142-211">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="ad142-211">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="ad142-212">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ad142-212">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="ad142-213">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-213">Batch</span></span>

* <span data-ttu-id="ad142-214">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="ad142-214">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ad142-215">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ad142-215">Batch AI</span></span>

* <span data-ttu-id="ad142-216">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="ad142-216">Added support for workspaces.</span></span> <span data-ttu-id="ad142-217">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ad142-217">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="ad142-218">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="ad142-218">Added support for experiments.</span></span> <span data-ttu-id="ad142-219">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="ad142-219">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="ad142-220">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="ad142-220">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="ad142-221">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="ad142-221">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="ad142-222">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="ad142-222">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="ad142-223">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="ad142-223">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="ad142-224">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="ad142-224">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="ad142-225">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="ad142-225">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="ad142-226">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-226">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="ad142-227">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="ad142-227">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="ad142-228">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-228">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="ad142-229">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="ad142-229">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="ad142-230">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="ad142-230">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="ad142-231">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="ad142-231">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="ad142-232">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-232">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="ad142-233">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="ad142-233">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="ad142-234">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="ad142-234">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="ad142-235">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="ad142-235">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="ad142-236">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="ad142-236">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="ad142-237">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="ad142-237">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="ad142-238">Карты</span><span class="sxs-lookup"><span data-stu-id="ad142-238">Maps</span></span>

* <span data-ttu-id="ad142-239">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="ad142-239">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="ad142-240">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-240">Network</span></span>

* <span data-ttu-id="ad142-241">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="ad142-241">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="ad142-242">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="ad142-242">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="ad142-243">#6502</span><span class="sxs-lookup"><span data-stu-id="ad142-243">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="ad142-244">Резервирование</span><span class="sxs-lookup"><span data-stu-id="ad142-244">Reservations</span></span>

* <span data-ttu-id="ad142-245">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-245">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="ad142-246">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-246">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="ad142-247">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="ad142-247">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="ad142-248">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="ad142-248">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="ad142-249">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="ad142-249">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="ad142-250">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-250">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="ad142-251">Роль</span><span class="sxs-lookup"><span data-stu-id="ad142-251">Role</span></span>

* <span data-ttu-id="ad142-252">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="ad142-252">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-253">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-253">SQL</span></span>

* <span data-ttu-id="ad142-254">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="ad142-254">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-255">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-255">Storage</span></span>

* <span data-ttu-id="ad142-256">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="ad142-256">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-257">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-257">VM</span></span>

* <span data-ttu-id="ad142-258">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-258">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="ad142-259">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="ad142-259">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="ad142-260">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="ad142-260">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="ad142-261">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-261">June 13, 2018</span></span>

<span data-ttu-id="ad142-262">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="ad142-262">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="ad142-263">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-263">Core</span></span>

* <span data-ttu-id="ad142-264">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="ad142-264">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="ad142-265">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-265">June 13, 2018</span></span>

<span data-ttu-id="ad142-266">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="ad142-266">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="ad142-267">AKS</span><span class="sxs-lookup"><span data-stu-id="ad142-267">AKS</span></span>

* <span data-ttu-id="ad142-268">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="ad142-268">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="ad142-269">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="ad142-269">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="ad142-270">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="ad142-270">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="ad142-271">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="ad142-271">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="ad142-272">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ad142-272">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-273">AppService</span><span class="sxs-lookup"><span data-stu-id="ad142-273">AppService</span></span>

* <span data-ttu-id="ad142-274">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="ad142-274">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ad142-275">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-275">June 5, 2018</span></span>

<span data-ttu-id="ad142-276">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="ad142-276">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="ad142-277">Interactive</span><span class="sxs-lookup"><span data-stu-id="ad142-277">Interactive</span></span>

* <span data-ttu-id="ad142-278">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="ad142-278">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="ad142-279">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-279">June 5, 2018</span></span>

<span data-ttu-id="ad142-280">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="ad142-280">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="ad142-281">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-281">Core</span></span>

* <span data-ttu-id="ad142-282">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="ad142-282">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="ad142-283">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ad142-283">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="ad142-284">ACR</span><span class="sxs-lookup"><span data-stu-id="ad142-284">ACR</span></span>

* <span data-ttu-id="ad142-285">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="ad142-285">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="ad142-286">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="ad142-286">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="ad142-287">AKS</span><span class="sxs-lookup"><span data-stu-id="ad142-287">AKS</span></span>

* <span data-ttu-id="ad142-288">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="ad142-288">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="ad142-289">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-289">Batch</span></span>

* <span data-ttu-id="ad142-290">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="ad142-290">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="ad142-291">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ad142-291">IOT</span></span>

* <span data-ttu-id="ad142-292">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="ad142-292">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="ad142-293">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-293">Network</span></span>

* <span data-ttu-id="ad142-294">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="ad142-294">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="ad142-295">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="ad142-295">Policy Insights</span></span>

* <span data-ttu-id="ad142-296">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ad142-296">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="ad142-297">ARM</span><span class="sxs-lookup"><span data-stu-id="ad142-297">ARM</span></span>

* <span data-ttu-id="ad142-298">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="ad142-298">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-299">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-299">SQL</span></span>

* <span data-ttu-id="ad142-300">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="ad142-300">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="ad142-301">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="ad142-301">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="ad142-302">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-302">Storage</span></span>

* <span data-ttu-id="ad142-303">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="ad142-303">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-304">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-304">VM</span></span>

* <span data-ttu-id="ad142-305">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="ad142-305">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="ad142-306">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-306">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="ad142-307">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-307">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="ad142-308">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-308">May 22, 2018</span></span>

<span data-ttu-id="ad142-309">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="ad142-309">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="ad142-310">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-310">Core</span></span>

* <span data-ttu-id="ad142-311">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="ad142-311">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-312">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-312">ACS</span></span>

* <span data-ttu-id="ad142-313">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="ad142-313">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="ad142-314">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="ad142-314">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-315">AppService</span><span class="sxs-lookup"><span data-stu-id="ad142-315">AppService</span></span>

* <span data-ttu-id="ad142-316">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="ad142-316">Improved generic update commands</span></span>
* <span data-ttu-id="ad142-317">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="ad142-317">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="ad142-318">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-318">Container</span></span>

* <span data-ttu-id="ad142-319">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="ad142-319">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="ad142-320">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ad142-320">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ad142-321">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ad142-321">Extension</span></span>

* <span data-ttu-id="ad142-322">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="ad142-322">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="ad142-323">Interactive</span><span class="sxs-lookup"><span data-stu-id="ad142-323">Interactive</span></span>

* <span data-ttu-id="ad142-324">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="ad142-324">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="ad142-325">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="ad142-325">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="ad142-326">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ad142-326">KeyVault</span></span>

* <span data-ttu-id="ad142-327">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="ad142-327">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="ad142-328">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-328">Network</span></span>

* <span data-ttu-id="ad142-329">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="ad142-329">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="ad142-330">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="ad142-330">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-331">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-331">SQL</span></span>

* <span data-ttu-id="ad142-332">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="ad142-332">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="ad142-333">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="ad142-333">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="ad142-334">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="ad142-334">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="ad142-335">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="ad142-335">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="ad142-336">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="ad142-336">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="ad142-337">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="ad142-337">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="ad142-338">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="ad142-338">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="ad142-339">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ad142-339">`edition`.</span></span> <span data-ttu-id="ad142-340">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="ad142-340">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="ad142-341">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="ad142-341">`elasticPoolName`.</span></span> <span data-ttu-id="ad142-342">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="ad142-342">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="ad142-343">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="ad142-343">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="ad142-344">`edition`.</span><span class="sxs-lookup"><span data-stu-id="ad142-344">`edition`.</span></span> <span data-ttu-id="ad142-345">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="ad142-345">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="ad142-346">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="ad142-346">`dtu`.</span></span> <span data-ttu-id="ad142-347">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="ad142-347">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="ad142-348">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="ad142-348">`databaseDtuMin`.</span></span> <span data-ttu-id="ad142-349">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="ad142-349">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="ad142-350">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="ad142-350">`databaseDtuMax`.</span></span> <span data-ttu-id="ad142-351">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="ad142-351">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="ad142-352">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="ad142-352">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="ad142-353">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="ad142-353">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-354">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-354">Storage</span></span>

* <span data-ttu-id="ad142-355">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="ad142-355">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="ad142-356">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="ad142-356">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-357">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-357">VM</span></span>

* <span data-ttu-id="ad142-358">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-358">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="ad142-359">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="ad142-359">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="ad142-360">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="ad142-360">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="ad142-361">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="ad142-361">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="ad142-362">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-362">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="ad142-363">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-363">May 7, 2018</span></span>

<span data-ttu-id="ad142-364">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="ad142-364">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="ad142-365">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-365">Core</span></span>

* <span data-ttu-id="ad142-366">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="ad142-366">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="ad142-367">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="ad142-367">Added limited support for positional arguments</span></span>
* <span data-ttu-id="ad142-368">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ad142-368">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="ad142-369">#5591</span><span class="sxs-lookup"><span data-stu-id="ad142-369">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="ad142-370">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ad142-370">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="ad142-371">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="ad142-371">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="ad142-372">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="ad142-372">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="ad142-373">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="ad142-373">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="ad142-374">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="ad142-374">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="ad142-375">ACR</span><span class="sxs-lookup"><span data-stu-id="ad142-375">ACR</span></span>

* <span data-ttu-id="ad142-376">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="ad142-376">Added ACR Build commands</span></span>
* <span data-ttu-id="ad142-377">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="ad142-377">Improved resource not found error messages</span></span>
* <span data-ttu-id="ad142-378">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="ad142-378">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="ad142-379">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="ad142-379">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="ad142-380">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="ad142-380">Improved repository commands error messages</span></span>
* <span data-ttu-id="ad142-381">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="ad142-381">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-382">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-382">ACS</span></span>

* <span data-ttu-id="ad142-383">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="ad142-383">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="ad142-384">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="ad142-384">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="ad142-385">AMS</span><span class="sxs-lookup"><span data-stu-id="ad142-385">AMS</span></span>

* <span data-ttu-id="ad142-386">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="ad142-386">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-387">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-387">Appservice</span></span>

* <span data-ttu-id="ad142-388">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="ad142-388">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="ad142-389">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-389">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="ad142-390">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="ad142-390">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="ad142-391">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ad142-391">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="ad142-392">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ad142-392">Batch AI</span></span>

* <span data-ttu-id="ad142-393">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="ad142-393">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ad142-394">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ad142-394">Cognitive Services</span></span>

* <span data-ttu-id="ad142-395">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="ad142-395">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="ad142-396">Потребление</span><span class="sxs-lookup"><span data-stu-id="ad142-396">Consumption</span></span>

* <span data-ttu-id="ad142-397">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="ad142-397">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="ad142-398">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-398">Container</span></span>

* <span data-ttu-id="ad142-399">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="ad142-399">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="ad142-400">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="ad142-400">Cosmos DB</span></span>

* <span data-ttu-id="ad142-401">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ad142-401">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="ad142-402">DMS</span><span class="sxs-lookup"><span data-stu-id="ad142-402">DMS</span></span>

* <span data-ttu-id="ad142-403">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="ad142-403">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="ad142-404">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ad142-404">Extension</span></span>

* <span data-ttu-id="ad142-405">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="ad142-405">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="ad142-406">Interactive</span><span class="sxs-lookup"><span data-stu-id="ad142-406">Interactive</span></span>

* <span data-ttu-id="ad142-407">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="ad142-407">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="ad142-408">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="ad142-408">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="ad142-409">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="ad142-409">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="ad142-410">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="ad142-410">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="ad142-411">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ad142-411">Lab</span></span>

* <span data-ttu-id="ad142-412">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="ad142-412">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="ad142-413">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-413">Network</span></span>

* <span data-ttu-id="ad142-414">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="ad142-414">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="ad142-415">Профиль</span><span class="sxs-lookup"><span data-stu-id="ad142-415">Profile</span></span>

* <span data-ttu-id="ad142-416">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-416">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="ad142-417">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="ad142-417">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="ad142-418">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="ad142-418">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="ad142-419">Redis</span><span class="sxs-lookup"><span data-stu-id="ad142-419">Redis</span></span>

* <span data-ttu-id="ad142-420">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-420">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="ad142-421">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="ad142-421">Deprecated `redis list-all`.</span></span> <span data-ttu-id="ad142-422">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="ad142-422">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="ad142-423">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="ad142-423">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="ad142-424">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="ad142-424">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="ad142-425">Роль</span><span class="sxs-lookup"><span data-stu-id="ad142-425">Role</span></span>

* <span data-ttu-id="ad142-426">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="ad142-426">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-427">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-427">Storage</span></span>

* <span data-ttu-id="ad142-428">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="ad142-428">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="ad142-429">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="ad142-429">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="ad142-430">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="ad142-430">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="ad142-431">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="ad142-431">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="ad142-432">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="ad142-432">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-433">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-433">VM</span></span>

* <span data-ttu-id="ad142-434">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="ad142-434">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="ad142-435">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="ad142-435">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="ad142-436">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="ad142-436">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="ad142-437">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="ad142-437">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="ad142-438">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="ad142-438">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="ad142-439">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="ad142-439">Added write accelerator support</span></span>
* <span data-ttu-id="ad142-440">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="ad142-440">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="ad142-441">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="ad142-441">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="ad142-442">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="ad142-442">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="ad142-443">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-443">April 10, 2018</span></span>

<span data-ttu-id="ad142-444">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="ad142-444">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="ad142-445">ACR</span><span class="sxs-lookup"><span data-stu-id="ad142-445">ACR</span></span>

* <span data-ttu-id="ad142-446">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="ad142-446">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-447">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-447">ACS</span></span>

* <span data-ttu-id="ad142-448">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="ad142-448">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-449">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-449">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="ad142-451">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="ad142-451">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="ad142-452">Batch AI</span><span class="sxs-lookup"><span data-stu-id="ad142-452">BatchAI</span></span>

* <span data-ttu-id="ad142-453">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="ad142-453">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="ad142-454">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="ad142-454">Job level mounting</span></span>
 - <span data-ttu-id="ad142-455">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="ad142-455">Environment variables with secret values</span></span>
 - <span data-ttu-id="ad142-456">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="ad142-456">Performance counters settings</span></span>
 - <span data-ttu-id="ad142-457">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="ad142-457">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="ad142-458">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="ad142-458">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="ad142-459">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="ad142-459">Usage and limits reporting</span></span>
 - <span data-ttu-id="ad142-460">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="ad142-460">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="ad142-461">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="ad142-461">Support for custom images</span></span>
 - <span data-ttu-id="ad142-462">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="ad142-462">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="ad142-463">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="ad142-463">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="ad142-464">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="ad142-464">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="ad142-465">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="ad142-465">National clouds are supported</span></span>
* <span data-ttu-id="ad142-466">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="ad142-466">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="ad142-467">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="ad142-467">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="ad142-468">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="ad142-468">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="ad142-469">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="ad142-469">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="ad142-470">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="ad142-470">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="ad142-471">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="ad142-471">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="ad142-472">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-472">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="ad142-473">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="ad142-473">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="ad142-474">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="ad142-474">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="ad142-475">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-475">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="ad142-476">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="ad142-476">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="ad142-477">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="ad142-477">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="ad142-478">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-478">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="ad142-479">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="ad142-479">Billing</span></span>

* <span data-ttu-id="ad142-480">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="ad142-480">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="ad142-481">Потребление</span><span class="sxs-lookup"><span data-stu-id="ad142-481">Consumption</span></span>

* <span data-ttu-id="ad142-482">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="ad142-482">Added `marketplace` commands</span></span>
* <span data-ttu-id="ad142-483">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="ad142-483">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="ad142-484">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="ad142-484">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="ad142-485">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="ad142-485">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="ad142-486">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="ad142-486">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="ad142-487">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="ad142-487">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="ad142-488">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-488">Container</span></span>

* <span data-ttu-id="ad142-489">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="ad142-489">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="ad142-490">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="ad142-490">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="ad142-491">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ad142-491">Extension</span></span>

* <span data-ttu-id="ad142-492">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="ad142-492">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="ad142-493">Interactive</span><span class="sxs-lookup"><span data-stu-id="ad142-493">Interactive</span></span>

* <span data-ttu-id="ad142-494">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="ad142-494">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="ad142-495">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="ad142-495">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="ad142-496">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="ad142-496">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="ad142-497">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-497">Network</span></span>

* <span data-ttu-id="ad142-498">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-498">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="ad142-499">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-499">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="ad142-500">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="ad142-500">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="ad142-501">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="ad142-501">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="ad142-502">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="ad142-502">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="ad142-503">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-503">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="ad142-504">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-504">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="ad142-505">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="ad142-505">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="ad142-506">Профиль</span><span class="sxs-lookup"><span data-stu-id="ad142-506">Profile</span></span>

* <span data-ttu-id="ad142-507">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="ad142-507">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="ad142-508">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="ad142-508">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="ad142-509">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ad142-509">RDBMS</span></span>

* <span data-ttu-id="ad142-510">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="ad142-510">Added `georestore` command</span></span>
* <span data-ttu-id="ad142-511">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="ad142-511">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-512">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-512">Resource</span></span>

* <span data-ttu-id="ad142-513">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-513">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="ad142-514">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-514">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-515">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-515">SQL</span></span>

* <span data-ttu-id="ad142-516">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="ad142-516">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-517">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-517">Storage</span></span>

* <span data-ttu-id="ad142-518">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="ad142-518">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-519">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-519">VM</span></span>

* <span data-ttu-id="ad142-520">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="ad142-520">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="ad142-521">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="ad142-521">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="ad142-523">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-523">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="ad142-524">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="ad142-524">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="ad142-525">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="ad142-525">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="ad142-526">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="ad142-526">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="ad142-527">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-527">March 27, 2018</span></span>

<span data-ttu-id="ad142-528">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="ad142-528">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="ad142-529">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-529">Core</span></span>

* <span data-ttu-id="ad142-530">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ad142-530">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-531">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-531">ACS</span></span>

* <span data-ttu-id="ad142-532">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ad142-532">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-533">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-533">Appservice</span></span>

* <span data-ttu-id="ad142-534">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-534">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="ad142-535">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-535">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ad142-536">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ad142-536">Backup</span></span>

* <span data-ttu-id="ad142-537">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="ad142-537">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="ad142-538">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="ad142-538">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="ad142-539">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ad142-539">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="ad142-540">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-540">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="ad142-541">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-541">Container</span></span>

* <span data-ttu-id="ad142-542">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="ad142-542">Added `container exec` command.</span></span> <span data-ttu-id="ad142-543">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ad142-543">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="ad142-544">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ad142-544">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="ad142-545">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ad142-545">Extension</span></span>

* <span data-ttu-id="ad142-546">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="ad142-546">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="ad142-547">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="ad142-547">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="ad142-548">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad142-548">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="ad142-549">Interactive</span><span class="sxs-lookup"><span data-stu-id="ad142-549">Interactive</span></span>

* <span data-ttu-id="ad142-550">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="ad142-550">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="ad142-551">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="ad142-551">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="ad142-552">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="ad142-552">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="ad142-553">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="ad142-553">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="ad142-554">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ad142-554">Lab</span></span>

* <span data-ttu-id="ad142-555">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="ad142-555">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="ad142-556">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ad142-556">Monitor</span></span>

* <span data-ttu-id="ad142-557">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="ad142-557">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="ad142-558">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="ad142-558">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="ad142-559">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="ad142-559">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="ad142-560">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-560">Network</span></span>

* <span data-ttu-id="ad142-561">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="ad142-561">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="ad142-562">Профиль</span><span class="sxs-lookup"><span data-stu-id="ad142-562">Profile</span></span>

* <span data-ttu-id="ad142-563">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="ad142-563">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ad142-564">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ad142-564">RDBMS</span></span>

* <span data-ttu-id="ad142-565">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="ad142-565">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-566">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-566">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="ad142-568">Роль</span><span class="sxs-lookup"><span data-stu-id="ad142-568">Role</span></span>

* <span data-ttu-id="ad142-569">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-569">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="ad142-570">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="ad142-570">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="ad142-571">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="ad142-571">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="ad142-572">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-572">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="ad142-573">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="ad142-573">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-574">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-574">Storage</span></span>

* <span data-ttu-id="ad142-575">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ad142-575">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="ad142-576">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="ad142-576">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-577">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-577">VM</span></span>

* <span data-ttu-id="ad142-578">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="ad142-578">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="ad142-579">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-579">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="ad142-580">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="ad142-580">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="ad142-581">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="ad142-581">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="ad142-582">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-582">March 13, 2018</span></span>

<span data-ttu-id="ad142-583">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="ad142-583">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="ad142-584">ACR</span><span class="sxs-lookup"><span data-stu-id="ad142-584">ACR</span></span>

* <span data-ttu-id="ad142-585">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="ad142-585">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="ad142-586">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ad142-586">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="ad142-587">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="ad142-587">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-588">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-588">ACS</span></span>

* <span data-ttu-id="ad142-589">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="ad142-589">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="ad142-590">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="ad142-590">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="ad142-591">Помощник</span><span class="sxs-lookup"><span data-stu-id="ad142-591">Advisor</span></span>

* <span data-ttu-id="ad142-592">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="ad142-592">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="ad142-593">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-593">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="ad142-594">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="ad142-594">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="ad142-595">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="ad142-595">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="ad142-596">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-596">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-597">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-597">Appservice</span></span>

* <span data-ttu-id="ad142-598">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="ad142-598">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="ad142-599">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-599">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="ad142-600">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="ad142-600">Eventhubs</span></span>

* <span data-ttu-id="ad142-601">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ad142-601">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="ad142-602">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ad142-602">Extension</span></span>

* <span data-ttu-id="ad142-603">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="ad142-603">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="ad142-604">Interactive</span><span class="sxs-lookup"><span data-stu-id="ad142-604">Interactive</span></span>

* <span data-ttu-id="ad142-605">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="ad142-605">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="ad142-606">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="ad142-606">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="ad142-607">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="ad142-607">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="ad142-608">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="ad142-608">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="ad142-609">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ad142-609">Monitor</span></span>

* <span data-ttu-id="ad142-610">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ad142-610">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="ad142-611">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="ad142-611">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="ad142-612">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="ad142-612">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="ad142-613">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="ad142-613">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="ad142-614">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-614">Network</span></span>

* <span data-ttu-id="ad142-615">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-615">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="ad142-616">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ad142-616">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="ad142-617">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="ad142-617">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="ad142-618">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ad142-618">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="ad142-619">Профиль</span><span class="sxs-lookup"><span data-stu-id="ad142-619">Profile</span></span>

* <span data-ttu-id="ad142-620">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="ad142-620">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="ad142-621">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="ad142-621">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="ad142-622">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ad142-622">RDBMS</span></span>

* <span data-ttu-id="ad142-623">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="ad142-623">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="ad142-624">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-624">Service Bus</span></span>

* <span data-ttu-id="ad142-625">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ad142-625">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-626">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-626">Storage</span></span>

* <span data-ttu-id="ad142-627">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="ad142-627">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="ad142-628">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="ad142-628">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-629">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-629">VM</span></span>

* <span data-ttu-id="ad142-630">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="ad142-630">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="ad142-631">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="ad142-631">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="ad142-632">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-632">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="ad142-633">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="ad142-633">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="ad142-634">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="ad142-634">February 27, 2018</span></span>

<span data-ttu-id="ad142-635">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="ad142-635">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="ad142-636">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-636">Core</span></span>

* <span data-ttu-id="ad142-637">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="ad142-637">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="ad142-638">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="ad142-638">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="ad142-639">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="ad142-639">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-640">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-640">ACS</span></span>

* <span data-ttu-id="ad142-641">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad142-641">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="ad142-642">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="ad142-642">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="ad142-643">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="ad142-643">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="ad142-644">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="ad142-644">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-645">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-645">Appservice</span></span>

* <span data-ttu-id="ad142-646">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="ad142-646">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="ad142-647">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="ad142-647">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="ad142-648">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="ad142-648">Cognitive Services</span></span>

* <span data-ttu-id="ad142-649">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="ad142-649">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="ad142-650">Потребление</span><span class="sxs-lookup"><span data-stu-id="ad142-650">Consumption</span></span>

* <span data-ttu-id="ad142-651">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="ad142-651">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="ad142-652">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="ad142-652">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="ad142-653">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-653">Container</span></span>

* <span data-ttu-id="ad142-654">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="ad142-654">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="ad142-655">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-655">Network</span></span>

* <span data-ttu-id="ad142-656">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="ad142-656">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-657">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-657">Resource</span></span>

* <span data-ttu-id="ad142-658">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="ad142-658">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="ad142-659">Роль</span><span class="sxs-lookup"><span data-stu-id="ad142-659">Role</span></span>

* <span data-ttu-id="ad142-660">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ad142-660">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-661">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-661">SQL</span></span>

* <span data-ttu-id="ad142-662">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="ad142-662">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-663">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-663">Storage</span></span>

* <span data-ttu-id="ad142-664">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-664">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-665">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-665">VM</span></span>

* <span data-ttu-id="ad142-666">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="ad142-666">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="ad142-667">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-667">February 13, 2018</span></span>

<span data-ttu-id="ad142-668">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="ad142-668">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="ad142-669">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-669">Core</span></span>

* <span data-ttu-id="ad142-670">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="ad142-670">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-671">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-671">ACS</span></span>

* <span data-ttu-id="ad142-672">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="ad142-672">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="ad142-673">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-673">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="ad142-674">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ad142-674">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="ad142-675">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="ad142-675">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="ad142-676">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="ad142-676">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="ad142-677">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="ad142-677">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="ad142-678">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ad142-678">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="ad142-679">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="ad142-679">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-680">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-680">Appservice</span></span>

* <span data-ttu-id="ad142-681">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="ad142-681">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="ad142-682">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="ad142-682">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="ad142-683">CDN</span><span class="sxs-lookup"><span data-stu-id="ad142-683">CDN</span></span>

* <span data-ttu-id="ad142-684">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-684">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="ad142-685">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-685">Container</span></span>

* <span data-ttu-id="ad142-686">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="ad142-686">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="ad142-687">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ad142-687">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ad142-688">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ad142-688">CosmosDB</span></span>

* <span data-ttu-id="ad142-689">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="ad142-689">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="ad142-690">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ad142-690">Extension</span></span>

* <span data-ttu-id="ad142-691">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-691">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="ad142-692">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-692">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="ad142-693">Отзыв</span><span class="sxs-lookup"><span data-stu-id="ad142-693">Feedback</span></span>

* <span data-ttu-id="ad142-694">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ad142-694">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="ad142-695">Interactive</span><span class="sxs-lookup"><span data-stu-id="ad142-695">Interactive</span></span>

* <span data-ttu-id="ad142-696">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="ad142-696">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="ad142-697">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="ad142-697">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="ad142-698">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ad142-698">IoT</span></span>

* <span data-ttu-id="ad142-699">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="ad142-699">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ad142-700">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="ad142-700">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="ad142-701">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-701">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="ad142-702">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="ad142-702">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="ad142-703">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ad142-703">Monitor</span></span>

* <span data-ttu-id="ad142-704">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-704">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="ad142-705">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-705">Network</span></span>

* <span data-ttu-id="ad142-706">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="ad142-706">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="ad142-707">Профиль</span><span class="sxs-lookup"><span data-stu-id="ad142-707">Profile</span></span>

* <span data-ttu-id="ad142-708">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="ad142-708">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-709">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-709">Resource</span></span>

* <span data-ttu-id="ad142-710">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-710">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="ad142-711">Роль</span><span class="sxs-lookup"><span data-stu-id="ad142-711">Role</span></span>

* <span data-ttu-id="ad142-712">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="ad142-712">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-713">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-713">SQL</span></span>

* <span data-ttu-id="ad142-714">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="ad142-714">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="ad142-715">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="ad142-715">Added `sql db rename`</span></span>
* <span data-ttu-id="ad142-716">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="ad142-716">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-717">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-717">Storage</span></span>

* <span data-ttu-id="ad142-718">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="ad142-718">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-719">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-719">VM</span></span>

* <span data-ttu-id="ad142-720">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="ad142-720">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="ad142-721">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="ad142-721">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="ad142-722">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="ad142-722">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="ad142-723">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-723">January 31, 2018</span></span>

<span data-ttu-id="ad142-724">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="ad142-724">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="ad142-725">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-725">Core</span></span>

* <span data-ttu-id="ad142-726">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="ad142-726">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="ad142-727">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="ad142-727">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="ad142-728">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="ad142-728">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="ad142-729">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="ad142-729">Use `--verbose` to see</span></span>
* <span data-ttu-id="ad142-730">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="ad142-730">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-731">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-731">ACS</span></span>

* <span data-ttu-id="ad142-732">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="ad142-732">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="ad142-733">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="ad142-733">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-734">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-734">Appservice</span></span>

* <span data-ttu-id="ad142-735">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="ad142-735">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="ad142-736">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="ad142-736">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="ad142-737">CDN</span><span class="sxs-lookup"><span data-stu-id="ad142-737">CDN</span></span>

* <span data-ttu-id="ad142-738">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-738">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ad142-739">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ad142-739">CosmosDB</span></span>

* <span data-ttu-id="ad142-740">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="ad142-740">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="ad142-741">Interactive</span><span class="sxs-lookup"><span data-stu-id="ad142-741">Interactive</span></span>

* <span data-ttu-id="ad142-742">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="ad142-742">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="ad142-743">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-743">Network</span></span>

* <span data-ttu-id="ad142-744">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-744">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="ad142-745">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad142-745">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="ad142-746">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-746">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="ad142-747">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-747">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="ad142-748">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="ad142-748">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="ad142-749">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="ad142-749">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="ad142-750">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="ad142-750">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="ad142-751">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="ad142-751">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="ad142-752">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="ad142-752">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="ad142-753">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="ad142-753">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="ad142-754">Профиль</span><span class="sxs-lookup"><span data-stu-id="ad142-754">Profile</span></span>

* <span data-ttu-id="ad142-755">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="ad142-755">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-756">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-756">Resource</span></span>

* <span data-ttu-id="ad142-757">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="ad142-757">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-758">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-758">Storage</span></span>

* <span data-ttu-id="ad142-759">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="ad142-759">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="ad142-760">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="ad142-760">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="ad142-761">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="ad142-761">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="ad142-762">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-762">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="ad142-763">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="ad142-763">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-764">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-764">VM</span></span>

* <span data-ttu-id="ad142-765">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="ad142-765">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="ad142-766">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ad142-766">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="ad142-767">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="ad142-767">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="ad142-768">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-768">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="ad142-769">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-769">January 17, 2018</span></span>

<span data-ttu-id="ad142-770">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="ad142-770">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="ad142-771">ACR</span><span class="sxs-lookup"><span data-stu-id="ad142-771">ACR</span></span>

* <span data-ttu-id="ad142-772">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="ad142-772">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="ad142-773">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="ad142-773">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-774">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-774">ACS</span></span>

* <span data-ttu-id="ad142-775">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="ad142-775">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="ad142-776">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="ad142-776">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-777">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-777">Appservice</span></span>

* <span data-ttu-id="ad142-778">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="ad142-778">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="ad142-779">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="ad142-779">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="ad142-780">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="ad142-780">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="ad142-781">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ad142-781">Backup</span></span>

* <span data-ttu-id="ad142-782">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="ad142-782">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="ad142-783">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="ad142-783">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="ad142-784">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="ad142-784">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="ad142-785">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="ad142-785">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="ad142-786">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="ad142-786">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="ad142-787">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-787">Batch</span></span>

* <span data-ttu-id="ad142-788">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="ad142-788">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="ad142-789">Облако</span><span class="sxs-lookup"><span data-stu-id="ad142-789">Cloud</span></span>

* <span data-ttu-id="ad142-790">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="ad142-790">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="ad142-791">Потребление</span><span class="sxs-lookup"><span data-stu-id="ad142-791">Consumption</span></span>

* <span data-ttu-id="ad142-792">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="ad142-792">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="ad142-793">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-793">Event Grid</span></span>

* <span data-ttu-id="ad142-794">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="ad142-794">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ad142-795">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="ad142-795">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="ad142-796">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="ad142-796">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="ad142-797">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="ad142-797">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="ad142-798">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-798">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="ad142-799">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-799">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="ad142-800">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="ad142-800">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="ad142-801">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="ad142-801">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="ad142-802">Interactive</span><span class="sxs-lookup"><span data-stu-id="ad142-802">Interactive</span></span>

* <span data-ttu-id="ad142-803">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="ad142-803">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="ad142-804">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="ad142-804">Fixed errors on startup</span></span>
* <span data-ttu-id="ad142-805">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="ad142-805">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="ad142-806">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ad142-806">IoT</span></span>

* <span data-ttu-id="ad142-807">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="ad142-807">Added support for device provisioning service</span></span>
* <span data-ttu-id="ad142-808">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="ad142-808">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="ad142-809">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="ad142-809">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="ad142-810">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ad142-810">Monitor</span></span>

* <span data-ttu-id="ad142-811">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="ad142-811">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="ad142-812">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-812">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="ad142-813">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="ad142-813">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="ad142-814">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-814">Network</span></span>

* <span data-ttu-id="ad142-815">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="ad142-815">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="ad142-816">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="ad142-816">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="ad142-817">Профиль</span><span class="sxs-lookup"><span data-stu-id="ad142-817">Profile</span></span>

* <span data-ttu-id="ad142-818">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ad142-818">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="ad142-819">Роль</span><span class="sxs-lookup"><span data-stu-id="ad142-819">Role</span></span>

* <span data-ttu-id="ad142-820">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="ad142-820">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ad142-821">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ad142-821">Service Fabric</span></span>

* <span data-ttu-id="ad142-822">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="ad142-822">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="ad142-823">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="ad142-823">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-824">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-824">VM</span></span>

* <span data-ttu-id="ad142-825">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="ad142-825">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="ad142-826">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="ad142-826">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="ad142-827">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="ad142-827">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="ad142-828">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="ad142-828">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="ad142-829">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="ad142-829">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="ad142-830">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="ad142-830">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="ad142-831">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-831">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="ad142-832">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="ad142-832">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="ad142-833">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-833">December 19, 2017</span></span>

<span data-ttu-id="ad142-834">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="ad142-834">Version 2.0.23</span></span>

* <span data-ttu-id="ad142-835">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="ad142-835">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="ad142-836">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-836">Container</span></span>

* <span data-ttu-id="ad142-837">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ad142-837">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="ad142-838">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-838">Network</span></span>

* <span data-ttu-id="ad142-839">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ad142-839">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="ad142-840">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ad142-840">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-841">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-841">Storage</span></span>

* <span data-ttu-id="ad142-842">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="ad142-842">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-843">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-843">VM</span></span>

* <span data-ttu-id="ad142-844">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="ad142-844">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="ad142-845">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-845">December 5, 2017</span></span>

<span data-ttu-id="ad142-846">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="ad142-846">Version 2.0.22</span></span>

* <span data-ttu-id="ad142-847">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="ad142-847">Removed `az component` commands.</span></span> <span data-ttu-id="ad142-848">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="ad142-848">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="ad142-849">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-849">Core</span></span>
* <span data-ttu-id="ad142-850">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="ad142-850">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="ad142-851">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ad142-851">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-852">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-852">ACS</span></span>

* <span data-ttu-id="ad142-853">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="ad142-853">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="ad142-854">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-854">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="ad142-855">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="ad142-855">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="ad142-856">Помощник</span><span class="sxs-lookup"><span data-stu-id="ad142-856">Advisor</span></span>

* <span data-ttu-id="ad142-857">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ad142-857">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-858">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-858">Appservice</span></span>

* <span data-ttu-id="ad142-859">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="ad142-859">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="ad142-860">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="ad142-860">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="ad142-861">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="ad142-861">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="ad142-862">Потребление</span><span class="sxs-lookup"><span data-stu-id="ad142-862">Consumption</span></span>

* <span data-ttu-id="ad142-863">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="ad142-863">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="ad142-864">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-864">Container</span></span>

* <span data-ttu-id="ad142-865">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="ad142-865">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="ad142-866">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ad142-866">Monitor</span></span>

* <span data-ttu-id="ad142-867">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="ad142-867">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-868">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-868">Resource</span></span>

* <span data-ttu-id="ad142-869">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="ad142-869">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="ad142-870">Роль</span><span class="sxs-lookup"><span data-stu-id="ad142-870">Role</span></span>

* <span data-ttu-id="ad142-871">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="ad142-871">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="ad142-872">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="ad142-872">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="ad142-873">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="ad142-873">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-874">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-874">SQL</span></span>

* <span data-ttu-id="ad142-875">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="ad142-875">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="ad142-876">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-876">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-877">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-877">VM</span></span>

* <span data-ttu-id="ad142-878">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ad142-878">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="ad142-879">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-879">November 14, 2017</span></span>

<span data-ttu-id="ad142-880">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="ad142-880">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="ad142-881">ACR</span><span class="sxs-lookup"><span data-stu-id="ad142-881">ACR</span></span>

* <span data-ttu-id="ad142-882">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="ad142-882">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="ad142-883">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-883">ACS</span></span>

* <span data-ttu-id="ad142-884">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="ad142-884">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="ad142-885">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="ad142-885">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="ad142-886">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="ad142-886">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="ad142-887">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="ad142-887">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="ad142-888">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="ad142-888">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-889">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-889">Appservice</span></span>

* <span data-ttu-id="ad142-890">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="ad142-890">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="ad142-891">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="ad142-891">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="ad142-892">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="ad142-892">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="ad142-893">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="ad142-893">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="ad142-894">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="ad142-894">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="ad142-895">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="ad142-895">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="ad142-896">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-896">Batch</span></span>

* <span data-ttu-id="ad142-897">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="ad142-897">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="ad142-898">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ad142-898">Batchai</span></span>

* <span data-ttu-id="ad142-899">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-899">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="ad142-900">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-900">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="ad142-901">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="ad142-901">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="ad142-902">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-902">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="ad142-903">Облако</span><span class="sxs-lookup"><span data-stu-id="ad142-903">Cloud</span></span>

* <span data-ttu-id="ad142-904">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="ad142-904">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="ad142-905">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-905">Container</span></span>

* <span data-ttu-id="ad142-906">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="ad142-906">Added support to open multiple ports</span></span>
* <span data-ttu-id="ad142-907">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ad142-907">Added container group restart policy</span></span>
* <span data-ttu-id="ad142-908">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="ad142-908">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="ad142-909">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="ad142-909">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ad142-910">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ad142-910">Data Lake Analytics</span></span>

* <span data-ttu-id="ad142-911">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="ad142-911">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ad142-912">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ad142-912">Data Lake Store</span></span>

* <span data-ttu-id="ad142-913">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="ad142-913">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="ad142-914">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ad142-914">Extension</span></span>

* <span data-ttu-id="ad142-915">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="ad142-915">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="ad142-916">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="ad142-916">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="ad142-917">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ad142-917">IoT</span></span>

* <span data-ttu-id="ad142-918">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ad142-918">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="ad142-919">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ad142-919">Monitor</span></span>

* <span data-ttu-id="ad142-920">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="ad142-920">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="ad142-921">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-921">Network</span></span>

* <span data-ttu-id="ad142-922">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="ad142-922">Added support for CAA DNS records</span></span>
* <span data-ttu-id="ad142-923">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-923">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="ad142-924">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="ad142-924">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="ad142-925">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="ad142-925">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="ad142-926">Резервирование</span><span class="sxs-lookup"><span data-stu-id="ad142-926">Reservations</span></span>

* <span data-ttu-id="ad142-927">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="ad142-927">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-928">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-928">Resource</span></span>

* <span data-ttu-id="ad142-929">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="ad142-929">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-930">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-930">SQL</span></span>

* <span data-ttu-id="ad142-931">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-931">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-932">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-932">Storage</span></span>

* <span data-ttu-id="ad142-933">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad142-933">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="ad142-934">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="ad142-934">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="ad142-935">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="ad142-935">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="ad142-936">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="ad142-936">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="ad142-937">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-937">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="ad142-938">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="ad142-938">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="ad142-939">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-939">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-940">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-940">VM</span></span>

* <span data-ttu-id="ad142-941">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="ad142-941">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="ad142-942">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="ad142-942">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="ad142-943">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="ad142-943">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="ad142-944">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="ad142-944">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="ad142-945">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="ad142-945">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="ad142-946">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-946">October 24, 2017</span></span>

<span data-ttu-id="ad142-947">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="ad142-947">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="ad142-948">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-948">Core</span></span>

* <span data-ttu-id="ad142-949">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="ad142-949">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="ad142-950">ACR</span><span class="sxs-lookup"><span data-stu-id="ad142-950">ACR</span></span>

* <span data-ttu-id="ad142-951">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="ad142-951">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="ad142-952">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="ad142-952">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="ad142-953">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="ad142-953">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-954">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-954">ACS</span></span>

* <span data-ttu-id="ad142-955">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="ad142-955">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="ad142-956">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="ad142-956">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-957">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-957">Appservice</span></span>

* <span data-ttu-id="ad142-958">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="ad142-958">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="ad142-959">Компонент</span><span class="sxs-lookup"><span data-stu-id="ad142-959">Component</span></span>

* <span data-ttu-id="ad142-960">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="ad142-960">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="ad142-961">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ad142-961">Monitor</span></span>

* <span data-ttu-id="ad142-962">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="ad142-962">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-963">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-963">Resource</span></span>

* <span data-ttu-id="ad142-964">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="ad142-964">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="ad142-965">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="ad142-965">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-966">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-966">VM</span></span>

* <span data-ttu-id="ad142-967">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="ad142-967">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="ad142-968">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-968">October 9, 2017</span></span>

<span data-ttu-id="ad142-969">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="ad142-969">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="ad142-970">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-970">Core</span></span>

* <span data-ttu-id="ad142-971">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="ad142-971">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-972">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-972">Appservice</span></span>

* <span data-ttu-id="ad142-973">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-973">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="ad142-974">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-974">Batch</span></span>

* <span data-ttu-id="ad142-975">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="ad142-975">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="ad142-976">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="ad142-976">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="ad142-977">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="ad142-977">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="ad142-978">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="ad142-978">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="ad142-979">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ad142-979">Batchai</span></span>

* <span data-ttu-id="ad142-980">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="ad142-980">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="ad142-981">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ad142-981">Keyvault</span></span>

* <span data-ttu-id="ad142-982">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ad142-982">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="ad142-983">(#4448)</span><span class="sxs-lookup"><span data-stu-id="ad142-983">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="ad142-984">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-984">Network</span></span>

* <span data-ttu-id="ad142-985">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="ad142-985">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="ad142-986">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="ad142-986">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-987">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-987">Resource</span></span>

* <span data-ttu-id="ad142-988">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="ad142-988">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="ad142-989">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="ad142-989">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="ad142-990">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="ad142-990">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="ad142-991">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="ad142-991">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-992">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-992">Sql</span></span>

* <span data-ttu-id="ad142-993">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="ad142-993">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="ad142-994">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="ad142-994">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="ad142-995">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="ad142-995">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-996">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-996">Storage</span></span>

* <span data-ttu-id="ad142-997">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ad142-997">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-998">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="ad142-998">Vm</span></span>

* <span data-ttu-id="ad142-999">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="ad142-999">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="ad142-1000">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1000">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="ad142-1001">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1001">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="ad142-1002">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1002">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="ad142-1003">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="ad142-1003">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="ad142-1004">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-1004">September 22, 2017</span></span>

<span data-ttu-id="ad142-1005">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="ad142-1005">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-1006">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-1006">Resource</span></span>

* <span data-ttu-id="ad142-1007">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="ad142-1007">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="ad142-1008">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="ad142-1008">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="ad142-1009">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="ad142-1009">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="ad142-1010">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1010">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="ad142-1011">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-1011">Network</span></span>

* <span data-ttu-id="ad142-1012">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="ad142-1012">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="ad142-1013">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="ad142-1013">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="ad142-1014">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="ad142-1014">Added `asg` application security group commands</span></span>
* <span data-ttu-id="ad142-1015">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="ad142-1015">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="ad142-1016">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ad142-1016">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ad142-1017">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ad142-1017">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="ad142-1018">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1018">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-1019">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-1019">Storage</span></span>

* <span data-ttu-id="ad142-1020">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="ad142-1020">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="ad142-1021">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="ad142-1021">Eventgrid</span></span>

* <span data-ttu-id="ad142-1022">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="ad142-1022">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-1023">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-1023">SQL</span></span>

* <span data-ttu-id="ad142-1024">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="ad142-1024">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="ad142-1025">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="ad142-1025">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="ad142-1026">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="ad142-1026">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="ad142-1027">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ad142-1027">Keyvault</span></span>

* <span data-ttu-id="ad142-1028">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="ad142-1028">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-1029">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-1029">VM</span></span>

* <span data-ttu-id="ad142-1030">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="ad142-1030">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="ad142-1031">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="ad142-1031">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="ad142-1032">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="ad142-1032">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="ad142-1033">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="ad142-1033">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="ad142-1034">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="ad142-1034">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="ad142-1035">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="ad142-1035">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-1036">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-1036">ACS</span></span>

* <span data-ttu-id="ad142-1037">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="ad142-1037">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-1038">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-1038">Appservice</span></span>

* <span data-ttu-id="ad142-1039">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="ad142-1039">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="ad142-1040">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="ad142-1040">Backup</span></span>

* <span data-ttu-id="ad142-1041">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="ad142-1041">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="ad142-1042">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-1042">September 11, 2017</span></span>

<span data-ttu-id="ad142-1043">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="ad142-1043">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="ad142-1044">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-1044">Core</span></span>

* <span data-ttu-id="ad142-1045">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="ad142-1045">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="ad142-1046">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="ad142-1046">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-1047">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-1047">Acs</span></span>

* <span data-ttu-id="ad142-1048">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1048">Added `acs list-locations` command</span></span>
* <span data-ttu-id="ad142-1049">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad142-1049">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-1050">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-1050">Appservice</span></span>

* <span data-ttu-id="ad142-1051">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="ad142-1051">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="ad142-1052">CDN</span><span class="sxs-lookup"><span data-stu-id="ad142-1052">CDN</span></span>

* <span data-ttu-id="ad142-1053">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1053">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="ad142-1054">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="ad142-1054">Extension</span></span>

* <span data-ttu-id="ad142-1055">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ad142-1055">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="ad142-1056">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ad142-1056">Keyvault</span></span>

* <span data-ttu-id="ad142-1057">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1057">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="ad142-1058">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-1058">Network</span></span>

* <span data-ttu-id="ad142-1059">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1059">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ad142-1060">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1060">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="ad142-1061">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1061">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="ad142-1062">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1062">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ad142-1063">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1063">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-1064">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-1064">Resource</span></span>

* <span data-ttu-id="ad142-1065">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1065">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="ad142-1066">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1066">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="ad142-1067">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="ad142-1067">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="ad142-1068">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="ad142-1068">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-1069">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-1069">SQL</span></span>

* <span data-ttu-id="ad142-1070">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1070">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-1071">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-1071">VM</span></span>

* <span data-ttu-id="ad142-1072">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="ad142-1072">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="ad142-1073">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="ad142-1073">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="ad142-1074">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1074">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="ad142-1075">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="ad142-1075">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="ad142-1076">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="ad142-1076">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="ad142-1077">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-1077">August 31, 2017</span></span>

<span data-ttu-id="ad142-1078">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="ad142-1078">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="ad142-1079">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ad142-1079">Keyvault</span></span>

* <span data-ttu-id="ad142-1080">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1080">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="ad142-1081">Sf</span><span class="sxs-lookup"><span data-stu-id="ad142-1081">Sf</span></span>

* <span data-ttu-id="ad142-1082">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="ad142-1082">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-1083">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-1083">Storage</span></span>

* <span data-ttu-id="ad142-1084">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="ad142-1084">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="ad142-1085">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="ad142-1085">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="ad142-1086">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-1086">August 28, 2017</span></span>

<span data-ttu-id="ad142-1087">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="ad142-1087">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="ad142-1088">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="ad142-1088">CLI</span></span>

* <span data-ttu-id="ad142-1089">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="ad142-1089">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-1090">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-1090">ACS</span></span>

* <span data-ttu-id="ad142-1091">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ad142-1091">Corrected preview regions</span></span>
* <span data-ttu-id="ad142-1092">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1092">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="ad142-1093">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="ad142-1093">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-1094">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-1094">Appservice</span></span>

* <span data-ttu-id="ad142-1095">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1095">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="ad142-1096">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1096">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="ad142-1097">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1097">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="ad142-1098">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="ad142-1098">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="ad142-1099">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="ad142-1099">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="ad142-1100">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ad142-1100">IoT</span></span>

* <span data-ttu-id="ad142-1101">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="ad142-1101">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="ad142-1102">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-1102">Network</span></span>

* <span data-ttu-id="ad142-1103">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1103">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="ad142-1104">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1104">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="ad142-1105">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1105">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="ad142-1106">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1106">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="ad142-1107">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1107">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="ad142-1108">Профиль</span><span class="sxs-lookup"><span data-stu-id="ad142-1108">Profile</span></span>

* <span data-ttu-id="ad142-1109">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="ad142-1109">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ad142-1110">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ad142-1110">Service Fabric</span></span>

* <span data-ttu-id="ad142-1111">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="ad142-1111">Preview release</span></span>
* <span data-ttu-id="ad142-1112">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="ad142-1112">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="ad142-1113">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="ad142-1113">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="ad142-1114">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1114">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-1115">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-1115">Storage</span></span>

* <span data-ttu-id="ad142-1116">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="ad142-1116">Enabled setting blob tier</span></span>
* <span data-ttu-id="ad142-1117">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="ad142-1117">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="ad142-1118">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1118">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="ad142-1119">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="ad142-1119">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="ad142-1120">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1120">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="ad142-1121">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1121">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-1122">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-1122">VM</span></span>

* <span data-ttu-id="ad142-1123">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1123">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="ad142-1124">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1124">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="ad142-1125">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="ad142-1125">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="ad142-1126">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="ad142-1126">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="ad142-1127">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="ad142-1127">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="ad142-1128">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1128">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="ad142-1129">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-1129">August 15, 2017</span></span>

<span data-ttu-id="ad142-1130">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="ad142-1130">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-1131">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-1131">ACS</span></span>

* <span data-ttu-id="ad142-1132">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="ad142-1132">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-1133">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-1133">Appservice</span></span>

* <span data-ttu-id="ad142-1134">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="ad142-1134">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="ad142-1135">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-1135">Event Grid</span></span>

* <span data-ttu-id="ad142-1136">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ad142-1136">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="ad142-1137">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-1137">August 11, 2017</span></span>

<span data-ttu-id="ad142-1138">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="ad142-1138">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-1139">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-1139">ACS</span></span>

* <span data-ttu-id="ad142-1140">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="ad142-1140">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="ad142-1141">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-1141">Batch</span></span>

* <span data-ttu-id="ad142-1142">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="ad142-1142">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="ad142-1143">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="ad142-1143">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="ad142-1144">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ad142-1144">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="ad142-1145">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="ad142-1145">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="ad142-1146">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="ad142-1146">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="ad142-1147">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="ad142-1147">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="ad142-1148">Компонент</span><span class="sxs-lookup"><span data-stu-id="ad142-1148">Component</span></span>

* <span data-ttu-id="ad142-1149">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="ad142-1149">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="ad142-1150">Контейнер</span><span class="sxs-lookup"><span data-stu-id="ad142-1150">Container</span></span>

* <span data-ttu-id="ad142-1151">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="ad142-1151">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="ad142-1152">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ad142-1152">Data Lake Store</span></span>

* <span data-ttu-id="ad142-1153">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="ad142-1153">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="ad142-1154">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-1154">Event Grid</span></span>

* <span data-ttu-id="ad142-1155">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="ad142-1155">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="ad142-1156">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-1156">Network</span></span>

* <span data-ttu-id="ad142-1157">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="ad142-1157">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="ad142-1158">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1158">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="ad142-1159">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1159">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="ad142-1160">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1160">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="ad142-1161">Профиль</span><span class="sxs-lookup"><span data-stu-id="ad142-1161">Profile</span></span>

* <span data-ttu-id="ad142-1162">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="ad142-1162">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-1163">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-1163">Storage</span></span>

* <span data-ttu-id="ad142-1164">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="ad142-1164">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-1165">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-1165">VM</span></span>

* <span data-ttu-id="ad142-1166">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="ad142-1166">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="ad142-1167">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1167">Exposed `list-skus` command</span></span>
* <span data-ttu-id="ad142-1168">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="ad142-1168">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="ad142-1169">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="ad142-1169">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="ad142-1170">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="ad142-1170">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="ad142-1171">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-1171">July 28, 2017</span></span>

<span data-ttu-id="ad142-1172">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="ad142-1172">Version 2.0.12</span></span>

* <span data-ttu-id="ad142-1173">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="ad142-1173">Added container commands</span></span>
* <span data-ttu-id="ad142-1174">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="ad142-1174">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="ad142-1175">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-1175">Core</span></span>

* <span data-ttu-id="ad142-1176">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="ad142-1176">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="ad142-1177">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="ad142-1177">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="ad142-1178">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="ad142-1178">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="ad142-1179">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="ad142-1179">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="ad142-1180">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="ad142-1180">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="ad142-1181">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="ad142-1181">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="ad142-1182">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="ad142-1182">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ad142-1183">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="ad142-1183">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="ad142-1184">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="ad142-1184">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="ad142-1185">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="ad142-1185">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="ad142-1186">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="ad142-1186">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="ad142-1187">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="ad142-1187">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="ad142-1188">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="ad142-1188">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="ad142-1189">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="ad142-1189">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="ad142-1190">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="ad142-1190">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="ad142-1191">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="ad142-1191">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="ad142-1192">ACR</span><span class="sxs-lookup"><span data-stu-id="ad142-1192">ACR</span></span>

* <span data-ttu-id="ad142-1193">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="ad142-1193">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="ad142-1194">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="ad142-1194">Support SKU update for managed registries</span></span>
* <span data-ttu-id="ad142-1195">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="ad142-1195">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="ad142-1196">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="ad142-1196">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="ad142-1197">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="ad142-1197">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="ad142-1198">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="ad142-1198">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-1199">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-1199">ACS</span></span>

* <span data-ttu-id="ad142-1200">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="ad142-1200">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-1201">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="ad142-1201">Appservice</span></span>

* <span data-ttu-id="ad142-1202">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="ad142-1202">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="ad142-1203">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="ad142-1203">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="ad142-1204">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1204">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="ad142-1205">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="ad142-1205">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="ad142-1206">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="ad142-1206">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="ad142-1207">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="ad142-1207">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="ad142-1208">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="ad142-1208">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="ad142-1209">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="ad142-1209">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="ad142-1210">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="ad142-1210">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="ad142-1211">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1211">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="ad142-1212">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="ad142-1212">Batch</span></span>

* <span data-ttu-id="ad142-1213">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="ad142-1213">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="ad142-1214">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1214">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="ad142-1215">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1215">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="ad142-1216">CDN</span><span class="sxs-lookup"><span data-stu-id="ad142-1216">CDN</span></span>

* <span data-ttu-id="ad142-1217">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="ad142-1217">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="ad142-1218">Облако</span><span class="sxs-lookup"><span data-stu-id="ad142-1218">Cloud</span></span>

* <span data-ttu-id="ad142-1219">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="ad142-1219">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="ad142-1220">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="ad142-1220">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="ad142-1221">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="ad142-1221">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="ad142-1222">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="ad142-1222">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="ad142-1223">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1223">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ad142-1224">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ad142-1224">CosmosDB</span></span>

* <span data-ttu-id="ad142-1225">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="ad142-1225">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="ad142-1226">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="ad142-1226">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ad142-1227">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ad142-1227">Data Lake Analytics</span></span>

* <span data-ttu-id="ad142-1228">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1228">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="ad142-1229">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1229">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="ad142-1230">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1230">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ad142-1231">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ad142-1231">Data Lake Store</span></span>

* <span data-ttu-id="ad142-1232">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1232">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="ad142-1233">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="ad142-1233">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="ad142-1234">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1234">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="ad142-1235">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ad142-1235">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="ad142-1236">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="ad142-1236">Interactive</span></span>

* <span data-ttu-id="ad142-1237">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="ad142-1237">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="ad142-1238">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="ad142-1238">Increased test coverage</span></span>
* <span data-ttu-id="ad142-1239">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="ad142-1239">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="ad142-1240">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="ad142-1240">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="ad142-1241">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="ad142-1241">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="ad142-1242">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="ad142-1242">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="ad142-1243">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="ad142-1243">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="ad142-1244">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1244">Added `--progress` flag</span></span>
* <span data-ttu-id="ad142-1245">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1245">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="ad142-1246">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="ad142-1246">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="ad142-1247">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="ad142-1247">IoT</span></span>

* <span data-ttu-id="ad142-1248">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="ad142-1248">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="ad142-1249">(3934).</span><span class="sxs-lookup"><span data-stu-id="ad142-1249">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="ad142-1250">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ad142-1250">Key vault</span></span>

* <span data-ttu-id="ad142-1251">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="ad142-1251">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="ad142-1252">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1252">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="ad142-1253">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="ad142-1253">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ad142-1254">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="ad142-1254">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="ad142-1255">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1255">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="ad142-1256">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="ad142-1256">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="ad142-1257">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="ad142-1257">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="ad142-1258">(3307).</span><span class="sxs-lookup"><span data-stu-id="ad142-1258">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="ad142-1259">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ad142-1259">Lab</span></span>

* <span data-ttu-id="ad142-1260">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1260">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="ad142-1261">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1261">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="ad142-1262">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ad142-1262">Monitor</span></span>

* <span data-ttu-id="ad142-1263">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="ad142-1263">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="ad142-1264">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1264">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="ad142-1265">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1265">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="ad142-1266">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1266">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="ad142-1267">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1267">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="ad142-1268">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="ad142-1268">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="ad142-1269">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="ad142-1269">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="ad142-1270">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="ad142-1270">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="ad142-1271">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="ad142-1271">`location` no longer required</span></span>
  * <span data-ttu-id="ad142-1272">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="ad142-1272">Add name and ID support for target</span></span>
  * <span data-ttu-id="ad142-1273">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="ad142-1273">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="ad142-1274">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="ad142-1274">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="ad142-1275">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="ad142-1275">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="ad142-1276">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="ad142-1276">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="ad142-1277">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1277">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="ad142-1278">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1278">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="ad142-1279">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-1279">Network</span></span>

* <span data-ttu-id="ad142-1280">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1280">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="ad142-1281">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1281">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="ad142-1282">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="ad142-1282">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="ad142-1283">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1283">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="ad142-1284">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1284">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="ad142-1285">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1285">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="ad142-1286">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1286">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="ad142-1287">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1287">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="ad142-1288">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1288">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="ad142-1289">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1289">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="ad142-1290">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1290">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="ad142-1291">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1291">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="ad142-1292">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1292">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="ad142-1293">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1293">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="ad142-1294">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1294">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="ad142-1295">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1295">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="ad142-1296">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="ad142-1296">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="ad142-1297">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1297">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="ad142-1298">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1298">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="ad142-1299">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1299">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="ad142-1300">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1300">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="ad142-1301">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1301">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="ad142-1302">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1302">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="ad142-1303">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="ad142-1303">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="ad142-1304">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="ad142-1304">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="ad142-1305">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="ad142-1305">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="ad142-1306">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="ad142-1306">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="ad142-1307">Профиль</span><span class="sxs-lookup"><span data-stu-id="ad142-1307">Profile</span></span>

* <span data-ttu-id="ad142-1308">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="ad142-1308">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="ad142-1309">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ad142-1309">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="ad142-1310">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="ad142-1310">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="ad142-1311">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="ad142-1311">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="ad142-1312">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="ad142-1312">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="ad142-1313">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="ad142-1313">RDBMS</span></span>

* <span data-ttu-id="ad142-1314">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="ad142-1314">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="ad142-1315">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="ad142-1315">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="ad142-1316">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="ad142-1316">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="ad142-1317">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="ad142-1317">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-1318">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-1318">Resource</span></span>

* <span data-ttu-id="ad142-1319">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1319">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="ad142-1320">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1320">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="ad142-1321">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1321">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="ad142-1322">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1322">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="ad142-1323">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="ad142-1323">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="ad142-1324">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1324">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="ad142-1325">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="ad142-1325">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="ad142-1326">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1326">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="ad142-1327">Роль</span><span class="sxs-lookup"><span data-stu-id="ad142-1327">Role</span></span>

* <span data-ttu-id="ad142-1328">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="ad142-1328">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="ad142-1329">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="ad142-1329">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="ad142-1330">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="ad142-1330">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="ad142-1331">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="ad142-1331">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="ad142-1332">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1332">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="ad142-1333">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="ad142-1333">Service Fabric</span></span>
* <span data-ttu-id="ad142-1334">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="ad142-1334">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="ad142-1335">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="ad142-1335">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="ad142-1336">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="ad142-1336">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-1337">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-1337">SQL</span></span>

* <span data-ttu-id="ad142-1338">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1338">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="ad142-1339">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1339">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="ad142-1340">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1340">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-1341">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-1341">Storage</span></span>

* <span data-ttu-id="ad142-1342">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="ad142-1342">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="ad142-1343">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="ad142-1343">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="ad142-1344">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="ad142-1344">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="ad142-1345">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="ad142-1345">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="ad142-1346">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="ad142-1346">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="ad142-1347">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="ad142-1347">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-1348">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-1348">VM</span></span>

* <span data-ttu-id="ad142-1349">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="ad142-1349">Support configuring nsg</span></span>
* <span data-ttu-id="ad142-1350">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="ad142-1350">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="ad142-1351">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="ad142-1351">Support managed service identities</span></span>
* <span data-ttu-id="ad142-1352">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1352">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="ad142-1353">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="ad142-1353">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="ad142-1354">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-1354">May 10, 2017</span></span>

<span data-ttu-id="ad142-1355">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="ad142-1355">Version 2.0.6</span></span>

* <span data-ttu-id="ad142-1356">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="ad142-1356">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="ad142-1357">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="ad142-1357">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="ad142-1358">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ad142-1358">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="ad142-1359">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="ad142-1359">Include Cognitive Services module</span></span>
* <span data-ttu-id="ad142-1360">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="ad142-1360">Include Service Fabric module</span></span>
* <span data-ttu-id="ad142-1361">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="ad142-1361">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="ad142-1362">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="ad142-1362">Add support for CDN commands</span></span>
* <span data-ttu-id="ad142-1363">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="ad142-1363">Remove Container module</span></span>
* <span data-ttu-id="ad142-1364">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1364">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="ad142-1365">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1365">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="ad142-1366">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-1366">Core</span></span>

* <span data-ttu-id="ad142-1367">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="ad142-1367">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="ad142-1368">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1368">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="ad142-1369">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1369">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="ad142-1370">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1370">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="ad142-1371">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1371">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="ad142-1372">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1372">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="ad142-1373">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1373">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="ad142-1374">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1374">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="ad142-1375">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1375">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="ad142-1376">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="ad142-1376">core: Improved performance</span></span>
* <span data-ttu-id="ad142-1377">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="ad142-1377">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="ad142-1378">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="ad142-1378">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-1379">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-1379">ACS</span></span>

* <span data-ttu-id="ad142-1380">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="ad142-1380">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="ad142-1381">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="ad142-1381">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="ad142-1382">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="ad142-1382">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="ad142-1383">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1383">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-1384">AppService</span><span class="sxs-lookup"><span data-stu-id="ad142-1384">AppService</span></span>

* <span data-ttu-id="ad142-1385">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="ad142-1385">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="ad142-1386">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="ad142-1386">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="ad142-1387">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="ad142-1387">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="ad142-1388">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="ad142-1388">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="ad142-1389">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="ad142-1389">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="ad142-1390">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1390">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="ad142-1391">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="ad142-1391">support slot swap with preview</span></span>
* <span data-ttu-id="ad142-1392">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1392">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="ad142-1393">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1393">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="ad142-1394">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="ad142-1394">CosmosDB</span></span>

* <span data-ttu-id="ad142-1395">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="ad142-1395">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="ad142-1396">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="ad142-1396">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="ad142-1397">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="ad142-1397">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="ad142-1398">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="ad142-1398">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="ad142-1399">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="ad142-1399">Data Lake Analytics</span></span>

* <span data-ttu-id="ad142-1400">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="ad142-1400">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="ad142-1401">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="ad142-1401">Add support for new catalog item type: package.</span></span> <span data-ttu-id="ad142-1402">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1402">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="ad142-1403">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="ad142-1403">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="ad142-1404">Таблица</span><span class="sxs-lookup"><span data-stu-id="ad142-1404">Table</span></span>
  * <span data-ttu-id="ad142-1405">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="ad142-1405">Table valued function</span></span>
  * <span data-ttu-id="ad142-1406">Просмотр</span><span class="sxs-lookup"><span data-stu-id="ad142-1406">View</span></span>
  * <span data-ttu-id="ad142-1407">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="ad142-1407">Table Statistics.</span></span> <span data-ttu-id="ad142-1408">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="ad142-1408">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="ad142-1409">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="ad142-1409">Data Lake Store</span></span>

* <span data-ttu-id="ad142-1410">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="ad142-1410">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="ad142-1411">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1411">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="ad142-1412">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="ad142-1412">missed help for access show.</span></span> <span data-ttu-id="ad142-1413">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="ad142-1413">adding it.</span></span> <span data-ttu-id="ad142-1414">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="ad142-1414">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="ad142-1415">Поиск</span><span class="sxs-lookup"><span data-stu-id="ad142-1415">Find</span></span>

* <span data-ttu-id="ad142-1416">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="ad142-1416">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="ad142-1417">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="ad142-1417">KeyVault</span></span>

* <span data-ttu-id="ad142-1418">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="ad142-1418">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="ad142-1419">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="ad142-1419">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="ad142-1420">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="ad142-1420">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="ad142-1421">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="ad142-1421">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="ad142-1422">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1422">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="ad142-1423">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="ad142-1423">Lab</span></span>

* <span data-ttu-id="ad142-1424">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ad142-1424">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="ad142-1425">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ad142-1425">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="ad142-1426">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ad142-1426">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="ad142-1427">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ad142-1427">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="ad142-1428">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="ad142-1428">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="ad142-1429">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="ad142-1429">Monitor</span></span>

* <span data-ttu-id="ad142-1430">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1430">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="ad142-1431">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1431">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="ad142-1432">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-1432">Network</span></span>

* <span data-ttu-id="ad142-1433">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1433">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="ad142-1434">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1434">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="ad142-1435">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ad142-1435">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="ad142-1436">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="ad142-1436">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="ad142-1437">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="ad142-1437">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="ad142-1438">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="ad142-1438">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="ad142-1439">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="ad142-1439">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="ad142-1440">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="ad142-1440">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="ad142-1441">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1441">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="ad142-1442">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="ad142-1442">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="ad142-1443">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1443">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="ad142-1444">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1444">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="ad142-1445">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="ad142-1445">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="ad142-1446">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="ad142-1446">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="ad142-1447">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="ad142-1447">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="ad142-1448">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="ad142-1448">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="ad142-1449">Профиль</span><span class="sxs-lookup"><span data-stu-id="ad142-1449">Profile</span></span>

* <span data-ttu-id="ad142-1450">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1450">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="ad142-1451">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1451">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="ad142-1452">Redis</span><span class="sxs-lookup"><span data-stu-id="ad142-1452">Redis</span></span>

* <span data-ttu-id="ad142-1453">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="ad142-1453">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="ad142-1454">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="ad142-1454">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="ad142-1455">Ресурс</span><span class="sxs-lookup"><span data-stu-id="ad142-1455">Resource</span></span>

* <span data-ttu-id="ad142-1456">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1456">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="ad142-1457">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1457">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="ad142-1458">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1458">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="ad142-1459">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="ad142-1459">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="ad142-1460">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="ad142-1460">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="ad142-1461">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="ad142-1461">Add docs for az lock update.</span></span> <span data-ttu-id="ad142-1462">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="ad142-1462">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="ad142-1463">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="ad142-1463">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="ad142-1464">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="ad142-1464">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="ad142-1465">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="ad142-1465">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="ad142-1466">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="ad142-1466">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="ad142-1467">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1467">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="ad142-1468">Роль</span><span class="sxs-lookup"><span data-stu-id="ad142-1468">Role</span></span>

* <span data-ttu-id="ad142-1469">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1469">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="ad142-1470">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1470">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="ad142-1471">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1471">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="ad142-1472">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="ad142-1472">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="ad142-1473">SQL</span><span class="sxs-lookup"><span data-stu-id="ad142-1473">SQL</span></span>

* <span data-ttu-id="ad142-1474">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="ad142-1474">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="ad142-1475">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1475">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="ad142-1476">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-1476">Storage</span></span>

* <span data-ttu-id="ad142-1477">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1477">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="ad142-1478">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="ad142-1478">Add support for incremental blob copy</span></span>
* <span data-ttu-id="ad142-1479">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="ad142-1479">Add support for large block blob upload</span></span>
* <span data-ttu-id="ad142-1480">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ad142-1480">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-1481">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-1481">VM</span></span>

* <span data-ttu-id="ad142-1482">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="ad142-1482">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="ad142-1483">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="ad142-1483">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="ad142-1484">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="ad142-1484">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="ad142-1485">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="ad142-1485">az vm/vmss disk</span></span>
  3. <span data-ttu-id="ad142-1486">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="ad142-1486">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="ad142-1487">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="ad142-1487">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="ad142-1488">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1488">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="ad142-1489">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-1489">April 3, 2017</span></span>

<span data-ttu-id="ad142-1490">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="ad142-1490">Version 2.0.2</span></span>

<span data-ttu-id="ad142-1491">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="ad142-1491">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="ad142-1492">Core</span><span class="sxs-lookup"><span data-stu-id="ad142-1492">Core</span></span>

* <span data-ttu-id="ad142-1493">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad142-1493">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="ad142-1494">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1494">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="ad142-1495">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1495">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="ad142-1496">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1496">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ad142-1497">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1497">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="ad142-1498">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="ad142-1498">Add prompting for missing template parameters.</span></span> <span data-ttu-id="ad142-1499">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1499">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="ad142-1500">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="ad142-1500">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="ad142-1501">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="ad142-1501">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="ad142-1502">ACS</span><span class="sxs-lookup"><span data-stu-id="ad142-1502">ACS</span></span>

* <span data-ttu-id="ad142-1503">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1503">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="ad142-1504">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="ad142-1504">Add support for ssh key password prompting.</span></span> <span data-ttu-id="ad142-1505">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1505">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="ad142-1506">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="ad142-1506">Add support for windows clusters.</span></span> <span data-ttu-id="ad142-1507">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1507">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="ad142-1508">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="ad142-1508">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="ad142-1509">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1509">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="ad142-1510">AppService</span><span class="sxs-lookup"><span data-stu-id="ad142-1510">AppService</span></span>

* <span data-ttu-id="ad142-1511">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1511">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="ad142-1512">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1512">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="ad142-1513">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1513">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="ad142-1514">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1514">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="ad142-1515">Data Lake</span><span class="sxs-lookup"><span data-stu-id="ad142-1515">DataLake</span></span>

* <span data-ttu-id="ad142-1516">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="ad142-1516">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="ad142-1517">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="ad142-1517">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="ad142-1518">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="ad142-1518">DocuemntDB</span></span>

* <span data-ttu-id="ad142-1519">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1519">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="ad142-1520">ВМ</span><span class="sxs-lookup"><span data-stu-id="ad142-1520">VM</span></span>

* <span data-ttu-id="ad142-1521">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1521">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="ad142-1522">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1522">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="ad142-1523">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1523">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="ad142-1524">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1524">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="ad142-1525">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1525">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="ad142-1526">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1526">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="ad142-1527">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="ad142-1527">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="ad142-1528">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="ad142-1528">February 27, 2017</span></span>

<span data-ttu-id="ad142-1529">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="ad142-1529">Version 2.0.0</span></span>

<span data-ttu-id="ad142-1530">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="ad142-1530">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="ad142-1531">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="ad142-1531">Container Service (acs)</span></span>
- <span data-ttu-id="ad142-1532">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="ad142-1532">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="ad142-1533">Сеть</span><span class="sxs-lookup"><span data-stu-id="ad142-1533">Networking</span></span>
- <span data-ttu-id="ad142-1534">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="ad142-1534">Storage</span></span>

<span data-ttu-id="ad142-1535">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1535">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="ad142-1536">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="ad142-1536">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="ad142-1537">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="ad142-1537">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="ad142-1538">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="ad142-1538">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="ad142-1539">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="ad142-1539">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="ad142-1540">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="ad142-1540">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="ad142-1541">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="ad142-1541">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="ad142-1542">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="ad142-1542">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="ad142-1543">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="ad142-1543">Provide feedback from the command line with the `az feedback` command</span></span>

