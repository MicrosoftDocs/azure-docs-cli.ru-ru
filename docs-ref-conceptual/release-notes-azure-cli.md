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
ms.openlocfilehash: b44a387a144b9d7daca8d87309d8a5e1a47b078a
ms.sourcegitcommit: 64f2c628e83d687d0e172c01f13d71c8c39a8040
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2018
ms.locfileid: "38967883"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="f541c-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="f541c-103">Azure CLI 2.0 release notes</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f541c-104">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-104">July 3, 2018</span></span>

<span data-ttu-id="f541c-105">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="f541c-105">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="f541c-106">AKS</span><span class="sxs-lookup"><span data-stu-id="f541c-106">AKS</span></span>

* <span data-ttu-id="f541c-107">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="f541c-107">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="f541c-108">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-108">July 3, 2018</span></span>

<span data-ttu-id="f541c-109">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="f541c-109">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="f541c-110">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-110">Core</span></span>

* <span data-ttu-id="f541c-111">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="f541c-111">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="f541c-112">ACR</span><span class="sxs-lookup"><span data-stu-id="f541c-112">ACR</span></span>

* <span data-ttu-id="f541c-113">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="f541c-113">Added polling build status</span></span>
* <span data-ttu-id="f541c-114">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="f541c-114">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="f541c-115">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="f541c-115">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-116">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-116">ACS</span></span>

* <span data-ttu-id="f541c-117">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f541c-117">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="f541c-118">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f541c-118">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="f541c-119">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="f541c-119">Updated options for `aks browse` command.</span></span> <span data-ttu-id="f541c-120">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="f541c-120">Added `--listen-port` support</span></span>
* <span data-ttu-id="f541c-121">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="f541c-121">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="f541c-122">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="f541c-122">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="f541c-123">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="f541c-123">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-124">AppService</span><span class="sxs-lookup"><span data-stu-id="f541c-124">AppService</span></span>

* <span data-ttu-id="f541c-125">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="f541c-125">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="f541c-126">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="f541c-126">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="f541c-127">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="f541c-127">Backup</span></span>

* <span data-ttu-id="f541c-128">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="f541c-128">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="f541c-129">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f541c-129">BatchAI</span></span>

* <span data-ttu-id="f541c-130">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="f541c-130">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="f541c-131">Облако</span><span class="sxs-lookup"><span data-stu-id="f541c-131">Cloud</span></span>

* <span data-ttu-id="f541c-132">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="f541c-132">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="f541c-133">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f541c-133">Container</span></span>

* <span data-ttu-id="f541c-134">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="f541c-134">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="f541c-135">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="f541c-135">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="f541c-136">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="f541c-136">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="f541c-137">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f541c-137">Extension</span></span>

* <span data-ttu-id="f541c-138">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="f541c-138">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="f541c-139">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-139">Network</span></span>

* <span data-ttu-id="f541c-140">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="f541c-140">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="f541c-141">Rdbms</span><span class="sxs-lookup"><span data-stu-id="f541c-141">Rdbms</span></span>

* <span data-ttu-id="f541c-142">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="f541c-142">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-143">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-143">Resource</span></span>

* <span data-ttu-id="f541c-144">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="f541c-144">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-145">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-145">VM</span></span>

* <span data-ttu-id="f541c-146">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="f541c-146">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="f541c-147">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-147">June 25, 2018</span></span>

<span data-ttu-id="f541c-148">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="f541c-148">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="f541c-149">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="f541c-149">CLI</span></span>

* <span data-ttu-id="f541c-150">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="f541c-150">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="f541c-151">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-151">June 19, 2018</span></span>

<span data-ttu-id="f541c-152">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="f541c-152">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="f541c-153">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-153">Core</span></span>

* <span data-ttu-id="f541c-154">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="f541c-154">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="f541c-155">ACR</span><span class="sxs-lookup"><span data-stu-id="f541c-155">ACR</span></span>

* <span data-ttu-id="f541c-156">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="f541c-156">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="f541c-157">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="f541c-157">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-158">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-158">ACS</span></span>

* <span data-ttu-id="f541c-159">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="f541c-159">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="f541c-160">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-160">Added `--update` support</span></span>
* <span data-ttu-id="f541c-161">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="f541c-161">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="f541c-162">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="f541c-162">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="f541c-163">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="f541c-163">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="f541c-164">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="f541c-164">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="f541c-165">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="f541c-165">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="f541c-166">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="f541c-166">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-167">AppService</span><span class="sxs-lookup"><span data-stu-id="f541c-167">AppService</span></span>

* <span data-ttu-id="f541c-168">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="f541c-168">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="f541c-169">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f541c-169">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="f541c-170">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f541c-170">Batch</span></span>

* <span data-ttu-id="f541c-171">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="f541c-171">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f541c-172">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f541c-172">Batch AI</span></span>

* <span data-ttu-id="f541c-173">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="f541c-173">Added support for workspaces.</span></span> <span data-ttu-id="f541c-174">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f541c-174">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="f541c-175">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="f541c-175">Added support for experiments.</span></span> <span data-ttu-id="f541c-176">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="f541c-176">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="f541c-177">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="f541c-177">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="f541c-178">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="f541c-178">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="f541c-179">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="f541c-179">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="f541c-180">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="f541c-180">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="f541c-181">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="f541c-181">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="f541c-182">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="f541c-182">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="f541c-183">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-183">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="f541c-184">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="f541c-184">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="f541c-185">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-185">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="f541c-186">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="f541c-186">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="f541c-187">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="f541c-187">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="f541c-188">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="f541c-188">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="f541c-189">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-189">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="f541c-190">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="f541c-190">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="f541c-191">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="f541c-191">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="f541c-192">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="f541c-192">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="f541c-193">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="f541c-193">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="f541c-194">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="f541c-194">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="f541c-195">Карты</span><span class="sxs-lookup"><span data-stu-id="f541c-195">Maps</span></span>

* <span data-ttu-id="f541c-196">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="f541c-196">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="f541c-197">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-197">Network</span></span>

* <span data-ttu-id="f541c-198">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="f541c-198">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="f541c-199">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="f541c-199">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="f541c-200">#6502</span><span class="sxs-lookup"><span data-stu-id="f541c-200">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="f541c-201">Резервирование</span><span class="sxs-lookup"><span data-stu-id="f541c-201">Reservations</span></span>

* <span data-ttu-id="f541c-202">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-202">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="f541c-203">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-203">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="f541c-204">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="f541c-204">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="f541c-205">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="f541c-205">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="f541c-206">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="f541c-206">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="f541c-207">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-207">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="f541c-208">Роль</span><span class="sxs-lookup"><span data-stu-id="f541c-208">Role</span></span>

* <span data-ttu-id="f541c-209">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="f541c-209">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-210">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-210">SQL</span></span>

* <span data-ttu-id="f541c-211">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="f541c-211">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-212">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-212">Storage</span></span>

* <span data-ttu-id="f541c-213">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="f541c-213">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-214">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-214">VM</span></span>

* <span data-ttu-id="f541c-215">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-215">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="f541c-216">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="f541c-216">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="f541c-217">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="f541c-217">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f541c-218">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-218">June 13, 2018</span></span>

<span data-ttu-id="f541c-219">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="f541c-219">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="f541c-220">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-220">Core</span></span>

* <span data-ttu-id="f541c-221">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="f541c-221">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="f541c-222">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-222">June 13, 2018</span></span>

<span data-ttu-id="f541c-223">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="f541c-223">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="f541c-224">AKS</span><span class="sxs-lookup"><span data-stu-id="f541c-224">AKS</span></span>

* <span data-ttu-id="f541c-225">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="f541c-225">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="f541c-226">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="f541c-226">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="f541c-227">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="f541c-227">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="f541c-228">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="f541c-228">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="f541c-229">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f541c-229">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-230">AppService</span><span class="sxs-lookup"><span data-stu-id="f541c-230">AppService</span></span>

* <span data-ttu-id="f541c-231">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="f541c-231">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f541c-232">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-232">June 5, 2018</span></span>

<span data-ttu-id="f541c-233">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="f541c-233">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="f541c-234">Interactive</span><span class="sxs-lookup"><span data-stu-id="f541c-234">Interactive</span></span>

* <span data-ttu-id="f541c-235">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="f541c-235">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="f541c-236">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-236">June 5, 2018</span></span>

<span data-ttu-id="f541c-237">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="f541c-237">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="f541c-238">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-238">Core</span></span>

* <span data-ttu-id="f541c-239">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="f541c-239">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="f541c-240">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="f541c-240">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="f541c-241">ACR</span><span class="sxs-lookup"><span data-stu-id="f541c-241">ACR</span></span>

* <span data-ttu-id="f541c-242">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="f541c-242">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="f541c-243">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="f541c-243">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="f541c-244">AKS</span><span class="sxs-lookup"><span data-stu-id="f541c-244">AKS</span></span>

* <span data-ttu-id="f541c-245">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="f541c-245">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="f541c-246">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f541c-246">Batch</span></span>

* <span data-ttu-id="f541c-247">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="f541c-247">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="f541c-248">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f541c-248">IOT</span></span>

* <span data-ttu-id="f541c-249">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="f541c-249">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="f541c-250">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-250">Network</span></span>

* <span data-ttu-id="f541c-251">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="f541c-251">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="f541c-252">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="f541c-252">Policy Insights</span></span>

* <span data-ttu-id="f541c-253">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f541c-253">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="f541c-254">ARM</span><span class="sxs-lookup"><span data-stu-id="f541c-254">ARM</span></span>

* <span data-ttu-id="f541c-255">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="f541c-255">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-256">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-256">SQL</span></span>

* <span data-ttu-id="f541c-257">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="f541c-257">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="f541c-258">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="f541c-258">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="f541c-259">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-259">Storage</span></span>

* <span data-ttu-id="f541c-260">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="f541c-260">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-261">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-261">VM</span></span>

* <span data-ttu-id="f541c-262">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="f541c-262">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="f541c-263">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-263">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="f541c-264">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-264">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="f541c-265">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-265">May 22, 2018</span></span>

<span data-ttu-id="f541c-266">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="f541c-266">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="f541c-267">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-267">Core</span></span>

* <span data-ttu-id="f541c-268">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="f541c-268">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-269">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-269">ACS</span></span>

* <span data-ttu-id="f541c-270">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="f541c-270">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="f541c-271">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="f541c-271">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-272">AppService</span><span class="sxs-lookup"><span data-stu-id="f541c-272">AppService</span></span>

* <span data-ttu-id="f541c-273">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="f541c-273">Improved generic update commands</span></span>
* <span data-ttu-id="f541c-274">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="f541c-274">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="f541c-275">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f541c-275">Container</span></span>

* <span data-ttu-id="f541c-276">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="f541c-276">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="f541c-277">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f541c-277">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f541c-278">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f541c-278">Extension</span></span>

* <span data-ttu-id="f541c-279">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="f541c-279">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="f541c-280">Interactive</span><span class="sxs-lookup"><span data-stu-id="f541c-280">Interactive</span></span>

* <span data-ttu-id="f541c-281">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="f541c-281">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="f541c-282">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="f541c-282">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="f541c-283">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f541c-283">KeyVault</span></span>

* <span data-ttu-id="f541c-284">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="f541c-284">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="f541c-285">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-285">Network</span></span>

* <span data-ttu-id="f541c-286">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="f541c-286">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="f541c-287">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="f541c-287">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-288">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-288">SQL</span></span>

* <span data-ttu-id="f541c-289">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="f541c-289">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="f541c-290">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="f541c-290">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="f541c-291">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="f541c-291">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="f541c-292">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="f541c-292">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="f541c-293">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="f541c-293">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="f541c-294">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="f541c-294">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="f541c-295">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="f541c-295">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="f541c-296">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f541c-296">`edition`.</span></span> <span data-ttu-id="f541c-297">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="f541c-297">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="f541c-298">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="f541c-298">`elasticPoolName`.</span></span> <span data-ttu-id="f541c-299">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="f541c-299">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="f541c-300">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="f541c-300">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="f541c-301">`edition`.</span><span class="sxs-lookup"><span data-stu-id="f541c-301">`edition`.</span></span> <span data-ttu-id="f541c-302">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="f541c-302">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="f541c-303">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="f541c-303">`dtu`.</span></span> <span data-ttu-id="f541c-304">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="f541c-304">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="f541c-305">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="f541c-305">`databaseDtuMin`.</span></span> <span data-ttu-id="f541c-306">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="f541c-306">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="f541c-307">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="f541c-307">`databaseDtuMax`.</span></span> <span data-ttu-id="f541c-308">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="f541c-308">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="f541c-309">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="f541c-309">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="f541c-310">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="f541c-310">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-311">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-311">Storage</span></span>

* <span data-ttu-id="f541c-312">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="f541c-312">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="f541c-313">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="f541c-313">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-314">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-314">VM</span></span>

* <span data-ttu-id="f541c-315">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-315">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="f541c-316">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="f541c-316">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="f541c-317">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="f541c-317">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="f541c-318">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="f541c-318">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="f541c-319">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-319">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="f541c-320">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-320">May 7, 2018</span></span>

<span data-ttu-id="f541c-321">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="f541c-321">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="f541c-322">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-322">Core</span></span>

* <span data-ttu-id="f541c-323">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="f541c-323">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="f541c-324">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="f541c-324">Added limited support for positional arguments</span></span>
* <span data-ttu-id="f541c-325">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f541c-325">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="f541c-326">#5591</span><span class="sxs-lookup"><span data-stu-id="f541c-326">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="f541c-327">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f541c-327">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="f541c-328">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="f541c-328">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="f541c-329">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="f541c-329">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="f541c-330">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="f541c-330">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="f541c-331">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="f541c-331">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="f541c-332">ACR</span><span class="sxs-lookup"><span data-stu-id="f541c-332">ACR</span></span>

* <span data-ttu-id="f541c-333">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="f541c-333">Added ACR Build commands</span></span>
* <span data-ttu-id="f541c-334">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="f541c-334">Improved resource not found error messages</span></span>
* <span data-ttu-id="f541c-335">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="f541c-335">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="f541c-336">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="f541c-336">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="f541c-337">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="f541c-337">Improved repository commands error messages</span></span>
* <span data-ttu-id="f541c-338">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="f541c-338">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-339">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-339">ACS</span></span>

* <span data-ttu-id="f541c-340">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="f541c-340">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="f541c-341">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="f541c-341">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="f541c-342">AMS</span><span class="sxs-lookup"><span data-stu-id="f541c-342">AMS</span></span>

* <span data-ttu-id="f541c-343">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="f541c-343">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-344">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-344">Appservice</span></span>

* <span data-ttu-id="f541c-345">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="f541c-345">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="f541c-346">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-346">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="f541c-347">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="f541c-347">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="f541c-348">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f541c-348">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="f541c-349">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f541c-349">Batch AI</span></span>

* <span data-ttu-id="f541c-350">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="f541c-350">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f541c-351">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f541c-351">Cognitive Services</span></span>

* <span data-ttu-id="f541c-352">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="f541c-352">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="f541c-353">Потребление</span><span class="sxs-lookup"><span data-stu-id="f541c-353">Consumption</span></span>

* <span data-ttu-id="f541c-354">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="f541c-354">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="f541c-355">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f541c-355">Container</span></span>

* <span data-ttu-id="f541c-356">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="f541c-356">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="f541c-357">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="f541c-357">Cosmos DB</span></span>

* <span data-ttu-id="f541c-358">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f541c-358">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="f541c-359">DMS</span><span class="sxs-lookup"><span data-stu-id="f541c-359">DMS</span></span>

* <span data-ttu-id="f541c-360">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="f541c-360">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="f541c-361">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f541c-361">Extension</span></span>

* <span data-ttu-id="f541c-362">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="f541c-362">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="f541c-363">Interactive</span><span class="sxs-lookup"><span data-stu-id="f541c-363">Interactive</span></span>

* <span data-ttu-id="f541c-364">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="f541c-364">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="f541c-365">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="f541c-365">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="f541c-366">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="f541c-366">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="f541c-367">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="f541c-367">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="f541c-368">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="f541c-368">Lab</span></span>

* <span data-ttu-id="f541c-369">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="f541c-369">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="f541c-370">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-370">Network</span></span>

* <span data-ttu-id="f541c-371">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="f541c-371">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="f541c-372">Профиль</span><span class="sxs-lookup"><span data-stu-id="f541c-372">Profile</span></span>

* <span data-ttu-id="f541c-373">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-373">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="f541c-374">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="f541c-374">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="f541c-375">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="f541c-375">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="f541c-376">Redis</span><span class="sxs-lookup"><span data-stu-id="f541c-376">Redis</span></span>

* <span data-ttu-id="f541c-377">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-377">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="f541c-378">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="f541c-378">Deprecated `redis list-all`.</span></span> <span data-ttu-id="f541c-379">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="f541c-379">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="f541c-380">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="f541c-380">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="f541c-381">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="f541c-381">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="f541c-382">Роль</span><span class="sxs-lookup"><span data-stu-id="f541c-382">Role</span></span>

* <span data-ttu-id="f541c-383">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="f541c-383">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-384">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-384">Storage</span></span>

* <span data-ttu-id="f541c-385">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="f541c-385">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="f541c-386">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="f541c-386">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="f541c-387">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="f541c-387">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="f541c-388">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="f541c-388">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="f541c-389">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="f541c-389">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-390">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-390">VM</span></span>

* <span data-ttu-id="f541c-391">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="f541c-391">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="f541c-392">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="f541c-392">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="f541c-393">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="f541c-393">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="f541c-394">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="f541c-394">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="f541c-395">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="f541c-395">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="f541c-396">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="f541c-396">Added write accelerator support</span></span>
* <span data-ttu-id="f541c-397">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="f541c-397">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="f541c-398">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="f541c-398">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="f541c-399">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="f541c-399">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="f541c-400">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-400">April 10, 2018</span></span>

<span data-ttu-id="f541c-401">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="f541c-401">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="f541c-402">ACR</span><span class="sxs-lookup"><span data-stu-id="f541c-402">ACR</span></span>

* <span data-ttu-id="f541c-403">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="f541c-403">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-404">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-404">ACS</span></span>

* <span data-ttu-id="f541c-405">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="f541c-405">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-406">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-406">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="f541c-408">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="f541c-408">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="f541c-409">Batch AI</span><span class="sxs-lookup"><span data-stu-id="f541c-409">BatchAI</span></span>

* <span data-ttu-id="f541c-410">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="f541c-410">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="f541c-411">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="f541c-411">Job level mounting</span></span>
 - <span data-ttu-id="f541c-412">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="f541c-412">Environment variables with secret values</span></span>
 - <span data-ttu-id="f541c-413">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="f541c-413">Performance counters settings</span></span>
 - <span data-ttu-id="f541c-414">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="f541c-414">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="f541c-415">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="f541c-415">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="f541c-416">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="f541c-416">Usage and limits reporting</span></span>
 - <span data-ttu-id="f541c-417">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="f541c-417">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="f541c-418">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="f541c-418">Support for custom images</span></span>
 - <span data-ttu-id="f541c-419">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="f541c-419">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="f541c-420">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="f541c-420">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="f541c-421">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="f541c-421">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="f541c-422">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="f541c-422">National clouds are supported</span></span>
* <span data-ttu-id="f541c-423">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="f541c-423">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="f541c-424">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="f541c-424">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="f541c-425">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="f541c-425">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="f541c-426">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="f541c-426">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="f541c-427">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="f541c-427">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="f541c-428">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="f541c-428">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="f541c-429">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-429">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="f541c-430">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="f541c-430">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="f541c-431">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="f541c-431">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="f541c-432">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-432">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="f541c-433">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="f541c-433">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="f541c-434">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="f541c-434">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="f541c-435">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-435">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="f541c-436">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="f541c-436">Billing</span></span>

* <span data-ttu-id="f541c-437">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="f541c-437">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="f541c-438">Потребление</span><span class="sxs-lookup"><span data-stu-id="f541c-438">Consumption</span></span>

* <span data-ttu-id="f541c-439">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="f541c-439">Added `marketplace` commands</span></span>
* <span data-ttu-id="f541c-440">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="f541c-440">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="f541c-441">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="f541c-441">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="f541c-442">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="f541c-442">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="f541c-443">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="f541c-443">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="f541c-444">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="f541c-444">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="f541c-445">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f541c-445">Container</span></span>

* <span data-ttu-id="f541c-446">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="f541c-446">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="f541c-447">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="f541c-447">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="f541c-448">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f541c-448">Extension</span></span>

* <span data-ttu-id="f541c-449">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="f541c-449">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="f541c-450">Interactive</span><span class="sxs-lookup"><span data-stu-id="f541c-450">Interactive</span></span>

* <span data-ttu-id="f541c-451">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="f541c-451">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="f541c-452">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="f541c-452">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="f541c-453">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="f541c-453">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="f541c-454">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-454">Network</span></span>

* <span data-ttu-id="f541c-455">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-455">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="f541c-456">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-456">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="f541c-457">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="f541c-457">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="f541c-458">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="f541c-458">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="f541c-459">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="f541c-459">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="f541c-460">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-460">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="f541c-461">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-461">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="f541c-462">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="f541c-462">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="f541c-463">Профиль</span><span class="sxs-lookup"><span data-stu-id="f541c-463">Profile</span></span>

* <span data-ttu-id="f541c-464">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="f541c-464">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="f541c-465">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="f541c-465">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="f541c-466">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="f541c-466">RDBMS</span></span>

* <span data-ttu-id="f541c-467">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="f541c-467">Added `georestore` command</span></span>
* <span data-ttu-id="f541c-468">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="f541c-468">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-469">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-469">Resource</span></span>

* <span data-ttu-id="f541c-470">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-470">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="f541c-471">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-471">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-472">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-472">SQL</span></span>

* <span data-ttu-id="f541c-473">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="f541c-473">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-474">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-474">Storage</span></span>

* <span data-ttu-id="f541c-475">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="f541c-475">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-476">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-476">VM</span></span>

* <span data-ttu-id="f541c-477">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="f541c-477">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="f541c-478">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="f541c-478">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="f541c-480">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-480">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="f541c-481">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="f541c-481">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="f541c-482">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="f541c-482">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="f541c-483">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="f541c-483">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="f541c-484">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-484">March 27, 2018</span></span>

<span data-ttu-id="f541c-485">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="f541c-485">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="f541c-486">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-486">Core</span></span>

* <span data-ttu-id="f541c-487">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="f541c-487">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-488">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-488">ACS</span></span>

* <span data-ttu-id="f541c-489">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="f541c-489">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-490">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-490">Appservice</span></span>

* <span data-ttu-id="f541c-491">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-491">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="f541c-492">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-492">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f541c-493">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="f541c-493">Backup</span></span>

* <span data-ttu-id="f541c-494">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="f541c-494">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="f541c-495">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="f541c-495">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="f541c-496">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="f541c-496">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="f541c-497">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-497">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="f541c-498">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f541c-498">Container</span></span>

* <span data-ttu-id="f541c-499">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="f541c-499">Added `container exec` command.</span></span> <span data-ttu-id="f541c-500">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f541c-500">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="f541c-501">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f541c-501">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="f541c-502">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f541c-502">Extension</span></span>

* <span data-ttu-id="f541c-503">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="f541c-503">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="f541c-504">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="f541c-504">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="f541c-505">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f541c-505">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="f541c-506">Interactive</span><span class="sxs-lookup"><span data-stu-id="f541c-506">Interactive</span></span>

* <span data-ttu-id="f541c-507">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="f541c-507">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="f541c-508">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="f541c-508">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="f541c-509">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="f541c-509">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="f541c-510">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="f541c-510">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="f541c-511">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="f541c-511">Lab</span></span>

* <span data-ttu-id="f541c-512">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="f541c-512">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="f541c-513">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f541c-513">Monitor</span></span>

* <span data-ttu-id="f541c-514">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="f541c-514">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="f541c-515">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="f541c-515">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="f541c-516">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="f541c-516">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="f541c-517">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-517">Network</span></span>

* <span data-ttu-id="f541c-518">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="f541c-518">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="f541c-519">Профиль</span><span class="sxs-lookup"><span data-stu-id="f541c-519">Profile</span></span>

* <span data-ttu-id="f541c-520">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="f541c-520">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f541c-521">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="f541c-521">RDBMS</span></span>

* <span data-ttu-id="f541c-522">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="f541c-522">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-523">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-523">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="f541c-525">Роль</span><span class="sxs-lookup"><span data-stu-id="f541c-525">Role</span></span>

* <span data-ttu-id="f541c-526">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-526">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="f541c-527">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="f541c-527">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="f541c-528">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="f541c-528">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="f541c-529">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-529">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="f541c-530">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="f541c-530">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-531">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-531">Storage</span></span>

* <span data-ttu-id="f541c-532">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="f541c-532">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="f541c-533">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="f541c-533">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-534">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-534">VM</span></span>

* <span data-ttu-id="f541c-535">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="f541c-535">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="f541c-536">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-536">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="f541c-537">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="f541c-537">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="f541c-538">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="f541c-538">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="f541c-539">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-539">March 13, 2018</span></span>

<span data-ttu-id="f541c-540">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="f541c-540">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="f541c-541">ACR</span><span class="sxs-lookup"><span data-stu-id="f541c-541">ACR</span></span>

* <span data-ttu-id="f541c-542">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="f541c-542">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="f541c-543">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="f541c-543">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="f541c-544">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="f541c-544">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-545">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-545">ACS</span></span>

* <span data-ttu-id="f541c-546">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="f541c-546">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="f541c-547">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="f541c-547">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="f541c-548">Помощник</span><span class="sxs-lookup"><span data-stu-id="f541c-548">Advisor</span></span>

* <span data-ttu-id="f541c-549">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="f541c-549">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="f541c-550">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-550">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="f541c-551">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="f541c-551">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="f541c-552">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="f541c-552">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="f541c-553">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-553">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-554">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-554">Appservice</span></span>

* <span data-ttu-id="f541c-555">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="f541c-555">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="f541c-556">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-556">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="f541c-557">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="f541c-557">Eventhubs</span></span>

* <span data-ttu-id="f541c-558">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f541c-558">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="f541c-559">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f541c-559">Extension</span></span>

* <span data-ttu-id="f541c-560">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="f541c-560">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="f541c-561">Interactive</span><span class="sxs-lookup"><span data-stu-id="f541c-561">Interactive</span></span>

* <span data-ttu-id="f541c-562">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="f541c-562">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="f541c-563">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="f541c-563">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="f541c-564">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="f541c-564">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="f541c-565">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="f541c-565">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="f541c-566">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f541c-566">Monitor</span></span>

* <span data-ttu-id="f541c-567">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="f541c-567">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="f541c-568">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="f541c-568">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="f541c-569">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="f541c-569">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="f541c-570">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="f541c-570">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="f541c-571">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-571">Network</span></span>

* <span data-ttu-id="f541c-572">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-572">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="f541c-573">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="f541c-573">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="f541c-574">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="f541c-574">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="f541c-575">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="f541c-575">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="f541c-576">Профиль</span><span class="sxs-lookup"><span data-stu-id="f541c-576">Profile</span></span>

* <span data-ttu-id="f541c-577">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="f541c-577">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="f541c-578">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="f541c-578">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="f541c-579">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="f541c-579">RDBMS</span></span>

* <span data-ttu-id="f541c-580">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="f541c-580">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="f541c-581">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="f541c-581">Service Bus</span></span>

* <span data-ttu-id="f541c-582">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f541c-582">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-583">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-583">Storage</span></span>

* <span data-ttu-id="f541c-584">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="f541c-584">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="f541c-585">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="f541c-585">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-586">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-586">VM</span></span>

* <span data-ttu-id="f541c-587">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="f541c-587">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="f541c-588">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="f541c-588">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="f541c-589">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-589">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="f541c-590">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="f541c-590">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="f541c-591">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="f541c-591">February 27, 2018</span></span>

<span data-ttu-id="f541c-592">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="f541c-592">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="f541c-593">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-593">Core</span></span>

* <span data-ttu-id="f541c-594">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="f541c-594">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="f541c-595">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="f541c-595">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="f541c-596">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="f541c-596">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-597">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-597">ACS</span></span>

* <span data-ttu-id="f541c-598">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f541c-598">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="f541c-599">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="f541c-599">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="f541c-600">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="f541c-600">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="f541c-601">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="f541c-601">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-602">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-602">Appservice</span></span>

* <span data-ttu-id="f541c-603">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="f541c-603">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="f541c-604">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="f541c-604">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="f541c-605">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="f541c-605">Cognitive Services</span></span>

* <span data-ttu-id="f541c-606">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="f541c-606">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="f541c-607">Потребление</span><span class="sxs-lookup"><span data-stu-id="f541c-607">Consumption</span></span>

* <span data-ttu-id="f541c-608">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="f541c-608">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="f541c-609">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="f541c-609">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="f541c-610">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f541c-610">Container</span></span>

* <span data-ttu-id="f541c-611">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="f541c-611">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="f541c-612">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-612">Network</span></span>

* <span data-ttu-id="f541c-613">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="f541c-613">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-614">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-614">Resource</span></span>

* <span data-ttu-id="f541c-615">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="f541c-615">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="f541c-616">Роль</span><span class="sxs-lookup"><span data-stu-id="f541c-616">Role</span></span>

* <span data-ttu-id="f541c-617">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="f541c-617">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-618">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-618">SQL</span></span>

* <span data-ttu-id="f541c-619">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="f541c-619">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-620">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-620">Storage</span></span>

* <span data-ttu-id="f541c-621">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-621">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-622">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-622">VM</span></span>

* <span data-ttu-id="f541c-623">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="f541c-623">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="f541c-624">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-624">February 13, 2018</span></span>

<span data-ttu-id="f541c-625">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="f541c-625">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="f541c-626">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-626">Core</span></span>

* <span data-ttu-id="f541c-627">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="f541c-627">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-628">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-628">ACS</span></span>

* <span data-ttu-id="f541c-629">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="f541c-629">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="f541c-630">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-630">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="f541c-631">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="f541c-631">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="f541c-632">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="f541c-632">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="f541c-633">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="f541c-633">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="f541c-634">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="f541c-634">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="f541c-635">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="f541c-635">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="f541c-636">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="f541c-636">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-637">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-637">Appservice</span></span>

* <span data-ttu-id="f541c-638">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="f541c-638">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="f541c-639">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="f541c-639">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="f541c-640">CDN</span><span class="sxs-lookup"><span data-stu-id="f541c-640">CDN</span></span>

* <span data-ttu-id="f541c-641">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-641">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="f541c-642">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f541c-642">Container</span></span>

* <span data-ttu-id="f541c-643">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="f541c-643">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="f541c-644">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f541c-644">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f541c-645">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f541c-645">CosmosDB</span></span>

* <span data-ttu-id="f541c-646">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="f541c-646">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="f541c-647">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f541c-647">Extension</span></span>

* <span data-ttu-id="f541c-648">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-648">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="f541c-649">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-649">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="f541c-650">Отзыв</span><span class="sxs-lookup"><span data-stu-id="f541c-650">Feedback</span></span>

* <span data-ttu-id="f541c-651">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="f541c-651">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="f541c-652">Interactive</span><span class="sxs-lookup"><span data-stu-id="f541c-652">Interactive</span></span>

* <span data-ttu-id="f541c-653">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="f541c-653">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="f541c-654">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="f541c-654">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="f541c-655">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f541c-655">IoT</span></span>

* <span data-ttu-id="f541c-656">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="f541c-656">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f541c-657">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="f541c-657">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="f541c-658">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-658">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="f541c-659">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="f541c-659">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="f541c-660">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f541c-660">Monitor</span></span>

* <span data-ttu-id="f541c-661">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-661">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="f541c-662">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-662">Network</span></span>

* <span data-ttu-id="f541c-663">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="f541c-663">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="f541c-664">Профиль</span><span class="sxs-lookup"><span data-stu-id="f541c-664">Profile</span></span>

* <span data-ttu-id="f541c-665">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="f541c-665">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-666">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-666">Resource</span></span>

* <span data-ttu-id="f541c-667">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-667">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="f541c-668">Роль</span><span class="sxs-lookup"><span data-stu-id="f541c-668">Role</span></span>

* <span data-ttu-id="f541c-669">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="f541c-669">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-670">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-670">SQL</span></span>

* <span data-ttu-id="f541c-671">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="f541c-671">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="f541c-672">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="f541c-672">Added `sql db rename`</span></span>
* <span data-ttu-id="f541c-673">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="f541c-673">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-674">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-674">Storage</span></span>

* <span data-ttu-id="f541c-675">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="f541c-675">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-676">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-676">VM</span></span>

* <span data-ttu-id="f541c-677">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="f541c-677">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="f541c-678">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="f541c-678">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="f541c-679">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="f541c-679">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="f541c-680">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-680">January 31, 2018</span></span>

<span data-ttu-id="f541c-681">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="f541c-681">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="f541c-682">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-682">Core</span></span>

* <span data-ttu-id="f541c-683">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="f541c-683">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="f541c-684">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="f541c-684">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="f541c-685">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="f541c-685">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="f541c-686">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="f541c-686">Use `--verbose` to see</span></span>
* <span data-ttu-id="f541c-687">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="f541c-687">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-688">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-688">ACS</span></span>

* <span data-ttu-id="f541c-689">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="f541c-689">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="f541c-690">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="f541c-690">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-691">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-691">Appservice</span></span>

* <span data-ttu-id="f541c-692">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="f541c-692">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="f541c-693">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="f541c-693">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="f541c-694">CDN</span><span class="sxs-lookup"><span data-stu-id="f541c-694">CDN</span></span>

* <span data-ttu-id="f541c-695">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-695">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f541c-696">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f541c-696">CosmosDB</span></span>

* <span data-ttu-id="f541c-697">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="f541c-697">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="f541c-698">Interactive</span><span class="sxs-lookup"><span data-stu-id="f541c-698">Interactive</span></span>

* <span data-ttu-id="f541c-699">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="f541c-699">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="f541c-700">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-700">Network</span></span>

* <span data-ttu-id="f541c-701">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-701">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="f541c-702">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f541c-702">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="f541c-703">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-703">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="f541c-704">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-704">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="f541c-705">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="f541c-705">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="f541c-706">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="f541c-706">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="f541c-707">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="f541c-707">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="f541c-708">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="f541c-708">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="f541c-709">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="f541c-709">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="f541c-710">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="f541c-710">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="f541c-711">Профиль</span><span class="sxs-lookup"><span data-stu-id="f541c-711">Profile</span></span>

* <span data-ttu-id="f541c-712">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="f541c-712">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-713">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-713">Resource</span></span>

* <span data-ttu-id="f541c-714">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="f541c-714">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-715">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-715">Storage</span></span>

* <span data-ttu-id="f541c-716">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="f541c-716">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="f541c-717">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="f541c-717">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="f541c-718">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="f541c-718">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="f541c-719">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-719">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="f541c-720">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="f541c-720">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-721">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-721">VM</span></span>

* <span data-ttu-id="f541c-722">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="f541c-722">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="f541c-723">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="f541c-723">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="f541c-724">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="f541c-724">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="f541c-725">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-725">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="f541c-726">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-726">January 17, 2018</span></span>

<span data-ttu-id="f541c-727">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="f541c-727">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="f541c-728">ACR</span><span class="sxs-lookup"><span data-stu-id="f541c-728">ACR</span></span>

* <span data-ttu-id="f541c-729">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="f541c-729">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="f541c-730">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="f541c-730">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-731">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-731">ACS</span></span>

* <span data-ttu-id="f541c-732">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="f541c-732">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="f541c-733">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="f541c-733">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-734">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-734">Appservice</span></span>

* <span data-ttu-id="f541c-735">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="f541c-735">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="f541c-736">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="f541c-736">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="f541c-737">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="f541c-737">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="f541c-738">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="f541c-738">Backup</span></span>

* <span data-ttu-id="f541c-739">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="f541c-739">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="f541c-740">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="f541c-740">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="f541c-741">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="f541c-741">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="f541c-742">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="f541c-742">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="f541c-743">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="f541c-743">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="f541c-744">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f541c-744">Batch</span></span>

* <span data-ttu-id="f541c-745">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="f541c-745">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="f541c-746">Облако</span><span class="sxs-lookup"><span data-stu-id="f541c-746">Cloud</span></span>

* <span data-ttu-id="f541c-747">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="f541c-747">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="f541c-748">Потребление</span><span class="sxs-lookup"><span data-stu-id="f541c-748">Consumption</span></span>

* <span data-ttu-id="f541c-749">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="f541c-749">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="f541c-750">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="f541c-750">Event Grid</span></span>

* <span data-ttu-id="f541c-751">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="f541c-751">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f541c-752">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="f541c-752">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="f541c-753">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="f541c-753">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="f541c-754">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="f541c-754">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="f541c-755">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-755">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="f541c-756">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-756">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="f541c-757">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="f541c-757">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="f541c-758">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="f541c-758">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="f541c-759">Interactive</span><span class="sxs-lookup"><span data-stu-id="f541c-759">Interactive</span></span>

* <span data-ttu-id="f541c-760">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="f541c-760">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="f541c-761">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="f541c-761">Fixed errors on startup</span></span>
* <span data-ttu-id="f541c-762">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="f541c-762">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="f541c-763">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f541c-763">IoT</span></span>

* <span data-ttu-id="f541c-764">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="f541c-764">Added support for device provisioning service</span></span>
* <span data-ttu-id="f541c-765">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="f541c-765">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="f541c-766">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="f541c-766">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="f541c-767">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f541c-767">Monitor</span></span>

* <span data-ttu-id="f541c-768">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="f541c-768">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="f541c-769">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-769">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="f541c-770">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="f541c-770">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="f541c-771">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-771">Network</span></span>

* <span data-ttu-id="f541c-772">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="f541c-772">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="f541c-773">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="f541c-773">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="f541c-774">Профиль</span><span class="sxs-lookup"><span data-stu-id="f541c-774">Profile</span></span>

* <span data-ttu-id="f541c-775">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="f541c-775">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="f541c-776">Роль</span><span class="sxs-lookup"><span data-stu-id="f541c-776">Role</span></span>

* <span data-ttu-id="f541c-777">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="f541c-777">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f541c-778">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f541c-778">Service Fabric</span></span>

* <span data-ttu-id="f541c-779">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="f541c-779">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="f541c-780">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="f541c-780">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-781">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-781">VM</span></span>

* <span data-ttu-id="f541c-782">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="f541c-782">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="f541c-783">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="f541c-783">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="f541c-784">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="f541c-784">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="f541c-785">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="f541c-785">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="f541c-786">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="f541c-786">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="f541c-787">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="f541c-787">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="f541c-788">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-788">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="f541c-789">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="f541c-789">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="f541c-790">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-790">December 19, 2017</span></span>

<span data-ttu-id="f541c-791">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="f541c-791">Version 2.0.23</span></span>

* <span data-ttu-id="f541c-792">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="f541c-792">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="f541c-793">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f541c-793">Container</span></span>

* <span data-ttu-id="f541c-794">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f541c-794">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="f541c-795">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-795">Network</span></span>

* <span data-ttu-id="f541c-796">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f541c-796">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="f541c-797">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f541c-797">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-798">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-798">Storage</span></span>

* <span data-ttu-id="f541c-799">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="f541c-799">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-800">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-800">VM</span></span>

* <span data-ttu-id="f541c-801">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="f541c-801">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="f541c-802">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-802">December 5, 2017</span></span>

<span data-ttu-id="f541c-803">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="f541c-803">Version 2.0.22</span></span>

* <span data-ttu-id="f541c-804">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="f541c-804">Removed `az component` commands.</span></span> <span data-ttu-id="f541c-805">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="f541c-805">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="f541c-806">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-806">Core</span></span>
* <span data-ttu-id="f541c-807">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="f541c-807">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="f541c-808">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="f541c-808">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-809">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-809">ACS</span></span>

* <span data-ttu-id="f541c-810">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="f541c-810">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="f541c-811">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-811">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="f541c-812">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="f541c-812">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="f541c-813">Помощник</span><span class="sxs-lookup"><span data-stu-id="f541c-813">Advisor</span></span>

* <span data-ttu-id="f541c-814">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f541c-814">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-815">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-815">Appservice</span></span>

* <span data-ttu-id="f541c-816">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="f541c-816">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="f541c-817">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="f541c-817">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="f541c-818">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="f541c-818">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="f541c-819">Потребление</span><span class="sxs-lookup"><span data-stu-id="f541c-819">Consumption</span></span>

* <span data-ttu-id="f541c-820">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="f541c-820">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="f541c-821">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f541c-821">Container</span></span>

* <span data-ttu-id="f541c-822">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="f541c-822">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="f541c-823">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f541c-823">Monitor</span></span>

* <span data-ttu-id="f541c-824">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="f541c-824">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-825">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-825">Resource</span></span>

* <span data-ttu-id="f541c-826">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="f541c-826">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="f541c-827">Роль</span><span class="sxs-lookup"><span data-stu-id="f541c-827">Role</span></span>

* <span data-ttu-id="f541c-828">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="f541c-828">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="f541c-829">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="f541c-829">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="f541c-830">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="f541c-830">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-831">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-831">SQL</span></span>

* <span data-ttu-id="f541c-832">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="f541c-832">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="f541c-833">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-833">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-834">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-834">VM</span></span>

* <span data-ttu-id="f541c-835">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="f541c-835">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="f541c-836">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-836">November 14, 2017</span></span>

<span data-ttu-id="f541c-837">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="f541c-837">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="f541c-838">ACR</span><span class="sxs-lookup"><span data-stu-id="f541c-838">ACR</span></span>

* <span data-ttu-id="f541c-839">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="f541c-839">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="f541c-840">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-840">ACS</span></span>

* <span data-ttu-id="f541c-841">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="f541c-841">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="f541c-842">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="f541c-842">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="f541c-843">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="f541c-843">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="f541c-844">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="f541c-844">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="f541c-845">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="f541c-845">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-846">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-846">Appservice</span></span>

* <span data-ttu-id="f541c-847">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="f541c-847">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="f541c-848">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="f541c-848">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="f541c-849">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="f541c-849">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="f541c-850">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="f541c-850">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="f541c-851">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="f541c-851">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="f541c-852">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="f541c-852">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="f541c-853">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f541c-853">Batch</span></span>

* <span data-ttu-id="f541c-854">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="f541c-854">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="f541c-855">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f541c-855">Batchai</span></span>

* <span data-ttu-id="f541c-856">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-856">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="f541c-857">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-857">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="f541c-858">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="f541c-858">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="f541c-859">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-859">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="f541c-860">Облако</span><span class="sxs-lookup"><span data-stu-id="f541c-860">Cloud</span></span>

* <span data-ttu-id="f541c-861">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="f541c-861">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="f541c-862">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f541c-862">Container</span></span>

* <span data-ttu-id="f541c-863">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="f541c-863">Added support to open multiple ports</span></span>
* <span data-ttu-id="f541c-864">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f541c-864">Added container group restart policy</span></span>
* <span data-ttu-id="f541c-865">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="f541c-865">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="f541c-866">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="f541c-866">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f541c-867">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f541c-867">Data Lake Analytics</span></span>

* <span data-ttu-id="f541c-868">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="f541c-868">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f541c-869">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f541c-869">Data Lake Store</span></span>

* <span data-ttu-id="f541c-870">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="f541c-870">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="f541c-871">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f541c-871">Extension</span></span>

* <span data-ttu-id="f541c-872">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="f541c-872">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="f541c-873">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="f541c-873">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="f541c-874">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f541c-874">IoT</span></span>

* <span data-ttu-id="f541c-875">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="f541c-875">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="f541c-876">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f541c-876">Monitor</span></span>

* <span data-ttu-id="f541c-877">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="f541c-877">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="f541c-878">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-878">Network</span></span>

* <span data-ttu-id="f541c-879">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="f541c-879">Added support for CAA DNS records</span></span>
* <span data-ttu-id="f541c-880">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-880">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="f541c-881">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="f541c-881">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="f541c-882">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="f541c-882">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="f541c-883">Резервирование</span><span class="sxs-lookup"><span data-stu-id="f541c-883">Reservations</span></span>

* <span data-ttu-id="f541c-884">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="f541c-884">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-885">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-885">Resource</span></span>

* <span data-ttu-id="f541c-886">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="f541c-886">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-887">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-887">SQL</span></span>

* <span data-ttu-id="f541c-888">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-888">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-889">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-889">Storage</span></span>

* <span data-ttu-id="f541c-890">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f541c-890">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="f541c-891">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="f541c-891">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="f541c-892">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="f541c-892">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="f541c-893">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="f541c-893">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="f541c-894">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-894">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="f541c-895">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="f541c-895">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="f541c-896">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-896">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-897">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-897">VM</span></span>

* <span data-ttu-id="f541c-898">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="f541c-898">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="f541c-899">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="f541c-899">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="f541c-900">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="f541c-900">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="f541c-901">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="f541c-901">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="f541c-902">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="f541c-902">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="f541c-903">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-903">October 24, 2017</span></span>

<span data-ttu-id="f541c-904">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="f541c-904">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="f541c-905">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-905">Core</span></span>

* <span data-ttu-id="f541c-906">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="f541c-906">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="f541c-907">ACR</span><span class="sxs-lookup"><span data-stu-id="f541c-907">ACR</span></span>

* <span data-ttu-id="f541c-908">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="f541c-908">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="f541c-909">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="f541c-909">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="f541c-910">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="f541c-910">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-911">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-911">ACS</span></span>

* <span data-ttu-id="f541c-912">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="f541c-912">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="f541c-913">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="f541c-913">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-914">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-914">Appservice</span></span>

* <span data-ttu-id="f541c-915">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="f541c-915">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="f541c-916">Компонент</span><span class="sxs-lookup"><span data-stu-id="f541c-916">Component</span></span>

* <span data-ttu-id="f541c-917">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="f541c-917">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="f541c-918">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f541c-918">Monitor</span></span>

* <span data-ttu-id="f541c-919">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="f541c-919">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-920">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-920">Resource</span></span>

* <span data-ttu-id="f541c-921">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="f541c-921">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="f541c-922">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="f541c-922">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-923">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-923">VM</span></span>

* <span data-ttu-id="f541c-924">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="f541c-924">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="f541c-925">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-925">October 9, 2017</span></span>

<span data-ttu-id="f541c-926">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="f541c-926">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="f541c-927">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-927">Core</span></span>

* <span data-ttu-id="f541c-928">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="f541c-928">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-929">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-929">Appservice</span></span>

* <span data-ttu-id="f541c-930">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-930">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="f541c-931">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f541c-931">Batch</span></span>

* <span data-ttu-id="f541c-932">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="f541c-932">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="f541c-933">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="f541c-933">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="f541c-934">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="f541c-934">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="f541c-935">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="f541c-935">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="f541c-936">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f541c-936">Batchai</span></span>

* <span data-ttu-id="f541c-937">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="f541c-937">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="f541c-938">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f541c-938">Keyvault</span></span>

* <span data-ttu-id="f541c-939">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="f541c-939">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="f541c-940">(#4448)</span><span class="sxs-lookup"><span data-stu-id="f541c-940">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="f541c-941">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-941">Network</span></span>

* <span data-ttu-id="f541c-942">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="f541c-942">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="f541c-943">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="f541c-943">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-944">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-944">Resource</span></span>

* <span data-ttu-id="f541c-945">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="f541c-945">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="f541c-946">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="f541c-946">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="f541c-947">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="f541c-947">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="f541c-948">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="f541c-948">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-949">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-949">Sql</span></span>

* <span data-ttu-id="f541c-950">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="f541c-950">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="f541c-951">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="f541c-951">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="f541c-952">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="f541c-952">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-953">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-953">Storage</span></span>

* <span data-ttu-id="f541c-954">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f541c-954">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-955">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="f541c-955">Vm</span></span>

* <span data-ttu-id="f541c-956">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="f541c-956">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="f541c-957">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-957">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="f541c-958">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="f541c-958">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="f541c-959">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-959">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="f541c-960">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="f541c-960">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="f541c-961">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-961">September 22, 2017</span></span>

<span data-ttu-id="f541c-962">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="f541c-962">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-963">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-963">Resource</span></span>

* <span data-ttu-id="f541c-964">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="f541c-964">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="f541c-965">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="f541c-965">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="f541c-966">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="f541c-966">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="f541c-967">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="f541c-967">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="f541c-968">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-968">Network</span></span>

* <span data-ttu-id="f541c-969">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="f541c-969">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="f541c-970">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="f541c-970">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="f541c-971">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="f541c-971">Added `asg` application security group commands</span></span>
* <span data-ttu-id="f541c-972">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="f541c-972">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="f541c-973">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f541c-973">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f541c-974">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f541c-974">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="f541c-975">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-975">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-976">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-976">Storage</span></span>

* <span data-ttu-id="f541c-977">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="f541c-977">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="f541c-978">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="f541c-978">Eventgrid</span></span>

* <span data-ttu-id="f541c-979">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="f541c-979">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-980">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-980">SQL</span></span>

* <span data-ttu-id="f541c-981">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="f541c-981">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="f541c-982">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="f541c-982">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="f541c-983">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="f541c-983">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="f541c-984">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f541c-984">Keyvault</span></span>

* <span data-ttu-id="f541c-985">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="f541c-985">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-986">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-986">VM</span></span>

* <span data-ttu-id="f541c-987">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="f541c-987">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="f541c-988">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="f541c-988">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="f541c-989">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="f541c-989">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="f541c-990">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="f541c-990">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="f541c-991">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="f541c-991">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="f541c-992">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="f541c-992">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-993">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-993">ACS</span></span>

* <span data-ttu-id="f541c-994">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="f541c-994">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-995">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-995">Appservice</span></span>

* <span data-ttu-id="f541c-996">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="f541c-996">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="f541c-997">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="f541c-997">Backup</span></span>

* <span data-ttu-id="f541c-998">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="f541c-998">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="f541c-999">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-999">September 11, 2017</span></span>

<span data-ttu-id="f541c-1000">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="f541c-1000">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="f541c-1001">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-1001">Core</span></span>

* <span data-ttu-id="f541c-1002">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="f541c-1002">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="f541c-1003">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="f541c-1003">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-1004">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-1004">Acs</span></span>

* <span data-ttu-id="f541c-1005">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1005">Added `acs list-locations` command</span></span>
* <span data-ttu-id="f541c-1006">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f541c-1006">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-1007">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-1007">Appservice</span></span>

* <span data-ttu-id="f541c-1008">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="f541c-1008">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="f541c-1009">CDN</span><span class="sxs-lookup"><span data-stu-id="f541c-1009">CDN</span></span>

* <span data-ttu-id="f541c-1010">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1010">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="f541c-1011">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="f541c-1011">Extension</span></span>

* <span data-ttu-id="f541c-1012">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f541c-1012">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="f541c-1013">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f541c-1013">Keyvault</span></span>

* <span data-ttu-id="f541c-1014">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1014">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="f541c-1015">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-1015">Network</span></span>

* <span data-ttu-id="f541c-1016">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1016">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f541c-1017">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1017">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="f541c-1018">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1018">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="f541c-1019">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1019">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f541c-1020">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1020">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-1021">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-1021">Resource</span></span>

* <span data-ttu-id="f541c-1022">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1022">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="f541c-1023">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1023">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="f541c-1024">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="f541c-1024">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="f541c-1025">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="f541c-1025">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-1026">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-1026">SQL</span></span>

* <span data-ttu-id="f541c-1027">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1027">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-1028">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-1028">VM</span></span>

* <span data-ttu-id="f541c-1029">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="f541c-1029">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="f541c-1030">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="f541c-1030">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="f541c-1031">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1031">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="f541c-1032">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="f541c-1032">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="f541c-1033">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="f541c-1033">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="f541c-1034">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-1034">August 31, 2017</span></span>

<span data-ttu-id="f541c-1035">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="f541c-1035">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="f541c-1036">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f541c-1036">Keyvault</span></span>

* <span data-ttu-id="f541c-1037">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1037">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="f541c-1038">Sf</span><span class="sxs-lookup"><span data-stu-id="f541c-1038">Sf</span></span>

* <span data-ttu-id="f541c-1039">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="f541c-1039">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-1040">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-1040">Storage</span></span>

* <span data-ttu-id="f541c-1041">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="f541c-1041">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="f541c-1042">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="f541c-1042">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="f541c-1043">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-1043">August 28, 2017</span></span>

<span data-ttu-id="f541c-1044">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="f541c-1044">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="f541c-1045">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="f541c-1045">CLI</span></span>

* <span data-ttu-id="f541c-1046">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="f541c-1046">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-1047">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-1047">ACS</span></span>

* <span data-ttu-id="f541c-1048">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="f541c-1048">Corrected preview regions</span></span>
* <span data-ttu-id="f541c-1049">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1049">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="f541c-1050">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="f541c-1050">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-1051">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-1051">Appservice</span></span>

* <span data-ttu-id="f541c-1052">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1052">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="f541c-1053">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1053">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="f541c-1054">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1054">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="f541c-1055">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="f541c-1055">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="f541c-1056">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="f541c-1056">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="f541c-1057">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f541c-1057">IoT</span></span>

* <span data-ttu-id="f541c-1058">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="f541c-1058">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="f541c-1059">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-1059">Network</span></span>

* <span data-ttu-id="f541c-1060">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1060">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="f541c-1061">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1061">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="f541c-1062">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1062">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="f541c-1063">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1063">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="f541c-1064">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1064">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="f541c-1065">Профиль</span><span class="sxs-lookup"><span data-stu-id="f541c-1065">Profile</span></span>

* <span data-ttu-id="f541c-1066">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="f541c-1066">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f541c-1067">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f541c-1067">Service Fabric</span></span>

* <span data-ttu-id="f541c-1068">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="f541c-1068">Preview release</span></span>
* <span data-ttu-id="f541c-1069">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="f541c-1069">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="f541c-1070">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="f541c-1070">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="f541c-1071">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1071">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-1072">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-1072">Storage</span></span>

* <span data-ttu-id="f541c-1073">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="f541c-1073">Enabled setting blob tier</span></span>
* <span data-ttu-id="f541c-1074">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="f541c-1074">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="f541c-1075">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1075">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="f541c-1076">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="f541c-1076">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="f541c-1077">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1077">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="f541c-1078">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1078">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-1079">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-1079">VM</span></span>

* <span data-ttu-id="f541c-1080">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1080">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="f541c-1081">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1081">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="f541c-1082">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="f541c-1082">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="f541c-1083">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="f541c-1083">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="f541c-1084">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="f541c-1084">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="f541c-1085">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1085">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="f541c-1086">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-1086">August 15, 2017</span></span>

<span data-ttu-id="f541c-1087">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="f541c-1087">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-1088">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-1088">ACS</span></span>

* <span data-ttu-id="f541c-1089">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="f541c-1089">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-1090">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-1090">Appservice</span></span>

* <span data-ttu-id="f541c-1091">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="f541c-1091">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="f541c-1092">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="f541c-1092">Event Grid</span></span>

* <span data-ttu-id="f541c-1093">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="f541c-1093">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="f541c-1094">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-1094">August 11, 2017</span></span>

<span data-ttu-id="f541c-1095">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="f541c-1095">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-1096">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-1096">ACS</span></span>

* <span data-ttu-id="f541c-1097">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="f541c-1097">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="f541c-1098">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f541c-1098">Batch</span></span>

* <span data-ttu-id="f541c-1099">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="f541c-1099">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="f541c-1100">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="f541c-1100">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="f541c-1101">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f541c-1101">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="f541c-1102">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="f541c-1102">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="f541c-1103">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="f541c-1103">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="f541c-1104">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="f541c-1104">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="f541c-1105">Компонент</span><span class="sxs-lookup"><span data-stu-id="f541c-1105">Component</span></span>

* <span data-ttu-id="f541c-1106">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="f541c-1106">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="f541c-1107">Контейнер</span><span class="sxs-lookup"><span data-stu-id="f541c-1107">Container</span></span>

* <span data-ttu-id="f541c-1108">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="f541c-1108">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="f541c-1109">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f541c-1109">Data Lake Store</span></span>

* <span data-ttu-id="f541c-1110">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="f541c-1110">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="f541c-1111">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="f541c-1111">Event Grid</span></span>

* <span data-ttu-id="f541c-1112">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="f541c-1112">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="f541c-1113">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-1113">Network</span></span>

* <span data-ttu-id="f541c-1114">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="f541c-1114">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="f541c-1115">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1115">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="f541c-1116">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1116">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="f541c-1117">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1117">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="f541c-1118">Профиль</span><span class="sxs-lookup"><span data-stu-id="f541c-1118">Profile</span></span>

* <span data-ttu-id="f541c-1119">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="f541c-1119">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-1120">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-1120">Storage</span></span>

* <span data-ttu-id="f541c-1121">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="f541c-1121">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-1122">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-1122">VM</span></span>

* <span data-ttu-id="f541c-1123">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="f541c-1123">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="f541c-1124">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1124">Exposed `list-skus` command</span></span>
* <span data-ttu-id="f541c-1125">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="f541c-1125">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="f541c-1126">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="f541c-1126">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="f541c-1127">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="f541c-1127">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="f541c-1128">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-1128">July 28, 2017</span></span>

<span data-ttu-id="f541c-1129">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="f541c-1129">Version 2.0.12</span></span>

* <span data-ttu-id="f541c-1130">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="f541c-1130">Added container commands</span></span>
* <span data-ttu-id="f541c-1131">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="f541c-1131">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="f541c-1132">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-1132">Core</span></span>

* <span data-ttu-id="f541c-1133">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="f541c-1133">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="f541c-1134">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="f541c-1134">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="f541c-1135">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="f541c-1135">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="f541c-1136">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="f541c-1136">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="f541c-1137">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="f541c-1137">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="f541c-1138">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="f541c-1138">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="f541c-1139">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="f541c-1139">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f541c-1140">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="f541c-1140">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="f541c-1141">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="f541c-1141">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="f541c-1142">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="f541c-1142">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="f541c-1143">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="f541c-1143">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="f541c-1144">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="f541c-1144">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="f541c-1145">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="f541c-1145">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="f541c-1146">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="f541c-1146">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="f541c-1147">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="f541c-1147">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="f541c-1148">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="f541c-1148">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="f541c-1149">ACR</span><span class="sxs-lookup"><span data-stu-id="f541c-1149">ACR</span></span>

* <span data-ttu-id="f541c-1150">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="f541c-1150">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="f541c-1151">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="f541c-1151">Support SKU update for managed registries</span></span>
* <span data-ttu-id="f541c-1152">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="f541c-1152">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="f541c-1153">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="f541c-1153">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="f541c-1154">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="f541c-1154">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="f541c-1155">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="f541c-1155">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-1156">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-1156">ACS</span></span>

* <span data-ttu-id="f541c-1157">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="f541c-1157">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-1158">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="f541c-1158">Appservice</span></span>

* <span data-ttu-id="f541c-1159">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="f541c-1159">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="f541c-1160">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="f541c-1160">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="f541c-1161">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1161">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="f541c-1162">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="f541c-1162">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="f541c-1163">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="f541c-1163">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="f541c-1164">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="f541c-1164">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="f541c-1165">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="f541c-1165">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="f541c-1166">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="f541c-1166">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="f541c-1167">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="f541c-1167">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="f541c-1168">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1168">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="f541c-1169">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="f541c-1169">Batch</span></span>

* <span data-ttu-id="f541c-1170">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="f541c-1170">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="f541c-1171">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1171">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="f541c-1172">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1172">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="f541c-1173">CDN</span><span class="sxs-lookup"><span data-stu-id="f541c-1173">CDN</span></span>

* <span data-ttu-id="f541c-1174">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="f541c-1174">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="f541c-1175">Облако</span><span class="sxs-lookup"><span data-stu-id="f541c-1175">Cloud</span></span>

* <span data-ttu-id="f541c-1176">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="f541c-1176">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="f541c-1177">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="f541c-1177">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="f541c-1178">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="f541c-1178">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="f541c-1179">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="f541c-1179">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="f541c-1180">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1180">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f541c-1181">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f541c-1181">CosmosDB</span></span>

* <span data-ttu-id="f541c-1182">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="f541c-1182">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="f541c-1183">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="f541c-1183">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f541c-1184">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f541c-1184">Data Lake Analytics</span></span>

* <span data-ttu-id="f541c-1185">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1185">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="f541c-1186">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1186">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="f541c-1187">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1187">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f541c-1188">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f541c-1188">Data Lake Store</span></span>

* <span data-ttu-id="f541c-1189">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1189">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="f541c-1190">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="f541c-1190">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="f541c-1191">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1191">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="f541c-1192">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="f541c-1192">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="f541c-1193">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="f541c-1193">Interactive</span></span>

* <span data-ttu-id="f541c-1194">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="f541c-1194">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="f541c-1195">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="f541c-1195">Increased test coverage</span></span>
* <span data-ttu-id="f541c-1196">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="f541c-1196">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="f541c-1197">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="f541c-1197">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="f541c-1198">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="f541c-1198">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="f541c-1199">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="f541c-1199">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="f541c-1200">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="f541c-1200">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="f541c-1201">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1201">Added `--progress` flag</span></span>
* <span data-ttu-id="f541c-1202">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1202">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="f541c-1203">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="f541c-1203">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="f541c-1204">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="f541c-1204">IoT</span></span>

* <span data-ttu-id="f541c-1205">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="f541c-1205">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="f541c-1206">(3934).</span><span class="sxs-lookup"><span data-stu-id="f541c-1206">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="f541c-1207">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f541c-1207">Key vault</span></span>

* <span data-ttu-id="f541c-1208">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="f541c-1208">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="f541c-1209">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1209">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="f541c-1210">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="f541c-1210">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f541c-1211">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="f541c-1211">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="f541c-1212">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1212">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="f541c-1213">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="f541c-1213">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="f541c-1214">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="f541c-1214">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="f541c-1215">(3307).</span><span class="sxs-lookup"><span data-stu-id="f541c-1215">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="f541c-1216">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="f541c-1216">Lab</span></span>

* <span data-ttu-id="f541c-1217">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1217">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="f541c-1218">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1218">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="f541c-1219">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f541c-1219">Monitor</span></span>

* <span data-ttu-id="f541c-1220">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="f541c-1220">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="f541c-1221">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1221">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="f541c-1222">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1222">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="f541c-1223">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1223">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="f541c-1224">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1224">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="f541c-1225">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="f541c-1225">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="f541c-1226">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="f541c-1226">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="f541c-1227">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="f541c-1227">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="f541c-1228">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="f541c-1228">`location` no longer required</span></span>
  * <span data-ttu-id="f541c-1229">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="f541c-1229">Add name and ID support for target</span></span>
  * <span data-ttu-id="f541c-1230">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="f541c-1230">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="f541c-1231">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="f541c-1231">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="f541c-1232">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="f541c-1232">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="f541c-1233">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="f541c-1233">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="f541c-1234">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1234">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="f541c-1235">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1235">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="f541c-1236">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-1236">Network</span></span>

* <span data-ttu-id="f541c-1237">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1237">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="f541c-1238">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1238">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="f541c-1239">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="f541c-1239">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="f541c-1240">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1240">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="f541c-1241">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1241">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="f541c-1242">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1242">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="f541c-1243">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1243">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="f541c-1244">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1244">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="f541c-1245">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1245">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="f541c-1246">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1246">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="f541c-1247">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1247">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="f541c-1248">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1248">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="f541c-1249">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1249">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="f541c-1250">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1250">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="f541c-1251">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1251">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="f541c-1252">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1252">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="f541c-1253">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="f541c-1253">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="f541c-1254">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1254">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="f541c-1255">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1255">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="f541c-1256">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1256">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="f541c-1257">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1257">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="f541c-1258">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1258">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="f541c-1259">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1259">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="f541c-1260">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="f541c-1260">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="f541c-1261">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="f541c-1261">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="f541c-1262">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="f541c-1262">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="f541c-1263">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="f541c-1263">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="f541c-1264">Профиль</span><span class="sxs-lookup"><span data-stu-id="f541c-1264">Profile</span></span>

* <span data-ttu-id="f541c-1265">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="f541c-1265">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="f541c-1266">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="f541c-1266">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="f541c-1267">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="f541c-1267">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="f541c-1268">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="f541c-1268">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="f541c-1269">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="f541c-1269">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="f541c-1270">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="f541c-1270">RDBMS</span></span>

* <span data-ttu-id="f541c-1271">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="f541c-1271">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="f541c-1272">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="f541c-1272">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="f541c-1273">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="f541c-1273">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="f541c-1274">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="f541c-1274">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-1275">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-1275">Resource</span></span>

* <span data-ttu-id="f541c-1276">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1276">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="f541c-1277">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1277">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="f541c-1278">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1278">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="f541c-1279">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1279">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="f541c-1280">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="f541c-1280">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="f541c-1281">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1281">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="f541c-1282">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="f541c-1282">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="f541c-1283">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1283">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="f541c-1284">Роль</span><span class="sxs-lookup"><span data-stu-id="f541c-1284">Role</span></span>

* <span data-ttu-id="f541c-1285">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="f541c-1285">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="f541c-1286">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="f541c-1286">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="f541c-1287">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="f541c-1287">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="f541c-1288">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="f541c-1288">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="f541c-1289">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1289">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="f541c-1290">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="f541c-1290">Service Fabric</span></span>
* <span data-ttu-id="f541c-1291">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="f541c-1291">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="f541c-1292">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="f541c-1292">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="f541c-1293">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="f541c-1293">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-1294">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-1294">SQL</span></span>

* <span data-ttu-id="f541c-1295">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1295">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="f541c-1296">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1296">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="f541c-1297">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1297">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-1298">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-1298">Storage</span></span>

* <span data-ttu-id="f541c-1299">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="f541c-1299">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="f541c-1300">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="f541c-1300">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="f541c-1301">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="f541c-1301">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="f541c-1302">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="f541c-1302">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="f541c-1303">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="f541c-1303">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="f541c-1304">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="f541c-1304">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-1305">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-1305">VM</span></span>

* <span data-ttu-id="f541c-1306">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="f541c-1306">Support configuring nsg</span></span>
* <span data-ttu-id="f541c-1307">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="f541c-1307">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="f541c-1308">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="f541c-1308">Support managed service identities</span></span>
* <span data-ttu-id="f541c-1309">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1309">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="f541c-1310">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="f541c-1310">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="f541c-1311">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-1311">May 10, 2017</span></span>

<span data-ttu-id="f541c-1312">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="f541c-1312">Version 2.0.6</span></span>

* <span data-ttu-id="f541c-1313">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="f541c-1313">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="f541c-1314">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="f541c-1314">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="f541c-1315">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="f541c-1315">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="f541c-1316">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="f541c-1316">Include Cognitive Services module</span></span>
* <span data-ttu-id="f541c-1317">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="f541c-1317">Include Service Fabric module</span></span>
* <span data-ttu-id="f541c-1318">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="f541c-1318">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="f541c-1319">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="f541c-1319">Add support for CDN commands</span></span>
* <span data-ttu-id="f541c-1320">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="f541c-1320">Remove Container module</span></span>
* <span data-ttu-id="f541c-1321">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1321">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="f541c-1322">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1322">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="f541c-1323">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-1323">Core</span></span>

* <span data-ttu-id="f541c-1324">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="f541c-1324">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="f541c-1325">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1325">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="f541c-1326">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1326">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="f541c-1327">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1327">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="f541c-1328">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1328">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="f541c-1329">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1329">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="f541c-1330">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1330">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="f541c-1331">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1331">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="f541c-1332">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1332">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="f541c-1333">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="f541c-1333">core: Improved performance</span></span>
* <span data-ttu-id="f541c-1334">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="f541c-1334">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="f541c-1335">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="f541c-1335">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-1336">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-1336">ACS</span></span>

* <span data-ttu-id="f541c-1337">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="f541c-1337">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="f541c-1338">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="f541c-1338">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="f541c-1339">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="f541c-1339">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="f541c-1340">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1340">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-1341">AppService</span><span class="sxs-lookup"><span data-stu-id="f541c-1341">AppService</span></span>

* <span data-ttu-id="f541c-1342">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="f541c-1342">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="f541c-1343">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="f541c-1343">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="f541c-1344">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="f541c-1344">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="f541c-1345">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="f541c-1345">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="f541c-1346">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="f541c-1346">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="f541c-1347">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1347">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="f541c-1348">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="f541c-1348">support slot swap with preview</span></span>
* <span data-ttu-id="f541c-1349">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1349">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="f541c-1350">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1350">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="f541c-1351">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="f541c-1351">CosmosDB</span></span>

* <span data-ttu-id="f541c-1352">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="f541c-1352">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="f541c-1353">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="f541c-1353">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="f541c-1354">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="f541c-1354">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="f541c-1355">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="f541c-1355">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="f541c-1356">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="f541c-1356">Data Lake Analytics</span></span>

* <span data-ttu-id="f541c-1357">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="f541c-1357">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="f541c-1358">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="f541c-1358">Add support for new catalog item type: package.</span></span> <span data-ttu-id="f541c-1359">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1359">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="f541c-1360">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="f541c-1360">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="f541c-1361">Таблица</span><span class="sxs-lookup"><span data-stu-id="f541c-1361">Table</span></span>
  * <span data-ttu-id="f541c-1362">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="f541c-1362">Table valued function</span></span>
  * <span data-ttu-id="f541c-1363">Просмотр</span><span class="sxs-lookup"><span data-stu-id="f541c-1363">View</span></span>
  * <span data-ttu-id="f541c-1364">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="f541c-1364">Table Statistics.</span></span> <span data-ttu-id="f541c-1365">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="f541c-1365">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="f541c-1366">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="f541c-1366">Data Lake Store</span></span>

* <span data-ttu-id="f541c-1367">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="f541c-1367">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="f541c-1368">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1368">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="f541c-1369">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="f541c-1369">missed help for access show.</span></span> <span data-ttu-id="f541c-1370">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="f541c-1370">adding it.</span></span> <span data-ttu-id="f541c-1371">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="f541c-1371">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="f541c-1372">Поиск</span><span class="sxs-lookup"><span data-stu-id="f541c-1372">Find</span></span>

* <span data-ttu-id="f541c-1373">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="f541c-1373">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="f541c-1374">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="f541c-1374">KeyVault</span></span>

* <span data-ttu-id="f541c-1375">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="f541c-1375">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="f541c-1376">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="f541c-1376">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="f541c-1377">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="f541c-1377">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="f541c-1378">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="f541c-1378">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="f541c-1379">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1379">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="f541c-1380">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="f541c-1380">Lab</span></span>

* <span data-ttu-id="f541c-1381">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="f541c-1381">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="f541c-1382">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="f541c-1382">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="f541c-1383">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="f541c-1383">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="f541c-1384">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="f541c-1384">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="f541c-1385">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="f541c-1385">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="f541c-1386">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="f541c-1386">Monitor</span></span>

* <span data-ttu-id="f541c-1387">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1387">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="f541c-1388">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1388">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="f541c-1389">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-1389">Network</span></span>

* <span data-ttu-id="f541c-1390">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1390">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="f541c-1391">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1391">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="f541c-1392">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="f541c-1392">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="f541c-1393">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="f541c-1393">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="f541c-1394">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="f541c-1394">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="f541c-1395">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="f541c-1395">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="f541c-1396">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="f541c-1396">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="f541c-1397">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="f541c-1397">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="f541c-1398">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1398">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="f541c-1399">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="f541c-1399">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="f541c-1400">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1400">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="f541c-1401">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1401">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="f541c-1402">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="f541c-1402">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="f541c-1403">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="f541c-1403">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="f541c-1404">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="f541c-1404">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="f541c-1405">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="f541c-1405">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="f541c-1406">Профиль</span><span class="sxs-lookup"><span data-stu-id="f541c-1406">Profile</span></span>

* <span data-ttu-id="f541c-1407">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1407">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="f541c-1408">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1408">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="f541c-1409">Redis</span><span class="sxs-lookup"><span data-stu-id="f541c-1409">Redis</span></span>

* <span data-ttu-id="f541c-1410">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="f541c-1410">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="f541c-1411">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="f541c-1411">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="f541c-1412">Ресурс</span><span class="sxs-lookup"><span data-stu-id="f541c-1412">Resource</span></span>

* <span data-ttu-id="f541c-1413">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1413">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="f541c-1414">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1414">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="f541c-1415">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1415">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="f541c-1416">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="f541c-1416">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="f541c-1417">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="f541c-1417">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="f541c-1418">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="f541c-1418">Add docs for az lock update.</span></span> <span data-ttu-id="f541c-1419">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="f541c-1419">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="f541c-1420">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="f541c-1420">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="f541c-1421">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="f541c-1421">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="f541c-1422">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="f541c-1422">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="f541c-1423">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="f541c-1423">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="f541c-1424">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1424">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="f541c-1425">Роль</span><span class="sxs-lookup"><span data-stu-id="f541c-1425">Role</span></span>

* <span data-ttu-id="f541c-1426">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1426">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="f541c-1427">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1427">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="f541c-1428">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1428">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="f541c-1429">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="f541c-1429">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="f541c-1430">SQL</span><span class="sxs-lookup"><span data-stu-id="f541c-1430">SQL</span></span>

* <span data-ttu-id="f541c-1431">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="f541c-1431">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="f541c-1432">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1432">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="f541c-1433">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-1433">Storage</span></span>

* <span data-ttu-id="f541c-1434">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1434">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="f541c-1435">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="f541c-1435">Add support for incremental blob copy</span></span>
* <span data-ttu-id="f541c-1436">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="f541c-1436">Add support for large block blob upload</span></span>
* <span data-ttu-id="f541c-1437">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="f541c-1437">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-1438">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-1438">VM</span></span>

* <span data-ttu-id="f541c-1439">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="f541c-1439">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="f541c-1440">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="f541c-1440">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="f541c-1441">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="f541c-1441">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="f541c-1442">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="f541c-1442">az vm/vmss disk</span></span>
  3. <span data-ttu-id="f541c-1443">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="f541c-1443">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="f541c-1444">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="f541c-1444">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="f541c-1445">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1445">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="f541c-1446">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-1446">April 3, 2017</span></span>

<span data-ttu-id="f541c-1447">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="f541c-1447">Version 2.0.2</span></span>

<span data-ttu-id="f541c-1448">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="f541c-1448">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="f541c-1449">Core</span><span class="sxs-lookup"><span data-stu-id="f541c-1449">Core</span></span>

* <span data-ttu-id="f541c-1450">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f541c-1450">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="f541c-1451">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1451">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="f541c-1452">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1452">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="f541c-1453">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1453">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f541c-1454">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1454">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="f541c-1455">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="f541c-1455">Add prompting for missing template parameters.</span></span> <span data-ttu-id="f541c-1456">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1456">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="f541c-1457">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f541c-1457">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="f541c-1458">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="f541c-1458">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="f541c-1459">ACS</span><span class="sxs-lookup"><span data-stu-id="f541c-1459">ACS</span></span>

* <span data-ttu-id="f541c-1460">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1460">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="f541c-1461">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="f541c-1461">Add support for ssh key password prompting.</span></span> <span data-ttu-id="f541c-1462">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1462">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="f541c-1463">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="f541c-1463">Add support for windows clusters.</span></span> <span data-ttu-id="f541c-1464">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1464">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="f541c-1465">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="f541c-1465">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="f541c-1466">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1466">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="f541c-1467">AppService</span><span class="sxs-lookup"><span data-stu-id="f541c-1467">AppService</span></span>

* <span data-ttu-id="f541c-1468">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1468">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="f541c-1469">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1469">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="f541c-1470">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1470">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="f541c-1471">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1471">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="f541c-1472">Data Lake</span><span class="sxs-lookup"><span data-stu-id="f541c-1472">DataLake</span></span>

* <span data-ttu-id="f541c-1473">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="f541c-1473">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="f541c-1474">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="f541c-1474">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="f541c-1475">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="f541c-1475">DocuemntDB</span></span>

* <span data-ttu-id="f541c-1476">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1476">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="f541c-1477">ВМ</span><span class="sxs-lookup"><span data-stu-id="f541c-1477">VM</span></span>

* <span data-ttu-id="f541c-1478">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1478">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="f541c-1479">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1479">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="f541c-1480">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1480">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="f541c-1481">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1481">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="f541c-1482">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1482">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="f541c-1483">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1483">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="f541c-1484">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="f541c-1484">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="f541c-1485">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="f541c-1485">February 27, 2017</span></span>

<span data-ttu-id="f541c-1486">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="f541c-1486">Version 2.0.0</span></span>

<span data-ttu-id="f541c-1487">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="f541c-1487">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="f541c-1488">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="f541c-1488">Container Service (acs)</span></span>
- <span data-ttu-id="f541c-1489">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="f541c-1489">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="f541c-1490">Сеть</span><span class="sxs-lookup"><span data-stu-id="f541c-1490">Networking</span></span>
- <span data-ttu-id="f541c-1491">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="f541c-1491">Storage</span></span>

<span data-ttu-id="f541c-1492">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1492">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="f541c-1493">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="f541c-1493">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="f541c-1494">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="f541c-1494">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="f541c-1495">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="f541c-1495">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="f541c-1496">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="f541c-1496">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="f541c-1497">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="f541c-1497">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="f541c-1498">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="f541c-1498">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="f541c-1499">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="f541c-1499">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="f541c-1500">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="f541c-1500">Provide feedback from the command line with the `az feedback` command</span></span>

