---
title: Заметки о выпуске Azure CLI 2.0
description: Узнайте о последних обновлениях в Azure CLI 2.0
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 06/01/2018
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azure-cli
ms.openlocfilehash: 64db2b58ca883518757d8e189bf7263ed818b283
ms.sourcegitcommit: 1a38729d6ae93c49137b3d49b6a9ec8a75eff190
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/19/2018
ms.locfileid: "36262664"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="1368a-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="1368a-103">Azure CLI 2.0 release notes</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="1368a-104">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-104">June 19, 2018</span></span>

<span data-ttu-id="1368a-105">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="1368a-105">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="1368a-106">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-106">Core</span></span>

* <span data-ttu-id="1368a-107">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="1368a-107">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="1368a-108">ACR</span><span class="sxs-lookup"><span data-stu-id="1368a-108">ACR</span></span>

* <span data-ttu-id="1368a-109">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="1368a-109">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="1368a-110">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="1368a-110">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-111">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-111">ACS</span></span>

* <span data-ttu-id="1368a-112">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="1368a-112">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="1368a-113">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-113">Added `--update` support</span></span>
* <span data-ttu-id="1368a-114">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="1368a-114">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="1368a-115">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="1368a-115">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="1368a-116">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="1368a-116">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="1368a-117">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="1368a-117">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="1368a-118">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="1368a-118">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="1368a-119">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="1368a-119">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span> 

### <a name="appservice"></a><span data-ttu-id="1368a-120">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-120">AppService</span></span>

* <span data-ttu-id="1368a-121">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="1368a-121">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="1368a-122">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1368a-122">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="1368a-123">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="1368a-123">Batch</span></span>

* <span data-ttu-id="1368a-124">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="1368a-124">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1368a-125">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="1368a-125">Batch AI</span></span>

* <span data-ttu-id="1368a-126">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="1368a-126">Added support for workspaces.</span></span> <span data-ttu-id="1368a-127">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1368a-127">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="1368a-128">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="1368a-128">Added support for experiments.</span></span> <span data-ttu-id="1368a-129">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="1368a-129">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="1368a-130">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="1368a-130">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="1368a-131">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="1368a-131">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="1368a-132">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="1368a-132">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="1368a-133">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="1368a-133">Added support for `--ids` to `batchai` commands</span></span> 
* <span data-ttu-id="1368a-134">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="1368a-134">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="1368a-135">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="1368a-135">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="1368a-136">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-136">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="1368a-137">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="1368a-137">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="1368a-138">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-138">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="1368a-139">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="1368a-139">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="1368a-140">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="1368a-140">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="1368a-141">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="1368a-141">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="1368a-142">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-142">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="1368a-143">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="1368a-143">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="1368a-144">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="1368a-144">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="1368a-145">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="1368a-145">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="1368a-146">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="1368a-146">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="1368a-147">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="1368a-147">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="1368a-148">Карты</span><span class="sxs-lookup"><span data-stu-id="1368a-148">Maps</span></span>

* <span data-ttu-id="1368a-149">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="1368a-149">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="1368a-150">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-150">Network</span></span>

* <span data-ttu-id="1368a-151">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="1368a-151">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="1368a-152">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="1368a-152">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="1368a-153">#6502</span><span class="sxs-lookup"><span data-stu-id="1368a-153">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="1368a-154">Резервирование</span><span class="sxs-lookup"><span data-stu-id="1368a-154">Reservations</span></span>

* <span data-ttu-id="1368a-155">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-155">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="1368a-156">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-156">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="1368a-157">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="1368a-157">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="1368a-158">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="1368a-158">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="1368a-159">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="1368a-159">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="1368a-160">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-160">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="1368a-161">Роль</span><span class="sxs-lookup"><span data-stu-id="1368a-161">Role</span></span>

* <span data-ttu-id="1368a-162">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="1368a-162">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-163">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-163">SQL</span></span>

* <span data-ttu-id="1368a-164">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="1368a-164">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-165">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-165">Storage</span></span>

* <span data-ttu-id="1368a-166">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="1368a-166">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-167">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-167">VM</span></span>

* <span data-ttu-id="1368a-168">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-168">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="1368a-169">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="1368a-169">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="1368a-170">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="1368a-170">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="1368a-171">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-171">June 13, 2018</span></span>

<span data-ttu-id="1368a-172">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="1368a-172">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="1368a-173">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-173">Core</span></span>

* <span data-ttu-id="1368a-174">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="1368a-174">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="1368a-175">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-175">June 13, 2018</span></span>

<span data-ttu-id="1368a-176">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="1368a-176">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="1368a-177">AKS</span><span class="sxs-lookup"><span data-stu-id="1368a-177">AKS</span></span>

* <span data-ttu-id="1368a-178">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="1368a-178">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="1368a-179">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="1368a-179">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span> 
* <span data-ttu-id="1368a-180">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="1368a-180">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="1368a-181">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="1368a-181">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="1368a-182">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1368a-182">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-183">AppService</span><span class="sxs-lookup"><span data-stu-id="1368a-183">AppService</span></span>

* <span data-ttu-id="1368a-184">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="1368a-184">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="1368a-185">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-185">June 5, 2018</span></span>

<span data-ttu-id="1368a-186">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="1368a-186">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="1368a-187">Interactive</span><span class="sxs-lookup"><span data-stu-id="1368a-187">Interactive</span></span>

* <span data-ttu-id="1368a-188">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="1368a-188">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="1368a-189">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-189">June 5, 2018</span></span>

<span data-ttu-id="1368a-190">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="1368a-190">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="1368a-191">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-191">Core</span></span>

* <span data-ttu-id="1368a-192">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="1368a-192">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="1368a-193">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="1368a-193">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="1368a-194">ACR</span><span class="sxs-lookup"><span data-stu-id="1368a-194">ACR</span></span>

* <span data-ttu-id="1368a-195">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="1368a-195">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="1368a-196">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="1368a-196">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="1368a-197">AKS</span><span class="sxs-lookup"><span data-stu-id="1368a-197">AKS</span></span>

* <span data-ttu-id="1368a-198">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="1368a-198">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="1368a-199">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="1368a-199">Batch</span></span>

* <span data-ttu-id="1368a-200">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="1368a-200">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="1368a-201">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="1368a-201">IOT</span></span>

* <span data-ttu-id="1368a-202">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="1368a-202">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="1368a-203">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-203">Network</span></span>

* <span data-ttu-id="1368a-204">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="1368a-204">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="1368a-205">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="1368a-205">Policy Insights</span></span>

* <span data-ttu-id="1368a-206">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="1368a-206">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="1368a-207">ARM</span><span class="sxs-lookup"><span data-stu-id="1368a-207">ARM</span></span>

* <span data-ttu-id="1368a-208">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="1368a-208">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-209">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-209">SQL</span></span>

* <span data-ttu-id="1368a-210">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="1368a-210">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="1368a-211">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="1368a-211">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="1368a-212">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-212">Storage</span></span>

* <span data-ttu-id="1368a-213">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="1368a-213">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-214">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-214">VM</span></span>

* <span data-ttu-id="1368a-215">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="1368a-215">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="1368a-216">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-216">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="1368a-217">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-217">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="1368a-218">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-218">May 22, 2018</span></span>

<span data-ttu-id="1368a-219">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="1368a-219">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="1368a-220">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-220">Core</span></span>

* <span data-ttu-id="1368a-221">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="1368a-221">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-222">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-222">ACS</span></span>

* <span data-ttu-id="1368a-223">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="1368a-223">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="1368a-224">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="1368a-224">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-225">AppService</span><span class="sxs-lookup"><span data-stu-id="1368a-225">AppService</span></span>

* <span data-ttu-id="1368a-226">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="1368a-226">Improved generic update commands</span></span>
* <span data-ttu-id="1368a-227">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="1368a-227">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="1368a-228">Контейнер</span><span class="sxs-lookup"><span data-stu-id="1368a-228">Container</span></span>

* <span data-ttu-id="1368a-229">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="1368a-229">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="1368a-230">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="1368a-230">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="1368a-231">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="1368a-231">Extension</span></span>

* <span data-ttu-id="1368a-232">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="1368a-232">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="1368a-233">Interactive</span><span class="sxs-lookup"><span data-stu-id="1368a-233">Interactive</span></span>

* <span data-ttu-id="1368a-234">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="1368a-234">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="1368a-235">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="1368a-235">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="1368a-236">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="1368a-236">KeyVault</span></span>

* <span data-ttu-id="1368a-237">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="1368a-237">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="1368a-238">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-238">Network</span></span>

* <span data-ttu-id="1368a-239">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="1368a-239">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="1368a-240">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="1368a-240">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-241">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-241">SQL</span></span>

* <span data-ttu-id="1368a-242">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="1368a-242">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="1368a-243">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="1368a-243">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="1368a-244">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="1368a-244">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span> 
    * <span data-ttu-id="1368a-245">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="1368a-245">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="1368a-246">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="1368a-246">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="1368a-247">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="1368a-247">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="1368a-248">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="1368a-248">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="1368a-249">`edition`.</span><span class="sxs-lookup"><span data-stu-id="1368a-249">`edition`.</span></span> <span data-ttu-id="1368a-250">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="1368a-250">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="1368a-251">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="1368a-251">`elasticPoolName`.</span></span> <span data-ttu-id="1368a-252">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="1368a-252">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="1368a-253">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="1368a-253">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="1368a-254">`edition`.</span><span class="sxs-lookup"><span data-stu-id="1368a-254">`edition`.</span></span> <span data-ttu-id="1368a-255">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="1368a-255">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="1368a-256">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="1368a-256">`dtu`.</span></span> <span data-ttu-id="1368a-257">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="1368a-257">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="1368a-258">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="1368a-258">`databaseDtuMin`.</span></span> <span data-ttu-id="1368a-259">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="1368a-259">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="1368a-260">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="1368a-260">`databaseDtuMax`.</span></span> <span data-ttu-id="1368a-261">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="1368a-261">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="1368a-262">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="1368a-262">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="1368a-263">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="1368a-263">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-264">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-264">Storage</span></span>

* <span data-ttu-id="1368a-265">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="1368a-265">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="1368a-266">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="1368a-266">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-267">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-267">VM</span></span>

* <span data-ttu-id="1368a-268">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-268">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="1368a-269">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="1368a-269">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="1368a-270">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="1368a-270">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="1368a-271">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="1368a-271">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="1368a-272">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-272">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="1368a-273">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-273">May 7, 2018</span></span>

<span data-ttu-id="1368a-274">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="1368a-274">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="1368a-275">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-275">Core</span></span>

* <span data-ttu-id="1368a-276">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="1368a-276">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="1368a-277">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="1368a-277">Added limited support for positional arguments</span></span>
* <span data-ttu-id="1368a-278">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="1368a-278">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="1368a-279">#5591</span><span class="sxs-lookup"><span data-stu-id="1368a-279">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="1368a-280">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="1368a-280">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="1368a-281">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="1368a-281">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="1368a-282">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="1368a-282">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="1368a-283">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="1368a-283">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="1368a-284">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="1368a-284">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="1368a-285">ACR</span><span class="sxs-lookup"><span data-stu-id="1368a-285">ACR</span></span>

* <span data-ttu-id="1368a-286">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="1368a-286">Added ACR Build commands</span></span>
* <span data-ttu-id="1368a-287">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="1368a-287">Improved resource not found error messages</span></span>
* <span data-ttu-id="1368a-288">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="1368a-288">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="1368a-289">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="1368a-289">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="1368a-290">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="1368a-290">Improved repository commands error messages</span></span>
* <span data-ttu-id="1368a-291">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="1368a-291">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-292">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-292">ACS</span></span>

* <span data-ttu-id="1368a-293">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="1368a-293">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="1368a-294">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="1368a-294">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="1368a-295">AMS</span><span class="sxs-lookup"><span data-stu-id="1368a-295">AMS</span></span>

* <span data-ttu-id="1368a-296">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="1368a-296">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-297">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-297">Appservice</span></span>

* <span data-ttu-id="1368a-298">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="1368a-298">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="1368a-299">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-299">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="1368a-300">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="1368a-300">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="1368a-301">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="1368a-301">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="1368a-302">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="1368a-302">Batch AI</span></span>

* <span data-ttu-id="1368a-303">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="1368a-303">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1368a-304">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1368a-304">Cognitive Services</span></span>

* <span data-ttu-id="1368a-305">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="1368a-305">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="1368a-306">Потребление</span><span class="sxs-lookup"><span data-stu-id="1368a-306">Consumption</span></span>

* <span data-ttu-id="1368a-307">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="1368a-307">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="1368a-308">Контейнер</span><span class="sxs-lookup"><span data-stu-id="1368a-308">Container</span></span>

* <span data-ttu-id="1368a-309">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="1368a-309">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="1368a-310">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="1368a-310">Cosmos DB</span></span>

* <span data-ttu-id="1368a-311">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1368a-311">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="1368a-312">DMS</span><span class="sxs-lookup"><span data-stu-id="1368a-312">DMS</span></span>

* <span data-ttu-id="1368a-313">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="1368a-313">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="1368a-314">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="1368a-314">Extension</span></span>

* <span data-ttu-id="1368a-315">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="1368a-315">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="1368a-316">Interactive</span><span class="sxs-lookup"><span data-stu-id="1368a-316">Interactive</span></span>

* <span data-ttu-id="1368a-317">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="1368a-317">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="1368a-318">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="1368a-318">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="1368a-319">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="1368a-319">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="1368a-320">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="1368a-320">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="1368a-321">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="1368a-321">Lab</span></span>

* <span data-ttu-id="1368a-322">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="1368a-322">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="1368a-323">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-323">Network</span></span>

* <span data-ttu-id="1368a-324">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="1368a-324">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span> 
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="1368a-325">Профиль</span><span class="sxs-lookup"><span data-stu-id="1368a-325">Profile</span></span>

* <span data-ttu-id="1368a-326">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-326">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="1368a-327">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="1368a-327">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="1368a-328">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="1368a-328">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="1368a-329">Redis</span><span class="sxs-lookup"><span data-stu-id="1368a-329">Redis</span></span>

* <span data-ttu-id="1368a-330">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-330">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="1368a-331">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="1368a-331">Deprecated `redis list-all`.</span></span> <span data-ttu-id="1368a-332">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="1368a-332">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="1368a-333">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="1368a-333">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="1368a-334">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="1368a-334">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="1368a-335">Роль</span><span class="sxs-lookup"><span data-stu-id="1368a-335">Role</span></span>

* <span data-ttu-id="1368a-336">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="1368a-336">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-337">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-337">Storage</span></span>

* <span data-ttu-id="1368a-338">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="1368a-338">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="1368a-339">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="1368a-339">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="1368a-340">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="1368a-340">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="1368a-341">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="1368a-341">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="1368a-342">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="1368a-342">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-343">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-343">VM</span></span>

* <span data-ttu-id="1368a-344">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="1368a-344">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="1368a-345">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="1368a-345">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="1368a-346">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="1368a-346">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="1368a-347">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="1368a-347">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="1368a-348">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="1368a-348">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="1368a-349">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="1368a-349">Added write accelerator support</span></span> 
* <span data-ttu-id="1368a-350">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="1368a-350">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="1368a-351">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="1368a-351">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="1368a-352">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="1368a-352">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="1368a-353">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-353">April 10, 2018</span></span>

<span data-ttu-id="1368a-354">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="1368a-354">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="1368a-355">ACR</span><span class="sxs-lookup"><span data-stu-id="1368a-355">ACR</span></span>

* <span data-ttu-id="1368a-356">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="1368a-356">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-357">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-357">ACS</span></span>

* <span data-ttu-id="1368a-358">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="1368a-358">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-359">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-359">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="1368a-361">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="1368a-361">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="1368a-362">Batch AI</span><span class="sxs-lookup"><span data-stu-id="1368a-362">BatchAI</span></span>

* <span data-ttu-id="1368a-363">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="1368a-363">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="1368a-364">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="1368a-364">Job level mounting</span></span>
 - <span data-ttu-id="1368a-365">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="1368a-365">Environment variables with secret values</span></span>
 - <span data-ttu-id="1368a-366">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="1368a-366">Performance counters settings</span></span>
 - <span data-ttu-id="1368a-367">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="1368a-367">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="1368a-368">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="1368a-368">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="1368a-369">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="1368a-369">Usage and limits reporting</span></span>
 - <span data-ttu-id="1368a-370">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="1368a-370">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="1368a-371">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="1368a-371">Support for custom images</span></span>
 - <span data-ttu-id="1368a-372">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="1368a-372">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="1368a-373">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="1368a-373">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="1368a-374">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="1368a-374">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="1368a-375">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="1368a-375">National clouds are supported</span></span>
* <span data-ttu-id="1368a-376">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="1368a-376">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="1368a-377">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="1368a-377">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="1368a-378">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="1368a-378">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="1368a-379">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="1368a-379">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="1368a-380">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="1368a-380">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="1368a-381">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="1368a-381">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="1368a-382">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-382">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="1368a-383">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="1368a-383">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="1368a-384">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="1368a-384">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="1368a-385">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-385">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="1368a-386">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="1368a-386">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="1368a-387">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="1368a-387">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="1368a-388">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-388">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="1368a-389">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="1368a-389">Billing</span></span>

* <span data-ttu-id="1368a-390">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="1368a-390">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="1368a-391">Потребление</span><span class="sxs-lookup"><span data-stu-id="1368a-391">Consumption</span></span>

* <span data-ttu-id="1368a-392">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="1368a-392">Added `marketplace` commands</span></span>
* <span data-ttu-id="1368a-393">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="1368a-393">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="1368a-394">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="1368a-394">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="1368a-395">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="1368a-395">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="1368a-396">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="1368a-396">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="1368a-397">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="1368a-397">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="1368a-398">Контейнер</span><span class="sxs-lookup"><span data-stu-id="1368a-398">Container</span></span>

* <span data-ttu-id="1368a-399">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="1368a-399">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="1368a-400">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="1368a-400">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="1368a-401">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="1368a-401">Extension</span></span>

* <span data-ttu-id="1368a-402">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="1368a-402">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="1368a-403">Interactive</span><span class="sxs-lookup"><span data-stu-id="1368a-403">Interactive</span></span>

* <span data-ttu-id="1368a-404">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="1368a-404">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="1368a-405">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="1368a-405">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="1368a-406">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="1368a-406">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="1368a-407">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-407">Network</span></span>

* <span data-ttu-id="1368a-408">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-408">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="1368a-409">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-409">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="1368a-410">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="1368a-410">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="1368a-411">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="1368a-411">Added `ddos-protection` commands to create DDoS protection plans</span></span> 
* <span data-ttu-id="1368a-412">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="1368a-412">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="1368a-413">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-413">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="1368a-414">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-414">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="1368a-415">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="1368a-415">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="1368a-416">Профиль</span><span class="sxs-lookup"><span data-stu-id="1368a-416">Profile</span></span>

* <span data-ttu-id="1368a-417">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="1368a-417">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="1368a-418">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="1368a-418">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="1368a-419">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="1368a-419">RDBMS</span></span>

* <span data-ttu-id="1368a-420">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="1368a-420">Added `georestore` command</span></span>
* <span data-ttu-id="1368a-421">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="1368a-421">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-422">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-422">Resource</span></span>

* <span data-ttu-id="1368a-423">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-423">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="1368a-424">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-424">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-425">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-425">SQL</span></span>

* <span data-ttu-id="1368a-426">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="1368a-426">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-427">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-427">Storage</span></span>

* <span data-ttu-id="1368a-428">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="1368a-428">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-429">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-429">VM</span></span>

* <span data-ttu-id="1368a-430">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="1368a-430">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="1368a-431">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="1368a-431">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="1368a-433">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-433">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="1368a-434">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="1368a-434">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="1368a-435">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="1368a-435">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="1368a-436">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="1368a-436">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="1368a-437">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-437">March 27, 2018</span></span>

<span data-ttu-id="1368a-438">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="1368a-438">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="1368a-439">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-439">Core</span></span>

* <span data-ttu-id="1368a-440">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="1368a-440">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-441">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-441">ACS</span></span>

* <span data-ttu-id="1368a-442">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="1368a-442">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-443">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-443">Appservice</span></span>

* <span data-ttu-id="1368a-444">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-444">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="1368a-445">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-445">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="1368a-446">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="1368a-446">Backup</span></span>

* <span data-ttu-id="1368a-447">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="1368a-447">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="1368a-448">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="1368a-448">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="1368a-449">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="1368a-449">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="1368a-450">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-450">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="1368a-451">Контейнер</span><span class="sxs-lookup"><span data-stu-id="1368a-451">Container</span></span>

* <span data-ttu-id="1368a-452">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="1368a-452">Added `container exec` command.</span></span> <span data-ttu-id="1368a-453">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="1368a-453">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="1368a-454">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="1368a-454">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="1368a-455">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="1368a-455">Extension</span></span>

* <span data-ttu-id="1368a-456">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="1368a-456">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="1368a-457">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="1368a-457">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="1368a-458">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1368a-458">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="1368a-459">Interactive</span><span class="sxs-lookup"><span data-stu-id="1368a-459">Interactive</span></span>

* <span data-ttu-id="1368a-460">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="1368a-460">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="1368a-461">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="1368a-461">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="1368a-462">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="1368a-462">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="1368a-463">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="1368a-463">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="1368a-464">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="1368a-464">Lab</span></span>

* <span data-ttu-id="1368a-465">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="1368a-465">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="1368a-466">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="1368a-466">Monitor</span></span>

* <span data-ttu-id="1368a-467">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="1368a-467">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="1368a-468">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="1368a-468">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="1368a-469">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="1368a-469">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="1368a-470">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-470">Network</span></span>

* <span data-ttu-id="1368a-471">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="1368a-471">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="1368a-472">Профиль</span><span class="sxs-lookup"><span data-stu-id="1368a-472">Profile</span></span>

* <span data-ttu-id="1368a-473">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="1368a-473">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="1368a-474">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="1368a-474">RDBMS</span></span>

* <span data-ttu-id="1368a-475">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="1368a-475">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-476">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-476">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="1368a-478">Роль</span><span class="sxs-lookup"><span data-stu-id="1368a-478">Role</span></span>

* <span data-ttu-id="1368a-479">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-479">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="1368a-480">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="1368a-480">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="1368a-481">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="1368a-481">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="1368a-482">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-482">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="1368a-483">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="1368a-483">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-484">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-484">Storage</span></span>

* <span data-ttu-id="1368a-485">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="1368a-485">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="1368a-486">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="1368a-486">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-487">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-487">VM</span></span>

* <span data-ttu-id="1368a-488">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="1368a-488">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="1368a-489">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-489">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="1368a-490">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="1368a-490">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="1368a-491">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="1368a-491">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="1368a-492">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-492">March 13, 2018</span></span>

<span data-ttu-id="1368a-493">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="1368a-493">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="1368a-494">ACR</span><span class="sxs-lookup"><span data-stu-id="1368a-494">ACR</span></span>

* <span data-ttu-id="1368a-495">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="1368a-495">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="1368a-496">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="1368a-496">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="1368a-497">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="1368a-497">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-498">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-498">ACS</span></span>

* <span data-ttu-id="1368a-499">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="1368a-499">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="1368a-500">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="1368a-500">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="1368a-501">Помощник</span><span class="sxs-lookup"><span data-stu-id="1368a-501">Advisor</span></span>

* <span data-ttu-id="1368a-502">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="1368a-502">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="1368a-503">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-503">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="1368a-504">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="1368a-504">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span> 
* <span data-ttu-id="1368a-505">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="1368a-505">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="1368a-506">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-506">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-507">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-507">Appservice</span></span>

* <span data-ttu-id="1368a-508">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="1368a-508">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="1368a-509">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-509">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="1368a-510">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="1368a-510">Eventhubs</span></span>

* <span data-ttu-id="1368a-511">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="1368a-511">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="1368a-512">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="1368a-512">Extension</span></span>

* <span data-ttu-id="1368a-513">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="1368a-513">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="1368a-514">Interactive</span><span class="sxs-lookup"><span data-stu-id="1368a-514">Interactive</span></span>

* <span data-ttu-id="1368a-515">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="1368a-515">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="1368a-516">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="1368a-516">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="1368a-517">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="1368a-517">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="1368a-518">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="1368a-518">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="1368a-519">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="1368a-519">Monitor</span></span>

* <span data-ttu-id="1368a-520">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="1368a-520">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="1368a-521">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="1368a-521">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="1368a-522">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="1368a-522">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="1368a-523">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="1368a-523">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="1368a-524">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-524">Network</span></span>

* <span data-ttu-id="1368a-525">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-525">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="1368a-526">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="1368a-526">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="1368a-527">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="1368a-527">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="1368a-528">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="1368a-528">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="1368a-529">Профиль</span><span class="sxs-lookup"><span data-stu-id="1368a-529">Profile</span></span>

* <span data-ttu-id="1368a-530">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="1368a-530">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="1368a-531">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="1368a-531">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="1368a-532">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="1368a-532">RDBMS</span></span>

* <span data-ttu-id="1368a-533">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="1368a-533">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="1368a-534">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="1368a-534">Service Bus</span></span>

* <span data-ttu-id="1368a-535">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="1368a-535">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-536">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-536">Storage</span></span>

* <span data-ttu-id="1368a-537">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="1368a-537">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="1368a-538">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="1368a-538">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-539">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-539">VM</span></span>

* <span data-ttu-id="1368a-540">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="1368a-540">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="1368a-541">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="1368a-541">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="1368a-542">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-542">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="1368a-543">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="1368a-543">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="1368a-544">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="1368a-544">February 27, 2018</span></span>

<span data-ttu-id="1368a-545">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="1368a-545">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="1368a-546">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-546">Core</span></span>

* <span data-ttu-id="1368a-547">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="1368a-547">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="1368a-548">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="1368a-548">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="1368a-549">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="1368a-549">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-550">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-550">ACS</span></span>

* <span data-ttu-id="1368a-551">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1368a-551">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="1368a-552">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="1368a-552">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="1368a-553">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="1368a-553">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="1368a-554">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="1368a-554">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-555">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-555">Appservice</span></span>

* <span data-ttu-id="1368a-556">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="1368a-556">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="1368a-557">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="1368a-557">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="1368a-558">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="1368a-558">Cognitive Services</span></span>

* <span data-ttu-id="1368a-559">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="1368a-559">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="1368a-560">Потребление</span><span class="sxs-lookup"><span data-stu-id="1368a-560">Consumption</span></span>

* <span data-ttu-id="1368a-561">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="1368a-561">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="1368a-562">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="1368a-562">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="1368a-563">Контейнер</span><span class="sxs-lookup"><span data-stu-id="1368a-563">Container</span></span>

* <span data-ttu-id="1368a-564">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="1368a-564">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="1368a-565">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-565">Network</span></span>

* <span data-ttu-id="1368a-566">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="1368a-566">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-567">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-567">Resource</span></span>

* <span data-ttu-id="1368a-568">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="1368a-568">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="1368a-569">Роль</span><span class="sxs-lookup"><span data-stu-id="1368a-569">Role</span></span>

* <span data-ttu-id="1368a-570">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="1368a-570">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-571">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-571">SQL</span></span>

* <span data-ttu-id="1368a-572">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="1368a-572">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-573">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-573">Storage</span></span>

* <span data-ttu-id="1368a-574">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-574">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-575">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-575">VM</span></span>

* <span data-ttu-id="1368a-576">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="1368a-576">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="1368a-577">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-577">February 13, 2018</span></span>

<span data-ttu-id="1368a-578">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="1368a-578">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="1368a-579">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-579">Core</span></span>

* <span data-ttu-id="1368a-580">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="1368a-580">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-581">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-581">ACS</span></span>

* <span data-ttu-id="1368a-582">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="1368a-582">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="1368a-583">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-583">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="1368a-584">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="1368a-584">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="1368a-585">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="1368a-585">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="1368a-586">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="1368a-586">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="1368a-587">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="1368a-587">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="1368a-588">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="1368a-588">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="1368a-589">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="1368a-589">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-590">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-590">Appservice</span></span>

* <span data-ttu-id="1368a-591">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="1368a-591">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="1368a-592">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="1368a-592">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="1368a-593">CDN</span><span class="sxs-lookup"><span data-stu-id="1368a-593">CDN</span></span>

* <span data-ttu-id="1368a-594">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-594">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="1368a-595">Контейнер</span><span class="sxs-lookup"><span data-stu-id="1368a-595">Container</span></span>

* <span data-ttu-id="1368a-596">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="1368a-596">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="1368a-597">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="1368a-597">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1368a-598">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1368a-598">CosmosDB</span></span>

* <span data-ttu-id="1368a-599">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="1368a-599">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="1368a-600">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="1368a-600">Extension</span></span>

* <span data-ttu-id="1368a-601">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-601">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="1368a-602">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-602">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="1368a-603">Отзыв</span><span class="sxs-lookup"><span data-stu-id="1368a-603">Feedback</span></span>

* <span data-ttu-id="1368a-604">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="1368a-604">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="1368a-605">Interactive</span><span class="sxs-lookup"><span data-stu-id="1368a-605">Interactive</span></span>

* <span data-ttu-id="1368a-606">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="1368a-606">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="1368a-607">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="1368a-607">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="1368a-608">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="1368a-608">IoT</span></span>

* <span data-ttu-id="1368a-609">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="1368a-609">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="1368a-610">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="1368a-610">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="1368a-611">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-611">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="1368a-612">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="1368a-612">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="1368a-613">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="1368a-613">Monitor</span></span>

* <span data-ttu-id="1368a-614">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-614">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="1368a-615">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-615">Network</span></span>

* <span data-ttu-id="1368a-616">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="1368a-616">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="1368a-617">Профиль</span><span class="sxs-lookup"><span data-stu-id="1368a-617">Profile</span></span>

* <span data-ttu-id="1368a-618">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="1368a-618">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-619">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-619">Resource</span></span>

* <span data-ttu-id="1368a-620">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-620">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="1368a-621">Роль</span><span class="sxs-lookup"><span data-stu-id="1368a-621">Role</span></span>

* <span data-ttu-id="1368a-622">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="1368a-622">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-623">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-623">SQL</span></span>

* <span data-ttu-id="1368a-624">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="1368a-624">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="1368a-625">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="1368a-625">Added `sql db rename`</span></span>
* <span data-ttu-id="1368a-626">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="1368a-626">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-627">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-627">Storage</span></span>

* <span data-ttu-id="1368a-628">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="1368a-628">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-629">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-629">VM</span></span>

* <span data-ttu-id="1368a-630">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="1368a-630">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="1368a-631">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="1368a-631">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="1368a-632">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="1368a-632">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="1368a-633">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-633">January 31, 2018</span></span>

<span data-ttu-id="1368a-634">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="1368a-634">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="1368a-635">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-635">Core</span></span>

* <span data-ttu-id="1368a-636">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="1368a-636">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="1368a-637">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="1368a-637">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="1368a-638">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="1368a-638">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="1368a-639">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="1368a-639">Use `--verbose` to see</span></span>
* <span data-ttu-id="1368a-640">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="1368a-640">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-641">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-641">ACS</span></span>

* <span data-ttu-id="1368a-642">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="1368a-642">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="1368a-643">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="1368a-643">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-644">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-644">Appservice</span></span>

* <span data-ttu-id="1368a-645">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="1368a-645">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="1368a-646">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="1368a-646">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="1368a-647">CDN</span><span class="sxs-lookup"><span data-stu-id="1368a-647">CDN</span></span>

* <span data-ttu-id="1368a-648">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-648">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1368a-649">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1368a-649">CosmosDB</span></span>

* <span data-ttu-id="1368a-650">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="1368a-650">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="1368a-651">Interactive</span><span class="sxs-lookup"><span data-stu-id="1368a-651">Interactive</span></span>

* <span data-ttu-id="1368a-652">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="1368a-652">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="1368a-653">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-653">Network</span></span>

* <span data-ttu-id="1368a-654">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-654">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="1368a-655">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1368a-655">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="1368a-656">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-656">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="1368a-657">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-657">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="1368a-658">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="1368a-658">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="1368a-659">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="1368a-659">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="1368a-660">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="1368a-660">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="1368a-661">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="1368a-661">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="1368a-662">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="1368a-662">Fixed issue where certain records were imported twice with `dns zone import`</span></span> 
* <span data-ttu-id="1368a-663">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="1368a-663">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="1368a-664">Профиль</span><span class="sxs-lookup"><span data-stu-id="1368a-664">Profile</span></span>

* <span data-ttu-id="1368a-665">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="1368a-665">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-666">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-666">Resource</span></span>

* <span data-ttu-id="1368a-667">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="1368a-667">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-668">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-668">Storage</span></span>

* <span data-ttu-id="1368a-669">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="1368a-669">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="1368a-670">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="1368a-670">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="1368a-671">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="1368a-671">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>  
* <span data-ttu-id="1368a-672">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-672">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="1368a-673">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="1368a-673">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-674">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-674">VM</span></span>

* <span data-ttu-id="1368a-675">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="1368a-675">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="1368a-676">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="1368a-676">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="1368a-677">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="1368a-677">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="1368a-678">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-678">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="1368a-679">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-679">January 17, 2018</span></span>

<span data-ttu-id="1368a-680">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="1368a-680">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="1368a-681">ACR</span><span class="sxs-lookup"><span data-stu-id="1368a-681">ACR</span></span>

* <span data-ttu-id="1368a-682">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="1368a-682">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="1368a-683">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="1368a-683">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-684">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-684">ACS</span></span>

* <span data-ttu-id="1368a-685">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="1368a-685">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="1368a-686">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="1368a-686">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-687">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-687">Appservice</span></span>

* <span data-ttu-id="1368a-688">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="1368a-688">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="1368a-689">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="1368a-689">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="1368a-690">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="1368a-690">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="1368a-691">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="1368a-691">Backup</span></span>

* <span data-ttu-id="1368a-692">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="1368a-692">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="1368a-693">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="1368a-693">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="1368a-694">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="1368a-694">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="1368a-695">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="1368a-695">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="1368a-696">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="1368a-696">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="1368a-697">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="1368a-697">Batch</span></span>

* <span data-ttu-id="1368a-698">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="1368a-698">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="1368a-699">Облако</span><span class="sxs-lookup"><span data-stu-id="1368a-699">Cloud</span></span>

* <span data-ttu-id="1368a-700">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="1368a-700">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="1368a-701">Потребление</span><span class="sxs-lookup"><span data-stu-id="1368a-701">Consumption</span></span>

* <span data-ttu-id="1368a-702">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="1368a-702">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="1368a-703">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="1368a-703">Event Grid</span></span>

* <span data-ttu-id="1368a-704">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="1368a-704">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="1368a-705">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="1368a-705">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="1368a-706">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="1368a-706">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="1368a-707">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="1368a-707">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="1368a-708">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-708">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="1368a-709">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-709">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="1368a-710">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="1368a-710">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="1368a-711">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="1368a-711">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="1368a-712">Interactive</span><span class="sxs-lookup"><span data-stu-id="1368a-712">Interactive</span></span>

* <span data-ttu-id="1368a-713">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="1368a-713">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="1368a-714">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="1368a-714">Fixed errors on startup</span></span>
* <span data-ttu-id="1368a-715">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="1368a-715">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="1368a-716">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="1368a-716">IoT</span></span>

* <span data-ttu-id="1368a-717">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="1368a-717">Added support for device provisioning service</span></span>
* <span data-ttu-id="1368a-718">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="1368a-718">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="1368a-719">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="1368a-719">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="1368a-720">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="1368a-720">Monitor</span></span>

* <span data-ttu-id="1368a-721">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="1368a-721">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="1368a-722">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-722">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="1368a-723">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="1368a-723">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="1368a-724">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-724">Network</span></span>

* <span data-ttu-id="1368a-725">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="1368a-725">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="1368a-726">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="1368a-726">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="1368a-727">Профиль</span><span class="sxs-lookup"><span data-stu-id="1368a-727">Profile</span></span>

* <span data-ttu-id="1368a-728">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="1368a-728">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="1368a-729">Роль</span><span class="sxs-lookup"><span data-stu-id="1368a-729">Role</span></span>

* <span data-ttu-id="1368a-730">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="1368a-730">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1368a-731">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1368a-731">Service Fabric</span></span>

* <span data-ttu-id="1368a-732">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="1368a-732">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="1368a-733">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="1368a-733">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-734">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-734">VM</span></span>

* <span data-ttu-id="1368a-735">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="1368a-735">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="1368a-736">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="1368a-736">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="1368a-737">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="1368a-737">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="1368a-738">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="1368a-738">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="1368a-739">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="1368a-739">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="1368a-740">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="1368a-740">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="1368a-741">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-741">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="1368a-742">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="1368a-742">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="1368a-743">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-743">December 19, 2017</span></span>

<span data-ttu-id="1368a-744">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="1368a-744">Version 2.0.23</span></span>

* <span data-ttu-id="1368a-745">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="1368a-745">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="1368a-746">Контейнер</span><span class="sxs-lookup"><span data-stu-id="1368a-746">Container</span></span>

* <span data-ttu-id="1368a-747">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="1368a-747">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="1368a-748">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-748">Network</span></span>

* <span data-ttu-id="1368a-749">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1368a-749">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="1368a-750">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1368a-750">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-751">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-751">Storage</span></span>

* <span data-ttu-id="1368a-752">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="1368a-752">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-753">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-753">VM</span></span>

* <span data-ttu-id="1368a-754">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="1368a-754">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="1368a-755">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-755">December 5, 2017</span></span>

<span data-ttu-id="1368a-756">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="1368a-756">Version 2.0.22</span></span>

* <span data-ttu-id="1368a-757">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="1368a-757">Removed `az component` commands.</span></span> <span data-ttu-id="1368a-758">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="1368a-758">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="1368a-759">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-759">Core</span></span>
* <span data-ttu-id="1368a-760">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="1368a-760">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="1368a-761">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="1368a-761">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-762">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-762">ACS</span></span>

* <span data-ttu-id="1368a-763">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="1368a-763">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="1368a-764">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-764">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="1368a-765">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="1368a-765">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="1368a-766">Помощник</span><span class="sxs-lookup"><span data-stu-id="1368a-766">Advisor</span></span>

* <span data-ttu-id="1368a-767">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="1368a-767">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-768">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-768">Appservice</span></span>

* <span data-ttu-id="1368a-769">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="1368a-769">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="1368a-770">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="1368a-770">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="1368a-771">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="1368a-771">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="1368a-772">Потребление</span><span class="sxs-lookup"><span data-stu-id="1368a-772">Consumption</span></span>

* <span data-ttu-id="1368a-773">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="1368a-773">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="1368a-774">Контейнер</span><span class="sxs-lookup"><span data-stu-id="1368a-774">Container</span></span>

* <span data-ttu-id="1368a-775">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="1368a-775">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="1368a-776">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="1368a-776">Monitor</span></span>

* <span data-ttu-id="1368a-777">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="1368a-777">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-778">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-778">Resource</span></span>

* <span data-ttu-id="1368a-779">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="1368a-779">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="1368a-780">Роль</span><span class="sxs-lookup"><span data-stu-id="1368a-780">Role</span></span>

* <span data-ttu-id="1368a-781">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="1368a-781">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="1368a-782">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="1368a-782">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="1368a-783">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="1368a-783">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-784">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-784">SQL</span></span>

* <span data-ttu-id="1368a-785">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="1368a-785">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="1368a-786">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-786">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-787">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-787">VM</span></span>

* <span data-ttu-id="1368a-788">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="1368a-788">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="1368a-789">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-789">November 14, 2017</span></span>

<span data-ttu-id="1368a-790">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="1368a-790">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="1368a-791">ACR</span><span class="sxs-lookup"><span data-stu-id="1368a-791">ACR</span></span>

* <span data-ttu-id="1368a-792">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="1368a-792">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="1368a-793">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-793">ACS</span></span>

* <span data-ttu-id="1368a-794">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="1368a-794">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="1368a-795">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="1368a-795">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="1368a-796">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="1368a-796">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="1368a-797">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="1368a-797">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="1368a-798">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="1368a-798">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-799">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-799">Appservice</span></span>

* <span data-ttu-id="1368a-800">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="1368a-800">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="1368a-801">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="1368a-801">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="1368a-802">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="1368a-802">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="1368a-803">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="1368a-803">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="1368a-804">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="1368a-804">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="1368a-805">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="1368a-805">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="1368a-806">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="1368a-806">Batch</span></span>

* <span data-ttu-id="1368a-807">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="1368a-807">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="1368a-808">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="1368a-808">Batchai</span></span>

* <span data-ttu-id="1368a-809">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-809">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="1368a-810">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-810">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="1368a-811">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="1368a-811">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="1368a-812">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-812">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="1368a-813">Облако</span><span class="sxs-lookup"><span data-stu-id="1368a-813">Cloud</span></span>

* <span data-ttu-id="1368a-814">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="1368a-814">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="1368a-815">Контейнер</span><span class="sxs-lookup"><span data-stu-id="1368a-815">Container</span></span>

* <span data-ttu-id="1368a-816">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="1368a-816">Added support to open multiple ports</span></span>
* <span data-ttu-id="1368a-817">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="1368a-817">Added container group restart policy</span></span>
* <span data-ttu-id="1368a-818">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="1368a-818">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="1368a-819">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="1368a-819">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1368a-820">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1368a-820">Data Lake Analytics</span></span>

* <span data-ttu-id="1368a-821">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="1368a-821">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1368a-822">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1368a-822">Data Lake Store</span></span>

* <span data-ttu-id="1368a-823">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="1368a-823">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="1368a-824">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="1368a-824">Extension</span></span>

* <span data-ttu-id="1368a-825">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="1368a-825">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="1368a-826">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="1368a-826">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="1368a-827">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="1368a-827">IoT</span></span>

* <span data-ttu-id="1368a-828">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="1368a-828">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="1368a-829">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="1368a-829">Monitor</span></span>

* <span data-ttu-id="1368a-830">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="1368a-830">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="1368a-831">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-831">Network</span></span>

* <span data-ttu-id="1368a-832">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="1368a-832">Added support for CAA DNS records</span></span>
* <span data-ttu-id="1368a-833">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-833">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="1368a-834">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="1368a-834">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="1368a-835">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="1368a-835">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="1368a-836">Резервирование</span><span class="sxs-lookup"><span data-stu-id="1368a-836">Reservations</span></span>

* <span data-ttu-id="1368a-837">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="1368a-837">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-838">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-838">Resource</span></span>

* <span data-ttu-id="1368a-839">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="1368a-839">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-840">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-840">SQL</span></span>

* <span data-ttu-id="1368a-841">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-841">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-842">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-842">Storage</span></span>

* <span data-ttu-id="1368a-843">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1368a-843">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="1368a-844">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="1368a-844">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="1368a-845">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="1368a-845">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="1368a-846">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="1368a-846">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="1368a-847">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-847">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="1368a-848">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="1368a-848">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="1368a-849">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-849">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-850">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-850">VM</span></span>

* <span data-ttu-id="1368a-851">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="1368a-851">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="1368a-852">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="1368a-852">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="1368a-853">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="1368a-853">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="1368a-854">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="1368a-854">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="1368a-855">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="1368a-855">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="1368a-856">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-856">October 24, 2017</span></span>

<span data-ttu-id="1368a-857">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="1368a-857">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="1368a-858">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-858">Core</span></span>

* <span data-ttu-id="1368a-859">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="1368a-859">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="1368a-860">ACR</span><span class="sxs-lookup"><span data-stu-id="1368a-860">ACR</span></span>

* <span data-ttu-id="1368a-861">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="1368a-861">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="1368a-862">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="1368a-862">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="1368a-863">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="1368a-863">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-864">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-864">ACS</span></span>

* <span data-ttu-id="1368a-865">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="1368a-865">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="1368a-866">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="1368a-866">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-867">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-867">Appservice</span></span>

* <span data-ttu-id="1368a-868">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="1368a-868">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="1368a-869">Компонент</span><span class="sxs-lookup"><span data-stu-id="1368a-869">Component</span></span>

* <span data-ttu-id="1368a-870">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="1368a-870">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="1368a-871">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="1368a-871">Monitor</span></span>

* <span data-ttu-id="1368a-872">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="1368a-872">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-873">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-873">Resource</span></span>

* <span data-ttu-id="1368a-874">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="1368a-874">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="1368a-875">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="1368a-875">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-876">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-876">VM</span></span>

* <span data-ttu-id="1368a-877">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="1368a-877">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="1368a-878">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-878">October 9, 2017</span></span>

<span data-ttu-id="1368a-879">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="1368a-879">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="1368a-880">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-880">Core</span></span>

* <span data-ttu-id="1368a-881">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="1368a-881">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-882">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-882">Appservice</span></span>

* <span data-ttu-id="1368a-883">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-883">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="1368a-884">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="1368a-884">Batch</span></span>

* <span data-ttu-id="1368a-885">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="1368a-885">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="1368a-886">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="1368a-886">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="1368a-887">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="1368a-887">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="1368a-888">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="1368a-888">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="1368a-889">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="1368a-889">Batchai</span></span>

* <span data-ttu-id="1368a-890">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="1368a-890">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="1368a-891">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="1368a-891">Keyvault</span></span>

* <span data-ttu-id="1368a-892">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1368a-892">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="1368a-893">(#4448)</span><span class="sxs-lookup"><span data-stu-id="1368a-893">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="1368a-894">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-894">Network</span></span>

* <span data-ttu-id="1368a-895">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="1368a-895">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="1368a-896">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="1368a-896">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-897">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-897">Resource</span></span>

* <span data-ttu-id="1368a-898">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="1368a-898">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="1368a-899">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="1368a-899">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="1368a-900">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="1368a-900">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="1368a-901">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="1368a-901">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-902">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-902">Sql</span></span>

* <span data-ttu-id="1368a-903">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="1368a-903">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="1368a-904">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="1368a-904">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="1368a-905">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="1368a-905">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-906">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-906">Storage</span></span>

* <span data-ttu-id="1368a-907">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1368a-907">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-908">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="1368a-908">Vm</span></span>

* <span data-ttu-id="1368a-909">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="1368a-909">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="1368a-910">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-910">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="1368a-911">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="1368a-911">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="1368a-912">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-912">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="1368a-913">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="1368a-913">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="1368a-914">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-914">September 22, 2017</span></span>

<span data-ttu-id="1368a-915">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="1368a-915">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-916">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-916">Resource</span></span>

* <span data-ttu-id="1368a-917">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="1368a-917">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="1368a-918">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="1368a-918">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="1368a-919">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="1368a-919">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="1368a-920">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="1368a-920">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="1368a-921">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-921">Network</span></span>

* <span data-ttu-id="1368a-922">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="1368a-922">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="1368a-923">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="1368a-923">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="1368a-924">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="1368a-924">Added `asg` application security group commands</span></span>
* <span data-ttu-id="1368a-925">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="1368a-925">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="1368a-926">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1368a-926">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="1368a-927">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1368a-927">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="1368a-928">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-928">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-929">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-929">Storage</span></span>

* <span data-ttu-id="1368a-930">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="1368a-930">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="1368a-931">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="1368a-931">Eventgrid</span></span>

* <span data-ttu-id="1368a-932">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="1368a-932">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-933">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-933">SQL</span></span>

* <span data-ttu-id="1368a-934">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="1368a-934">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="1368a-935">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="1368a-935">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="1368a-936">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="1368a-936">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="1368a-937">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="1368a-937">Keyvault</span></span>

* <span data-ttu-id="1368a-938">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="1368a-938">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-939">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-939">VM</span></span>

* <span data-ttu-id="1368a-940">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="1368a-940">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="1368a-941">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="1368a-941">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="1368a-942">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="1368a-942">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="1368a-943">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="1368a-943">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="1368a-944">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="1368a-944">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="1368a-945">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="1368a-945">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-946">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-946">ACS</span></span>

* <span data-ttu-id="1368a-947">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="1368a-947">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-948">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-948">Appservice</span></span>

* <span data-ttu-id="1368a-949">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="1368a-949">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="1368a-950">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="1368a-950">Backup</span></span>

* <span data-ttu-id="1368a-951">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="1368a-951">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="1368a-952">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-952">September 11, 2017</span></span>

<span data-ttu-id="1368a-953">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="1368a-953">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="1368a-954">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-954">Core</span></span>

* <span data-ttu-id="1368a-955">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="1368a-955">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="1368a-956">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="1368a-956">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-957">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-957">Acs</span></span>

* <span data-ttu-id="1368a-958">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="1368a-958">Added `acs list-locations` command</span></span>
* <span data-ttu-id="1368a-959">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1368a-959">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-960">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-960">Appservice</span></span>

* <span data-ttu-id="1368a-961">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="1368a-961">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="1368a-962">CDN</span><span class="sxs-lookup"><span data-stu-id="1368a-962">CDN</span></span>

* <span data-ttu-id="1368a-963">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-963">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="1368a-964">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="1368a-964">Extension</span></span>

* <span data-ttu-id="1368a-965">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="1368a-965">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="1368a-966">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="1368a-966">Keyvault</span></span>

* <span data-ttu-id="1368a-967">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="1368a-967">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="1368a-968">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-968">Network</span></span>

* <span data-ttu-id="1368a-969">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="1368a-969">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="1368a-970">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-970">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="1368a-971">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-971">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="1368a-972">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-972">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="1368a-973">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-973">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-974">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-974">Resource</span></span>

* <span data-ttu-id="1368a-975">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-975">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="1368a-976">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-976">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="1368a-977">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="1368a-977">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="1368a-978">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="1368a-978">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-979">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-979">SQL</span></span>

* <span data-ttu-id="1368a-980">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="1368a-980">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-981">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-981">VM</span></span>

* <span data-ttu-id="1368a-982">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="1368a-982">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="1368a-983">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="1368a-983">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="1368a-984">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-984">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="1368a-985">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="1368a-985">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="1368a-986">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="1368a-986">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="1368a-987">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-987">August 31, 2017</span></span>

<span data-ttu-id="1368a-988">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="1368a-988">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="1368a-989">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="1368a-989">Keyvault</span></span>

* <span data-ttu-id="1368a-990">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="1368a-990">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="1368a-991">Sf</span><span class="sxs-lookup"><span data-stu-id="1368a-991">Sf</span></span>

* <span data-ttu-id="1368a-992">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="1368a-992">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-993">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-993">Storage</span></span>

* <span data-ttu-id="1368a-994">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="1368a-994">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="1368a-995">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="1368a-995">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="1368a-996">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-996">August 28, 2017</span></span>

<span data-ttu-id="1368a-997">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="1368a-997">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="1368a-998">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="1368a-998">CLI</span></span>

* <span data-ttu-id="1368a-999">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="1368a-999">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-1000">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-1000">ACS</span></span>

* <span data-ttu-id="1368a-1001">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="1368a-1001">Corrected preview regions</span></span>
* <span data-ttu-id="1368a-1002">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1002">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="1368a-1003">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="1368a-1003">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-1004">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-1004">Appservice</span></span>

* <span data-ttu-id="1368a-1005">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1005">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="1368a-1006">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1006">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="1368a-1007">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1007">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="1368a-1008">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="1368a-1008">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="1368a-1009">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="1368a-1009">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="1368a-1010">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="1368a-1010">IoT</span></span>

* <span data-ttu-id="1368a-1011">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="1368a-1011">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="1368a-1012">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-1012">Network</span></span>

* <span data-ttu-id="1368a-1013">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1013">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="1368a-1014">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1014">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="1368a-1015">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1015">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="1368a-1016">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1016">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="1368a-1017">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1017">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="1368a-1018">Профиль</span><span class="sxs-lookup"><span data-stu-id="1368a-1018">Profile</span></span>

* <span data-ttu-id="1368a-1019">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="1368a-1019">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1368a-1020">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1368a-1020">Service Fabric</span></span>

* <span data-ttu-id="1368a-1021">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="1368a-1021">Preview release</span></span>
* <span data-ttu-id="1368a-1022">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="1368a-1022">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="1368a-1023">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="1368a-1023">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="1368a-1024">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1024">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-1025">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-1025">Storage</span></span>

* <span data-ttu-id="1368a-1026">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="1368a-1026">Enabled setting blob tier</span></span>
* <span data-ttu-id="1368a-1027">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="1368a-1027">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="1368a-1028">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1028">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="1368a-1029">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="1368a-1029">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="1368a-1030">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1030">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="1368a-1031">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1031">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-1032">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-1032">VM</span></span>

* <span data-ttu-id="1368a-1033">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1033">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="1368a-1034">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1034">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="1368a-1035">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="1368a-1035">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="1368a-1036">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="1368a-1036">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="1368a-1037">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="1368a-1037">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="1368a-1038">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1038">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="1368a-1039">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-1039">August 15, 2017</span></span>

<span data-ttu-id="1368a-1040">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="1368a-1040">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-1041">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-1041">ACS</span></span>

* <span data-ttu-id="1368a-1042">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="1368a-1042">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-1043">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-1043">Appservice</span></span>

* <span data-ttu-id="1368a-1044">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="1368a-1044">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="1368a-1045">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="1368a-1045">Event Grid</span></span>

* <span data-ttu-id="1368a-1046">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="1368a-1046">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="1368a-1047">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-1047">August 11, 2017</span></span>

<span data-ttu-id="1368a-1048">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="1368a-1048">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-1049">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-1049">ACS</span></span>

* <span data-ttu-id="1368a-1050">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="1368a-1050">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="1368a-1051">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="1368a-1051">Batch</span></span>

* <span data-ttu-id="1368a-1052">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="1368a-1052">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="1368a-1053">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="1368a-1053">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="1368a-1054">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1368a-1054">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="1368a-1055">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="1368a-1055">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="1368a-1056">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="1368a-1056">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="1368a-1057">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="1368a-1057">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="1368a-1058">Компонент</span><span class="sxs-lookup"><span data-stu-id="1368a-1058">Component</span></span>

* <span data-ttu-id="1368a-1059">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="1368a-1059">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="1368a-1060">Контейнер</span><span class="sxs-lookup"><span data-stu-id="1368a-1060">Container</span></span>

* <span data-ttu-id="1368a-1061">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="1368a-1061">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="1368a-1062">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1368a-1062">Data Lake Store</span></span>

* <span data-ttu-id="1368a-1063">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="1368a-1063">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="1368a-1064">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="1368a-1064">Event Grid</span></span>

* <span data-ttu-id="1368a-1065">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="1368a-1065">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="1368a-1066">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-1066">Network</span></span>

* <span data-ttu-id="1368a-1067">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="1368a-1067">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="1368a-1068">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1068">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="1368a-1069">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1069">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="1368a-1070">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1070">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="1368a-1071">Профиль</span><span class="sxs-lookup"><span data-stu-id="1368a-1071">Profile</span></span>

* <span data-ttu-id="1368a-1072">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="1368a-1072">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-1073">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-1073">Storage</span></span>

* <span data-ttu-id="1368a-1074">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="1368a-1074">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-1075">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-1075">VM</span></span>

* <span data-ttu-id="1368a-1076">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="1368a-1076">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="1368a-1077">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1077">Exposed `list-skus` command</span></span>
* <span data-ttu-id="1368a-1078">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="1368a-1078">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="1368a-1079">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="1368a-1079">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="1368a-1080">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="1368a-1080">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="1368a-1081">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-1081">July 28, 2017</span></span>

<span data-ttu-id="1368a-1082">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="1368a-1082">Version 2.0.12</span></span>

* <span data-ttu-id="1368a-1083">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="1368a-1083">Added container commands</span></span>
* <span data-ttu-id="1368a-1084">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="1368a-1084">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="1368a-1085">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-1085">Core</span></span>

* <span data-ttu-id="1368a-1086">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="1368a-1086">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="1368a-1087">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="1368a-1087">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="1368a-1088">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="1368a-1088">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="1368a-1089">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="1368a-1089">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="1368a-1090">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="1368a-1090">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="1368a-1091">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="1368a-1091">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="1368a-1092">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="1368a-1092">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1368a-1093">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="1368a-1093">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="1368a-1094">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="1368a-1094">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="1368a-1095">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="1368a-1095">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="1368a-1096">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="1368a-1096">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="1368a-1097">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="1368a-1097">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="1368a-1098">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="1368a-1098">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="1368a-1099">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="1368a-1099">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="1368a-1100">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="1368a-1100">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="1368a-1101">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="1368a-1101">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="1368a-1102">ACR</span><span class="sxs-lookup"><span data-stu-id="1368a-1102">ACR</span></span>

* <span data-ttu-id="1368a-1103">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="1368a-1103">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="1368a-1104">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="1368a-1104">Support SKU update for managed registries</span></span>
* <span data-ttu-id="1368a-1105">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="1368a-1105">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="1368a-1106">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="1368a-1106">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="1368a-1107">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="1368a-1107">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="1368a-1108">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="1368a-1108">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-1109">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-1109">ACS</span></span>

* <span data-ttu-id="1368a-1110">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="1368a-1110">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-1111">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="1368a-1111">Appservice</span></span>

* <span data-ttu-id="1368a-1112">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="1368a-1112">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="1368a-1113">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="1368a-1113">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="1368a-1114">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1114">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="1368a-1115">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="1368a-1115">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="1368a-1116">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="1368a-1116">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="1368a-1117">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="1368a-1117">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="1368a-1118">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="1368a-1118">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="1368a-1119">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="1368a-1119">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="1368a-1120">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="1368a-1120">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="1368a-1121">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1121">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="1368a-1122">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="1368a-1122">Batch</span></span>

* <span data-ttu-id="1368a-1123">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="1368a-1123">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="1368a-1124">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1124">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="1368a-1125">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1125">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="1368a-1126">CDN</span><span class="sxs-lookup"><span data-stu-id="1368a-1126">CDN</span></span>

* <span data-ttu-id="1368a-1127">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="1368a-1127">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="1368a-1128">Облако</span><span class="sxs-lookup"><span data-stu-id="1368a-1128">Cloud</span></span>

* <span data-ttu-id="1368a-1129">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="1368a-1129">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="1368a-1130">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="1368a-1130">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="1368a-1131">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="1368a-1131">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="1368a-1132">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="1368a-1132">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="1368a-1133">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1133">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1368a-1134">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1368a-1134">CosmosDB</span></span>

* <span data-ttu-id="1368a-1135">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="1368a-1135">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="1368a-1136">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="1368a-1136">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1368a-1137">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1368a-1137">Data Lake Analytics</span></span>

* <span data-ttu-id="1368a-1138">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1138">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="1368a-1139">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1139">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="1368a-1140">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1140">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1368a-1141">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1368a-1141">Data Lake Store</span></span>

* <span data-ttu-id="1368a-1142">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1142">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="1368a-1143">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="1368a-1143">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="1368a-1144">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1144">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="1368a-1145">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="1368a-1145">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="1368a-1146">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="1368a-1146">Interactive</span></span>

* <span data-ttu-id="1368a-1147">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="1368a-1147">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="1368a-1148">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="1368a-1148">Increased test coverage</span></span>
* <span data-ttu-id="1368a-1149">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="1368a-1149">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="1368a-1150">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="1368a-1150">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="1368a-1151">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="1368a-1151">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="1368a-1152">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="1368a-1152">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="1368a-1153">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="1368a-1153">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="1368a-1154">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1154">Added `--progress` flag</span></span>
* <span data-ttu-id="1368a-1155">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1155">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="1368a-1156">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="1368a-1156">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="1368a-1157">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="1368a-1157">IoT</span></span>

* <span data-ttu-id="1368a-1158">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="1368a-1158">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="1368a-1159">(3934).</span><span class="sxs-lookup"><span data-stu-id="1368a-1159">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="1368a-1160">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="1368a-1160">Key vault</span></span>

* <span data-ttu-id="1368a-1161">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="1368a-1161">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="1368a-1162">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1162">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="1368a-1163">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="1368a-1163">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="1368a-1164">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="1368a-1164">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="1368a-1165">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1165">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="1368a-1166">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="1368a-1166">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="1368a-1167">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="1368a-1167">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="1368a-1168">(3307).</span><span class="sxs-lookup"><span data-stu-id="1368a-1168">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="1368a-1169">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="1368a-1169">Lab</span></span>

* <span data-ttu-id="1368a-1170">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1170">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="1368a-1171">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1171">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="1368a-1172">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="1368a-1172">Monitor</span></span>

* <span data-ttu-id="1368a-1173">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="1368a-1173">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="1368a-1174">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1174">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="1368a-1175">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1175">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="1368a-1176">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1176">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="1368a-1177">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1177">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="1368a-1178">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="1368a-1178">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="1368a-1179">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="1368a-1179">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="1368a-1180">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="1368a-1180">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="1368a-1181">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="1368a-1181">`location` no longer required</span></span>
  * <span data-ttu-id="1368a-1182">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="1368a-1182">Add name and ID support for target</span></span>
  * <span data-ttu-id="1368a-1183">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="1368a-1183">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="1368a-1184">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="1368a-1184">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="1368a-1185">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="1368a-1185">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="1368a-1186">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="1368a-1186">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="1368a-1187">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1187">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="1368a-1188">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1188">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="1368a-1189">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-1189">Network</span></span>

* <span data-ttu-id="1368a-1190">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1190">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="1368a-1191">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1191">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="1368a-1192">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="1368a-1192">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="1368a-1193">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1193">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="1368a-1194">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1194">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="1368a-1195">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1195">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="1368a-1196">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1196">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="1368a-1197">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1197">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="1368a-1198">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1198">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="1368a-1199">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1199">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="1368a-1200">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1200">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="1368a-1201">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1201">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="1368a-1202">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1202">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="1368a-1203">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1203">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="1368a-1204">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1204">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="1368a-1205">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1205">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="1368a-1206">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="1368a-1206">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="1368a-1207">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1207">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="1368a-1208">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1208">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="1368a-1209">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1209">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="1368a-1210">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1210">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="1368a-1211">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1211">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="1368a-1212">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1212">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="1368a-1213">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="1368a-1213">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="1368a-1214">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="1368a-1214">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="1368a-1215">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="1368a-1215">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="1368a-1216">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="1368a-1216">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="1368a-1217">Профиль</span><span class="sxs-lookup"><span data-stu-id="1368a-1217">Profile</span></span>

* <span data-ttu-id="1368a-1218">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="1368a-1218">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="1368a-1219">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="1368a-1219">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="1368a-1220">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="1368a-1220">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="1368a-1221">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="1368a-1221">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="1368a-1222">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="1368a-1222">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="1368a-1223">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="1368a-1223">RDBMS</span></span>

* <span data-ttu-id="1368a-1224">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="1368a-1224">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="1368a-1225">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="1368a-1225">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="1368a-1226">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="1368a-1226">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="1368a-1227">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="1368a-1227">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-1228">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-1228">Resource</span></span>

* <span data-ttu-id="1368a-1229">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1229">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="1368a-1230">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1230">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="1368a-1231">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1231">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="1368a-1232">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1232">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="1368a-1233">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="1368a-1233">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="1368a-1234">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1234">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="1368a-1235">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="1368a-1235">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="1368a-1236">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1236">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="1368a-1237">Роль</span><span class="sxs-lookup"><span data-stu-id="1368a-1237">Role</span></span>

* <span data-ttu-id="1368a-1238">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="1368a-1238">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="1368a-1239">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="1368a-1239">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="1368a-1240">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="1368a-1240">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="1368a-1241">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="1368a-1241">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="1368a-1242">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1242">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="1368a-1243">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="1368a-1243">Service Fabric</span></span>
* <span data-ttu-id="1368a-1244">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="1368a-1244">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="1368a-1245">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="1368a-1245">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="1368a-1246">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="1368a-1246">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-1247">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-1247">SQL</span></span>

* <span data-ttu-id="1368a-1248">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1248">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="1368a-1249">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1249">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="1368a-1250">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1250">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-1251">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-1251">Storage</span></span>

* <span data-ttu-id="1368a-1252">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="1368a-1252">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="1368a-1253">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="1368a-1253">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="1368a-1254">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="1368a-1254">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="1368a-1255">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="1368a-1255">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="1368a-1256">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="1368a-1256">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="1368a-1257">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="1368a-1257">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-1258">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-1258">VM</span></span>

* <span data-ttu-id="1368a-1259">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="1368a-1259">Support configuring nsg</span></span>
* <span data-ttu-id="1368a-1260">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="1368a-1260">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="1368a-1261">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="1368a-1261">Support managed service identities</span></span>
* <span data-ttu-id="1368a-1262">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1262">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="1368a-1263">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="1368a-1263">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="1368a-1264">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-1264">May 10, 2017</span></span>

<span data-ttu-id="1368a-1265">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="1368a-1265">Version 2.0.6</span></span>

* <span data-ttu-id="1368a-1266">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="1368a-1266">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="1368a-1267">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="1368a-1267">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="1368a-1268">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="1368a-1268">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="1368a-1269">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="1368a-1269">Include Cognitive Services module</span></span>
* <span data-ttu-id="1368a-1270">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="1368a-1270">Include Service Fabric module</span></span>
* <span data-ttu-id="1368a-1271">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="1368a-1271">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="1368a-1272">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="1368a-1272">Add support for CDN commands</span></span>
* <span data-ttu-id="1368a-1273">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="1368a-1273">Remove Container module</span></span>
* <span data-ttu-id="1368a-1274">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1274">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="1368a-1275">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1275">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="1368a-1276">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-1276">Core</span></span>

* <span data-ttu-id="1368a-1277">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="1368a-1277">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="1368a-1278">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1278">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="1368a-1279">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1279">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="1368a-1280">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1280">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="1368a-1281">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1281">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="1368a-1282">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1282">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="1368a-1283">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1283">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="1368a-1284">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1284">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="1368a-1285">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1285">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="1368a-1286">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="1368a-1286">core: Improved performance</span></span>
* <span data-ttu-id="1368a-1287">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="1368a-1287">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="1368a-1288">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="1368a-1288">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-1289">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-1289">ACS</span></span>

* <span data-ttu-id="1368a-1290">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="1368a-1290">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="1368a-1291">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="1368a-1291">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="1368a-1292">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="1368a-1292">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="1368a-1293">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1293">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-1294">AppService</span><span class="sxs-lookup"><span data-stu-id="1368a-1294">AppService</span></span>

* <span data-ttu-id="1368a-1295">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="1368a-1295">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="1368a-1296">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="1368a-1296">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="1368a-1297">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="1368a-1297">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="1368a-1298">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="1368a-1298">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="1368a-1299">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="1368a-1299">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="1368a-1300">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1300">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="1368a-1301">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="1368a-1301">support slot swap with preview</span></span>
* <span data-ttu-id="1368a-1302">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1302">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="1368a-1303">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1303">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="1368a-1304">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="1368a-1304">CosmosDB</span></span>

* <span data-ttu-id="1368a-1305">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="1368a-1305">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="1368a-1306">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="1368a-1306">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="1368a-1307">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="1368a-1307">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="1368a-1308">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="1368a-1308">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="1368a-1309">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="1368a-1309">Data Lake Analytics</span></span>

* <span data-ttu-id="1368a-1310">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="1368a-1310">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="1368a-1311">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="1368a-1311">Add support for new catalog item type: package.</span></span> <span data-ttu-id="1368a-1312">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1312">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="1368a-1313">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="1368a-1313">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="1368a-1314">Таблица</span><span class="sxs-lookup"><span data-stu-id="1368a-1314">Table</span></span>
  * <span data-ttu-id="1368a-1315">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="1368a-1315">Table valued function</span></span>
  * <span data-ttu-id="1368a-1316">Просмотр</span><span class="sxs-lookup"><span data-stu-id="1368a-1316">View</span></span>
  * <span data-ttu-id="1368a-1317">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="1368a-1317">Table Statistics.</span></span> <span data-ttu-id="1368a-1318">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="1368a-1318">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="1368a-1319">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="1368a-1319">Data Lake Store</span></span>

* <span data-ttu-id="1368a-1320">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="1368a-1320">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="1368a-1321">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1321">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="1368a-1322">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="1368a-1322">missed help for access show.</span></span> <span data-ttu-id="1368a-1323">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="1368a-1323">adding it.</span></span> <span data-ttu-id="1368a-1324">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="1368a-1324">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="1368a-1325">Поиск</span><span class="sxs-lookup"><span data-stu-id="1368a-1325">Find</span></span>

* <span data-ttu-id="1368a-1326">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="1368a-1326">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="1368a-1327">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="1368a-1327">KeyVault</span></span>

* <span data-ttu-id="1368a-1328">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="1368a-1328">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="1368a-1329">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="1368a-1329">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="1368a-1330">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="1368a-1330">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="1368a-1331">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="1368a-1331">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="1368a-1332">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1332">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="1368a-1333">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="1368a-1333">Lab</span></span>

* <span data-ttu-id="1368a-1334">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="1368a-1334">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="1368a-1335">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="1368a-1335">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="1368a-1336">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="1368a-1336">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="1368a-1337">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="1368a-1337">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="1368a-1338">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="1368a-1338">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="1368a-1339">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="1368a-1339">Monitor</span></span>

* <span data-ttu-id="1368a-1340">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1340">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="1368a-1341">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1341">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="1368a-1342">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-1342">Network</span></span>

* <span data-ttu-id="1368a-1343">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1343">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="1368a-1344">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1344">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="1368a-1345">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="1368a-1345">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="1368a-1346">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="1368a-1346">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="1368a-1347">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="1368a-1347">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="1368a-1348">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="1368a-1348">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="1368a-1349">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="1368a-1349">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="1368a-1350">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="1368a-1350">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="1368a-1351">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1351">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="1368a-1352">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="1368a-1352">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="1368a-1353">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1353">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="1368a-1354">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1354">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="1368a-1355">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="1368a-1355">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="1368a-1356">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="1368a-1356">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="1368a-1357">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="1368a-1357">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="1368a-1358">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="1368a-1358">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="1368a-1359">Профиль</span><span class="sxs-lookup"><span data-stu-id="1368a-1359">Profile</span></span>

* <span data-ttu-id="1368a-1360">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1360">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="1368a-1361">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1361">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="1368a-1362">Redis</span><span class="sxs-lookup"><span data-stu-id="1368a-1362">Redis</span></span>

* <span data-ttu-id="1368a-1363">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="1368a-1363">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="1368a-1364">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="1368a-1364">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="1368a-1365">Ресурс</span><span class="sxs-lookup"><span data-stu-id="1368a-1365">Resource</span></span>

* <span data-ttu-id="1368a-1366">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1366">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="1368a-1367">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1367">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="1368a-1368">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1368">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="1368a-1369">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="1368a-1369">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="1368a-1370">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="1368a-1370">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="1368a-1371">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="1368a-1371">Add docs for az lock update.</span></span> <span data-ttu-id="1368a-1372">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="1368a-1372">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="1368a-1373">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="1368a-1373">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="1368a-1374">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="1368a-1374">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="1368a-1375">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="1368a-1375">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="1368a-1376">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="1368a-1376">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="1368a-1377">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1377">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="1368a-1378">Роль</span><span class="sxs-lookup"><span data-stu-id="1368a-1378">Role</span></span>

* <span data-ttu-id="1368a-1379">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1379">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="1368a-1380">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1380">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="1368a-1381">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1381">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="1368a-1382">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="1368a-1382">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="1368a-1383">SQL</span><span class="sxs-lookup"><span data-stu-id="1368a-1383">SQL</span></span>

* <span data-ttu-id="1368a-1384">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="1368a-1384">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="1368a-1385">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1385">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="1368a-1386">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-1386">Storage</span></span>

* <span data-ttu-id="1368a-1387">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1387">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="1368a-1388">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="1368a-1388">Add support for incremental blob copy</span></span>
* <span data-ttu-id="1368a-1389">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="1368a-1389">Add support for large block blob upload</span></span>
* <span data-ttu-id="1368a-1390">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="1368a-1390">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-1391">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-1391">VM</span></span>

* <span data-ttu-id="1368a-1392">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="1368a-1392">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="1368a-1393">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="1368a-1393">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="1368a-1394">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="1368a-1394">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="1368a-1395">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="1368a-1395">az vm/vmss disk</span></span>
  3. <span data-ttu-id="1368a-1396">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="1368a-1396">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="1368a-1397">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="1368a-1397">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="1368a-1398">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1398">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="1368a-1399">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-1399">April 3, 2017</span></span>

<span data-ttu-id="1368a-1400">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="1368a-1400">Version 2.0.2</span></span>

<span data-ttu-id="1368a-1401">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="1368a-1401">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="1368a-1402">Core</span><span class="sxs-lookup"><span data-stu-id="1368a-1402">Core</span></span>

* <span data-ttu-id="1368a-1403">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1368a-1403">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="1368a-1404">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1404">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="1368a-1405">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1405">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="1368a-1406">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1406">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1368a-1407">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1407">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="1368a-1408">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="1368a-1408">Add prompting for missing template parameters.</span></span> <span data-ttu-id="1368a-1409">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1409">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="1368a-1410">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1368a-1410">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="1368a-1411">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="1368a-1411">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="1368a-1412">ACS</span><span class="sxs-lookup"><span data-stu-id="1368a-1412">ACS</span></span>

* <span data-ttu-id="1368a-1413">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1413">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="1368a-1414">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="1368a-1414">Add support for ssh key password prompting.</span></span> <span data-ttu-id="1368a-1415">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1415">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="1368a-1416">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="1368a-1416">Add support for windows clusters.</span></span> <span data-ttu-id="1368a-1417">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1417">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="1368a-1418">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="1368a-1418">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="1368a-1419">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1419">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="1368a-1420">AppService</span><span class="sxs-lookup"><span data-stu-id="1368a-1420">AppService</span></span>

* <span data-ttu-id="1368a-1421">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1421">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="1368a-1422">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1422">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="1368a-1423">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1423">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="1368a-1424">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1424">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="1368a-1425">Data Lake</span><span class="sxs-lookup"><span data-stu-id="1368a-1425">DataLake</span></span>

* <span data-ttu-id="1368a-1426">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="1368a-1426">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="1368a-1427">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="1368a-1427">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="1368a-1428">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="1368a-1428">DocuemntDB</span></span>

* <span data-ttu-id="1368a-1429">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1429">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="1368a-1430">ВМ</span><span class="sxs-lookup"><span data-stu-id="1368a-1430">VM</span></span>

* <span data-ttu-id="1368a-1431">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1431">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="1368a-1432">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1432">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="1368a-1433">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1433">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="1368a-1434">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1434">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="1368a-1435">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1435">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="1368a-1436">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1436">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="1368a-1437">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="1368a-1437">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="1368a-1438">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="1368a-1438">February 27, 2017</span></span>

<span data-ttu-id="1368a-1439">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="1368a-1439">Version 2.0.0</span></span>

<span data-ttu-id="1368a-1440">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="1368a-1440">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="1368a-1441">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="1368a-1441">Container Service (acs)</span></span>
- <span data-ttu-id="1368a-1442">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="1368a-1442">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="1368a-1443">Сеть</span><span class="sxs-lookup"><span data-stu-id="1368a-1443">Networking</span></span>
- <span data-ttu-id="1368a-1444">Служба хранилища</span><span class="sxs-lookup"><span data-stu-id="1368a-1444">Storage</span></span>

<span data-ttu-id="1368a-1445">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1445">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="1368a-1446">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="1368a-1446">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="1368a-1447">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="1368a-1447">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="1368a-1448">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="1368a-1448">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="1368a-1449">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="1368a-1449">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="1368a-1450">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="1368a-1450">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="1368a-1451">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="1368a-1451">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="1368a-1452">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="1368a-1452">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="1368a-1453">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="1368a-1453">Provide feedback from the command line with the `az feedback` command</span></span>

