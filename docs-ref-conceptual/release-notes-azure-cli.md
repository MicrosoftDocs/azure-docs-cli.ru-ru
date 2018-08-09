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
ms.openlocfilehash: 549317fb3ffffbe5f392e7a2bbc5cb4ed10b7e89
ms.sourcegitcommit: 772aad0d9696156d6e87fa00e255dfd0b6394d23
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/08/2018
ms.locfileid: "39718020"
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="95c8c-103">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="95c8c-103">Azure CLI 2.0 release notes</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="95c8c-104">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-104">July 31, 2018</span></span>

<span data-ttu-id="95c8c-105">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="95c8c-105">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-106">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-106">ACR</span></span>

* <span data-ttu-id="95c8c-107">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-107">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="95c8c-108">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-108">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-109">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-109">ACS</span></span>

* <span data-ttu-id="95c8c-110">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="95c8c-110">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="95c8c-111">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-111">Batch</span></span>

* <span data-ttu-id="95c8c-112">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="95c8c-112">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-113">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-113">Container</span></span>

* <span data-ttu-id="95c8c-114">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-114">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-115">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-115">Network</span></span>

* <span data-ttu-id="95c8c-116">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="95c8c-116">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="95c8c-117">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-117">Resource</span></span>

* <span data-ttu-id="95c8c-118">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-118">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="95c8c-119">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="95c8c-119">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="95c8c-120">Роль</span><span class="sxs-lookup"><span data-stu-id="95c8c-120">Role</span></span>

* <span data-ttu-id="95c8c-121">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="95c8c-121">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="95c8c-122">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="95c8c-122">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="95c8c-123">поиска</span><span class="sxs-lookup"><span data-stu-id="95c8c-123">Search</span></span>

* <span data-ttu-id="95c8c-124">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="95c8c-124">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="95c8c-125">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-125">Service Bus</span></span>

* <span data-ttu-id="95c8c-126">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="95c8c-126">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="95c8c-127">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="95c8c-127">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="95c8c-128">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="95c8c-128">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="95c8c-129">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-129">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-130">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-130">Storage</span></span>

* <span data-ttu-id="95c8c-131">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="95c8c-131">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="95c8c-132">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="95c8c-132">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-133">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-133">VM</span></span>

* <span data-ttu-id="95c8c-134">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="95c8c-134">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="95c8c-135">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-135">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="95c8c-136">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="95c8c-136">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="95c8c-137">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="95c8c-137">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="95c8c-138">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-138">July 18, 2018</span></span>

<span data-ttu-id="95c8c-139">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="95c8c-139">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-140">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-140">Core</span></span>

* <span data-ttu-id="95c8c-141">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="95c8c-141">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="95c8c-142">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="95c8c-142">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="95c8c-143">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="95c8c-143">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-144">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-144">ACR</span></span>

* <span data-ttu-id="95c8c-145">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="95c8c-145">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="95c8c-146">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-146">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="95c8c-147">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="95c8c-147">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="95c8c-148">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="95c8c-148">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-149">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-149">ACS</span></span>

* <span data-ttu-id="95c8c-150">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="95c8c-150">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-151">AppService</span><span class="sxs-lookup"><span data-stu-id="95c8c-151">AppService</span></span>

* <span data-ttu-id="95c8c-152">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="95c8c-152">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="95c8c-153">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-153">Batch</span></span>

* <span data-ttu-id="95c8c-154">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="95c8c-154">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="95c8c-155">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="95c8c-155">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="95c8c-156">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="95c8c-156">Batch AI</span></span>

* <span data-ttu-id="95c8c-157">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-157">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-158">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-158">Container</span></span>

* <span data-ttu-id="95c8c-159">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="95c8c-159">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="95c8c-160">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="95c8c-160">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-161">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-161">Network</span></span>

* <span data-ttu-id="95c8c-162">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-162">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="95c8c-163">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-163">Added `network nic wait`</span></span>
* <span data-ttu-id="95c8c-164">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="95c8c-164">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="95c8c-165">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="95c8c-165">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="95c8c-166">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-166">Resource</span></span>

* <span data-ttu-id="95c8c-167">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-167">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="95c8c-168">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-168">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="95c8c-169">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-169">Added `deployment wait` command</span></span>
* <span data-ttu-id="95c8c-170">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="95c8c-170">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-171">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-171">SQL</span></span>

* <span data-ttu-id="95c8c-172">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-172">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="95c8c-173">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-173">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="95c8c-174">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-174">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-175">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-175">Storage</span></span>

* <span data-ttu-id="95c8c-176">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-176">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-177">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-177">VM</span></span>

* <span data-ttu-id="95c8c-178">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95c8c-178">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="95c8c-179">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-179">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="95c8c-180">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-180">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="95c8c-181">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-181">July 3, 2018</span></span>

<span data-ttu-id="95c8c-182">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="95c8c-182">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="95c8c-183">AKS</span><span class="sxs-lookup"><span data-stu-id="95c8c-183">AKS</span></span>

* <span data-ttu-id="95c8c-184">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-184">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="95c8c-185">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-185">July 3, 2018</span></span>

<span data-ttu-id="95c8c-186">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="95c8c-186">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-187">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-187">Core</span></span>

* <span data-ttu-id="95c8c-188">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="95c8c-188">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-189">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-189">ACR</span></span>

* <span data-ttu-id="95c8c-190">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="95c8c-190">Added polling build status</span></span>
* <span data-ttu-id="95c8c-191">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="95c8c-191">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="95c8c-192">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-192">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-193">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-193">ACS</span></span>

* <span data-ttu-id="95c8c-194">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95c8c-194">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="95c8c-195">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95c8c-195">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="95c8c-196">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-196">Updated options for `aks browse` command.</span></span> <span data-ttu-id="95c8c-197">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-197">Added `--listen-port` support</span></span>
* <span data-ttu-id="95c8c-198">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-198">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="95c8c-199">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="95c8c-199">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="95c8c-200">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-200">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-201">AppService</span><span class="sxs-lookup"><span data-stu-id="95c8c-201">AppService</span></span>

* <span data-ttu-id="95c8c-202">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-202">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="95c8c-203">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="95c8c-203">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="95c8c-204">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="95c8c-204">Backup</span></span>

* <span data-ttu-id="95c8c-205">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="95c8c-205">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="95c8c-206">Batch AI</span><span class="sxs-lookup"><span data-stu-id="95c8c-206">BatchAI</span></span>

* <span data-ttu-id="95c8c-207">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-207">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="95c8c-208">Облако</span><span class="sxs-lookup"><span data-stu-id="95c8c-208">Cloud</span></span>

* <span data-ttu-id="95c8c-209">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-209">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-210">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-210">Container</span></span>

* <span data-ttu-id="95c8c-211">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="95c8c-211">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="95c8c-212">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-212">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="95c8c-213">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="95c8c-213">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="95c8c-214">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="95c8c-214">Extension</span></span>

* <span data-ttu-id="95c8c-215">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="95c8c-215">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-216">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-216">Network</span></span>

* <span data-ttu-id="95c8c-217">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-217">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="95c8c-218">Rdbms</span><span class="sxs-lookup"><span data-stu-id="95c8c-218">Rdbms</span></span>

* <span data-ttu-id="95c8c-219">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-219">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-220">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-220">Resource</span></span>

* <span data-ttu-id="95c8c-221">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-221">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-222">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-222">VM</span></span>

* <span data-ttu-id="95c8c-223">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="95c8c-223">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="95c8c-224">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-224">June 25, 2018</span></span>

<span data-ttu-id="95c8c-225">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="95c8c-225">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="95c8c-226">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="95c8c-226">CLI</span></span>

* <span data-ttu-id="95c8c-227">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-227">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="95c8c-228">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-228">June 19, 2018</span></span>

<span data-ttu-id="95c8c-229">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="95c8c-229">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-230">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-230">Core</span></span>

* <span data-ttu-id="95c8c-231">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="95c8c-231">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-232">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-232">ACR</span></span>

* <span data-ttu-id="95c8c-233">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-233">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="95c8c-234">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="95c8c-234">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-235">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-235">ACS</span></span>

* <span data-ttu-id="95c8c-236">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-236">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="95c8c-237">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-237">Added `--update` support</span></span>
* <span data-ttu-id="95c8c-238">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-238">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="95c8c-239">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-239">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="95c8c-240">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-240">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="95c8c-241">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-241">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="95c8c-242">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-242">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="95c8c-243">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-243">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-244">AppService</span><span class="sxs-lookup"><span data-stu-id="95c8c-244">AppService</span></span>

* <span data-ttu-id="95c8c-245">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="95c8c-245">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="95c8c-246">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-246">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="95c8c-247">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-247">Batch</span></span>

* <span data-ttu-id="95c8c-248">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-248">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="95c8c-249">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="95c8c-249">Batch AI</span></span>

* <span data-ttu-id="95c8c-250">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="95c8c-250">Added support for workspaces.</span></span> <span data-ttu-id="95c8c-251">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-251">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="95c8c-252">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-252">Added support for experiments.</span></span> <span data-ttu-id="95c8c-253">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="95c8c-253">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="95c8c-254">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="95c8c-254">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="95c8c-255">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-255">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="95c8c-256">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-256">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="95c8c-257">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-257">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="95c8c-258">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="95c8c-258">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="95c8c-259">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-259">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="95c8c-260">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-260">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="95c8c-261">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-261">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="95c8c-262">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-262">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="95c8c-263">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-263">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="95c8c-264">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-264">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="95c8c-265">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="95c8c-265">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="95c8c-266">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-266">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="95c8c-267">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="95c8c-267">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
 - <span data-ttu-id="95c8c-268">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="95c8c-268">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
 - <span data-ttu-id="95c8c-269">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="95c8c-269">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="95c8c-270">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="95c8c-270">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
 - <span data-ttu-id="95c8c-271">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="95c8c-271">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="95c8c-272">Карты</span><span class="sxs-lookup"><span data-stu-id="95c8c-272">Maps</span></span>

* <span data-ttu-id="95c8c-273">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-273">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-274">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-274">Network</span></span>

* <span data-ttu-id="95c8c-275">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="95c8c-275">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="95c8c-276">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="95c8c-276">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="95c8c-277">#6502</span><span class="sxs-lookup"><span data-stu-id="95c8c-277">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="95c8c-278">Резервирование</span><span class="sxs-lookup"><span data-stu-id="95c8c-278">Reservations</span></span>

* <span data-ttu-id="95c8c-279">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-279">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="95c8c-280">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-280">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="95c8c-281">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-281">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="95c8c-282">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-282">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="95c8c-283">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-283">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="95c8c-284">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-284">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="95c8c-285">Роль</span><span class="sxs-lookup"><span data-stu-id="95c8c-285">Role</span></span>

* <span data-ttu-id="95c8c-286">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="95c8c-286">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-287">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-287">SQL</span></span>

* <span data-ttu-id="95c8c-288">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-288">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-289">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-289">Storage</span></span>

* <span data-ttu-id="95c8c-290">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="95c8c-290">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-291">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-291">VM</span></span>

* <span data-ttu-id="95c8c-292">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-292">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="95c8c-293">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-293">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="95c8c-294">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="95c8c-294">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="95c8c-295">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-295">June 13, 2018</span></span>

<span data-ttu-id="95c8c-296">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="95c8c-296">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-297">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-297">Core</span></span>

* <span data-ttu-id="95c8c-298">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="95c8c-298">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="95c8c-299">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-299">June 13, 2018</span></span>

<span data-ttu-id="95c8c-300">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="95c8c-300">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="95c8c-301">AKS</span><span class="sxs-lookup"><span data-stu-id="95c8c-301">AKS</span></span>

* <span data-ttu-id="95c8c-302">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="95c8c-302">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="95c8c-303">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="95c8c-303">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="95c8c-304">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="95c8c-304">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="95c8c-305">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="95c8c-305">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="95c8c-306">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="95c8c-306">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-307">AppService</span><span class="sxs-lookup"><span data-stu-id="95c8c-307">AppService</span></span>

* <span data-ttu-id="95c8c-308">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="95c8c-308">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="95c8c-309">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-309">June 5, 2018</span></span>

<span data-ttu-id="95c8c-310">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="95c8c-310">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="95c8c-311">Interactive</span><span class="sxs-lookup"><span data-stu-id="95c8c-311">Interactive</span></span>

* <span data-ttu-id="95c8c-312">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="95c8c-312">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="95c8c-313">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-313">June 5, 2018</span></span>

<span data-ttu-id="95c8c-314">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="95c8c-314">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-315">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-315">Core</span></span>

* <span data-ttu-id="95c8c-316">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="95c8c-316">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="95c8c-317">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="95c8c-317">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-318">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-318">ACR</span></span>

* <span data-ttu-id="95c8c-319">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="95c8c-319">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="95c8c-320">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-320">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="95c8c-321">AKS</span><span class="sxs-lookup"><span data-stu-id="95c8c-321">AKS</span></span>

* <span data-ttu-id="95c8c-322">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="95c8c-322">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="95c8c-323">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-323">Batch</span></span>

* <span data-ttu-id="95c8c-324">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="95c8c-324">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="95c8c-325">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="95c8c-325">IOT</span></span>

* <span data-ttu-id="95c8c-326">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="95c8c-326">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-327">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-327">Network</span></span>

* <span data-ttu-id="95c8c-328">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-328">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="95c8c-329">Policy Insights</span><span class="sxs-lookup"><span data-stu-id="95c8c-329">Policy Insights</span></span>

* <span data-ttu-id="95c8c-330">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="95c8c-330">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="95c8c-331">ARM</span><span class="sxs-lookup"><span data-stu-id="95c8c-331">ARM</span></span>

* <span data-ttu-id="95c8c-332">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-332">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-333">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-333">SQL</span></span>

* <span data-ttu-id="95c8c-334">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="95c8c-334">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="95c8c-335">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="95c8c-335">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="95c8c-336">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-336">Storage</span></span>

* <span data-ttu-id="95c8c-337">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-337">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-338">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-338">VM</span></span>

* <span data-ttu-id="95c8c-339">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-339">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="95c8c-340">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-340">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="95c8c-341">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-341">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="95c8c-342">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-342">May 22, 2018</span></span>

<span data-ttu-id="95c8c-343">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="95c8c-343">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-344">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-344">Core</span></span>

* <span data-ttu-id="95c8c-345">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-345">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-346">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-346">ACS</span></span>

* <span data-ttu-id="95c8c-347">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-347">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="95c8c-348">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="95c8c-348">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-349">AppService</span><span class="sxs-lookup"><span data-stu-id="95c8c-349">AppService</span></span>

* <span data-ttu-id="95c8c-350">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="95c8c-350">Improved generic update commands</span></span>
* <span data-ttu-id="95c8c-351">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-351">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-352">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-352">Container</span></span>

* <span data-ttu-id="95c8c-353">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="95c8c-353">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="95c8c-354">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-354">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="95c8c-355">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="95c8c-355">Extension</span></span>

* <span data-ttu-id="95c8c-356">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-356">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="95c8c-357">Interactive</span><span class="sxs-lookup"><span data-stu-id="95c8c-357">Interactive</span></span>

* <span data-ttu-id="95c8c-358">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="95c8c-358">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="95c8c-359">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-359">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="95c8c-360">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="95c8c-360">KeyVault</span></span>

* <span data-ttu-id="95c8c-361">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="95c8c-361">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-362">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-362">Network</span></span>

* <span data-ttu-id="95c8c-363">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="95c8c-363">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="95c8c-364">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="95c8c-364">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-365">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-365">SQL</span></span>

* <span data-ttu-id="95c8c-366">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="95c8c-366">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="95c8c-367">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-367">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="95c8c-368">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-368">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="95c8c-369">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="95c8c-369">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="95c8c-370">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="95c8c-370">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="95c8c-371">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-371">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="95c8c-372">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-372">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="95c8c-373">`edition`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-373">`edition`.</span></span> <span data-ttu-id="95c8c-374">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-374">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="95c8c-375">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-375">`elasticPoolName`.</span></span> <span data-ttu-id="95c8c-376">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-376">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="95c8c-377">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="95c8c-377">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="95c8c-378">`edition`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-378">`edition`.</span></span> <span data-ttu-id="95c8c-379">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-379">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="95c8c-380">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-380">`dtu`.</span></span> <span data-ttu-id="95c8c-381">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-381">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="95c8c-382">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-382">`databaseDtuMin`.</span></span> <span data-ttu-id="95c8c-383">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-383">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="95c8c-384">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-384">`databaseDtuMax`.</span></span> <span data-ttu-id="95c8c-385">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-385">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="95c8c-386">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-386">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="95c8c-387">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-387">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-388">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-388">Storage</span></span>

* <span data-ttu-id="95c8c-389">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-389">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="95c8c-390">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-390">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-391">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-391">VM</span></span>

* <span data-ttu-id="95c8c-392">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-392">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="95c8c-393">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-393">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="95c8c-394">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-394">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="95c8c-395">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-395">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="95c8c-396">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-396">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="95c8c-397">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-397">May 7, 2018</span></span>

<span data-ttu-id="95c8c-398">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="95c8c-398">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-399">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-399">Core</span></span>

* <span data-ttu-id="95c8c-400">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="95c8c-400">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="95c8c-401">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-401">Added limited support for positional arguments</span></span>
* <span data-ttu-id="95c8c-402">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-402">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="95c8c-403">#5591</span><span class="sxs-lookup"><span data-stu-id="95c8c-403">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="95c8c-404">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-404">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="95c8c-405">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="95c8c-405">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="95c8c-406">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="95c8c-406">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="95c8c-407">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-407">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="95c8c-408">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-408">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-409">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-409">ACR</span></span>

* <span data-ttu-id="95c8c-410">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="95c8c-410">Added ACR Build commands</span></span>
* <span data-ttu-id="95c8c-411">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="95c8c-411">Improved resource not found error messages</span></span>
* <span data-ttu-id="95c8c-412">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="95c8c-412">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="95c8c-413">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="95c8c-413">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="95c8c-414">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="95c8c-414">Improved repository commands error messages</span></span>
* <span data-ttu-id="95c8c-415">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="95c8c-415">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-416">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-416">ACS</span></span>

* <span data-ttu-id="95c8c-417">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="95c8c-417">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="95c8c-418">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="95c8c-418">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="95c8c-419">AMS</span><span class="sxs-lookup"><span data-stu-id="95c8c-419">AMS</span></span>

* <span data-ttu-id="95c8c-420">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="95c8c-420">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-421">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-421">Appservice</span></span>

* <span data-ttu-id="95c8c-422">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="95c8c-422">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="95c8c-423">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-423">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="95c8c-424">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="95c8c-424">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="95c8c-425">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-425">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="95c8c-426">Искусственный интеллект пакетной службы</span><span class="sxs-lookup"><span data-stu-id="95c8c-426">Batch AI</span></span>

* <span data-ttu-id="95c8c-427">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="95c8c-427">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="95c8c-428">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="95c8c-428">Cognitive Services</span></span>

* <span data-ttu-id="95c8c-429">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="95c8c-429">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="95c8c-430">Потребление</span><span class="sxs-lookup"><span data-stu-id="95c8c-430">Consumption</span></span>

* <span data-ttu-id="95c8c-431">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="95c8c-431">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-432">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-432">Container</span></span>

* <span data-ttu-id="95c8c-433">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="95c8c-433">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="95c8c-434">База данных Cosmos</span><span class="sxs-lookup"><span data-stu-id="95c8c-434">Cosmos DB</span></span>

* <span data-ttu-id="95c8c-435">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="95c8c-435">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="95c8c-436">DMS</span><span class="sxs-lookup"><span data-stu-id="95c8c-436">DMS</span></span>

* <span data-ttu-id="95c8c-437">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="95c8c-437">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="95c8c-438">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="95c8c-438">Extension</span></span>

* <span data-ttu-id="95c8c-439">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="95c8c-439">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="95c8c-440">Interactive</span><span class="sxs-lookup"><span data-stu-id="95c8c-440">Interactive</span></span>

* <span data-ttu-id="95c8c-441">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="95c8c-441">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="95c8c-442">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="95c8c-442">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="95c8c-443">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-443">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="95c8c-444">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="95c8c-444">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="95c8c-445">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="95c8c-445">Lab</span></span>

* <span data-ttu-id="95c8c-446">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="95c8c-446">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-447">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-447">Network</span></span>

* <span data-ttu-id="95c8c-448">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="95c8c-448">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="95c8c-449">Профиль</span><span class="sxs-lookup"><span data-stu-id="95c8c-449">Profile</span></span>

* <span data-ttu-id="95c8c-450">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-450">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="95c8c-451">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="95c8c-451">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="95c8c-452">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-452">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="95c8c-453">Redis</span><span class="sxs-lookup"><span data-stu-id="95c8c-453">Redis</span></span>

* <span data-ttu-id="95c8c-454">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-454">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="95c8c-455">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="95c8c-455">Deprecated `redis list-all`.</span></span> <span data-ttu-id="95c8c-456">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-456">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="95c8c-457">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-457">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="95c8c-458">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="95c8c-458">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="95c8c-459">Роль</span><span class="sxs-lookup"><span data-stu-id="95c8c-459">Role</span></span>

* <span data-ttu-id="95c8c-460">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="95c8c-460">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-461">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-461">Storage</span></span>

* <span data-ttu-id="95c8c-462">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="95c8c-462">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="95c8c-463">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="95c8c-463">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="95c8c-464">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="95c8c-464">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="95c8c-465">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="95c8c-465">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="95c8c-466">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="95c8c-466">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-467">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-467">VM</span></span>

* <span data-ttu-id="95c8c-468">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="95c8c-468">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="95c8c-469">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="95c8c-469">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="95c8c-470">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]. Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="95c8c-470">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="95c8c-471">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-471">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="95c8c-472">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="95c8c-472">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="95c8c-473">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="95c8c-473">Added write accelerator support</span></span>
* <span data-ttu-id="95c8c-474">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-474">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="95c8c-475">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="95c8c-475">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="95c8c-476">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="95c8c-476">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="95c8c-477">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-477">April 10, 2018</span></span>

<span data-ttu-id="95c8c-478">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="95c8c-478">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-479">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-479">ACR</span></span>

* <span data-ttu-id="95c8c-480">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="95c8c-480">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-481">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-481">ACS</span></span>

* <span data-ttu-id="95c8c-482">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="95c8c-482">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-483">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-483">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="95c8c-485">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-485">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="95c8c-486">Batch AI</span><span class="sxs-lookup"><span data-stu-id="95c8c-486">BatchAI</span></span>

* <span data-ttu-id="95c8c-487">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="95c8c-487">Added support for 2018-03-01 API</span></span>

 - <span data-ttu-id="95c8c-488">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="95c8c-488">Job level mounting</span></span>
 - <span data-ttu-id="95c8c-489">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-489">Environment variables with secret values</span></span>
 - <span data-ttu-id="95c8c-490">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="95c8c-490">Performance counters settings</span></span>
 - <span data-ttu-id="95c8c-491">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="95c8c-491">Reporting of job specific path segment</span></span>
 - <span data-ttu-id="95c8c-492">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-492">Support for subfolders in list files api</span></span>
 - <span data-ttu-id="95c8c-493">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="95c8c-493">Usage and limits reporting</span></span>
 - <span data-ttu-id="95c8c-494">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-494">Allow to specify caching type for NFS servers</span></span>
 - <span data-ttu-id="95c8c-495">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-495">Support for custom images</span></span>
 - <span data-ttu-id="95c8c-496">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="95c8c-496">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="95c8c-497">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="95c8c-497">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="95c8c-498">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-498">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="95c8c-499">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="95c8c-499">National clouds are supported</span></span>
* <span data-ttu-id="95c8c-500">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="95c8c-500">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="95c8c-501">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="95c8c-501">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="95c8c-502">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="95c8c-502">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="95c8c-503">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="95c8c-503">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="95c8c-504">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="95c8c-504">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="95c8c-505">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="95c8c-505">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="95c8c-506">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-506">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="95c8c-507">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="95c8c-507">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="95c8c-508">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="95c8c-508">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="95c8c-509">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-509">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="95c8c-510">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="95c8c-510">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="95c8c-511">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-511">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="95c8c-512">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-512">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="95c8c-513">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="95c8c-513">Billing</span></span>

* <span data-ttu-id="95c8c-514">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="95c8c-514">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="95c8c-515">Потребление</span><span class="sxs-lookup"><span data-stu-id="95c8c-515">Consumption</span></span>

* <span data-ttu-id="95c8c-516">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-516">Added `marketplace` commands</span></span>
* <span data-ttu-id="95c8c-517">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-517">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="95c8c-518">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-518">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="95c8c-519">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-519">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="95c8c-520">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-520">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="95c8c-521">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-521">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-522">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-522">Container</span></span>

* <span data-ttu-id="95c8c-523">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-523">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="95c8c-524">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="95c8c-524">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="95c8c-525">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="95c8c-525">Extension</span></span>

* <span data-ttu-id="95c8c-526">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-526">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="95c8c-527">Interactive</span><span class="sxs-lookup"><span data-stu-id="95c8c-527">Interactive</span></span>

* <span data-ttu-id="95c8c-528">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="95c8c-528">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="95c8c-529">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="95c8c-529">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="95c8c-530">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-530">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-531">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-531">Network</span></span>

* <span data-ttu-id="95c8c-532">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-532">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="95c8c-533">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-533">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="95c8c-534">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="95c8c-534">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="95c8c-535">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="95c8c-535">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="95c8c-536">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="95c8c-536">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="95c8c-537">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-537">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="95c8c-538">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-538">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="95c8c-539">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="95c8c-539">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="95c8c-540">Профиль</span><span class="sxs-lookup"><span data-stu-id="95c8c-540">Profile</span></span>

* <span data-ttu-id="95c8c-541">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-541">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="95c8c-542">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-542">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="95c8c-543">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="95c8c-543">RDBMS</span></span>

* <span data-ttu-id="95c8c-544">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-544">Added `georestore` command</span></span>
* <span data-ttu-id="95c8c-545">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="95c8c-545">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-546">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-546">Resource</span></span>

* <span data-ttu-id="95c8c-547">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-547">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="95c8c-548">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-548">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-549">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-549">SQL</span></span>

* <span data-ttu-id="95c8c-550">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-550">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-551">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-551">Storage</span></span>

* <span data-ttu-id="95c8c-552">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="95c8c-552">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-553">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-553">VM</span></span>

* <span data-ttu-id="95c8c-554">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="95c8c-554">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="95c8c-555">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="95c8c-555">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="95c8c-557">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-557">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="95c8c-558">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="95c8c-558">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="95c8c-559">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="95c8c-559">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="95c8c-560">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="95c8c-560">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="95c8c-561">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-561">March 27, 2018</span></span>

<span data-ttu-id="95c8c-562">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="95c8c-562">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-563">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-563">Core</span></span>

* <span data-ttu-id="95c8c-564">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="95c8c-564">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-565">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-565">ACS</span></span>

* <span data-ttu-id="95c8c-566">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="95c8c-566">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-567">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-567">Appservice</span></span>

* <span data-ttu-id="95c8c-568">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-568">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="95c8c-569">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-569">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="95c8c-570">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="95c8c-570">Backup</span></span>

* <span data-ttu-id="95c8c-571">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-571">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="95c8c-572">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="95c8c-572">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="95c8c-573">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="95c8c-573">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="95c8c-574">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-574">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-575">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-575">Container</span></span>

* <span data-ttu-id="95c8c-576">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-576">Added `container exec` command.</span></span> <span data-ttu-id="95c8c-577">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-577">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="95c8c-578">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-578">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="95c8c-579">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="95c8c-579">Extension</span></span>

* <span data-ttu-id="95c8c-580">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="95c8c-580">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="95c8c-581">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-581">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="95c8c-582">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95c8c-582">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="95c8c-583">Interactive</span><span class="sxs-lookup"><span data-stu-id="95c8c-583">Interactive</span></span>

* <span data-ttu-id="95c8c-584">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="95c8c-584">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="95c8c-585">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-585">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="95c8c-586">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="95c8c-586">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="95c8c-587">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="95c8c-587">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="95c8c-588">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="95c8c-588">Lab</span></span>

* <span data-ttu-id="95c8c-589">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-589">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="95c8c-590">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="95c8c-590">Monitor</span></span>

* <span data-ttu-id="95c8c-591">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="95c8c-591">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="95c8c-592">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="95c8c-592">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="95c8c-593">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="95c8c-593">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-594">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-594">Network</span></span>

* <span data-ttu-id="95c8c-595">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="95c8c-595">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="95c8c-596">Профиль</span><span class="sxs-lookup"><span data-stu-id="95c8c-596">Profile</span></span>

* <span data-ttu-id="95c8c-597">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-597">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="95c8c-598">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="95c8c-598">RDBMS</span></span>

* <span data-ttu-id="95c8c-599">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="95c8c-599">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-600">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-600">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="95c8c-602">Роль</span><span class="sxs-lookup"><span data-stu-id="95c8c-602">Role</span></span>

* <span data-ttu-id="95c8c-603">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-603">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="95c8c-604">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="95c8c-604">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="95c8c-605">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="95c8c-605">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="95c8c-606">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-606">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="95c8c-607">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-607">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-608">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-608">Storage</span></span>

* <span data-ttu-id="95c8c-609">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="95c8c-609">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="95c8c-610">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049): проблемы, когда при отправке добавочного большого двоичного объекта игнорируются параметры условия.</span><span class="sxs-lookup"><span data-stu-id="95c8c-610">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-611">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-611">VM</span></span>

* <span data-ttu-id="95c8c-612">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-612">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="95c8c-613">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-613">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="95c8c-614">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="95c8c-614">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="95c8c-615">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="95c8c-615">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="95c8c-616">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-616">March 13, 2018</span></span>

<span data-ttu-id="95c8c-617">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="95c8c-617">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-618">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-618">ACR</span></span>

* <span data-ttu-id="95c8c-619">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-619">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="95c8c-620">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="95c8c-620">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="95c8c-621">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="95c8c-621">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-622">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-622">ACS</span></span>

* <span data-ttu-id="95c8c-623">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="95c8c-623">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="95c8c-624">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-624">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="95c8c-625">Помощник</span><span class="sxs-lookup"><span data-stu-id="95c8c-625">Advisor</span></span>

* <span data-ttu-id="95c8c-626">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-626">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="95c8c-627">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-627">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="95c8c-628">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-628">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="95c8c-629">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-629">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="95c8c-630">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-630">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-631">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-631">Appservice</span></span>

* <span data-ttu-id="95c8c-632">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="95c8c-632">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="95c8c-633">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-633">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="95c8c-634">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="95c8c-634">Eventhubs</span></span>

* <span data-ttu-id="95c8c-635">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="95c8c-635">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="95c8c-636">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="95c8c-636">Extension</span></span>

* <span data-ttu-id="95c8c-637">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="95c8c-637">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="95c8c-638">Interactive</span><span class="sxs-lookup"><span data-stu-id="95c8c-638">Interactive</span></span>

* <span data-ttu-id="95c8c-639">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625): теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="95c8c-639">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="95c8c-640">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016): при использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="95c8c-640">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="95c8c-641">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688): если при загрузке таблицы команд возникало исключение, опережающий ввод не выполнялся.</span><span class="sxs-lookup"><span data-stu-id="95c8c-641">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="95c8c-642">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="95c8c-642">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="95c8c-643">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="95c8c-643">Monitor</span></span>

* <span data-ttu-id="95c8c-644">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="95c8c-644">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="95c8c-645">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-645">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="95c8c-646">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-646">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="95c8c-647">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-647">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-648">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-648">Network</span></span>

* <span data-ttu-id="95c8c-649">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-649">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="95c8c-650">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="95c8c-650">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="95c8c-651">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-651">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="95c8c-652">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-652">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="95c8c-653">Профиль</span><span class="sxs-lookup"><span data-stu-id="95c8c-653">Profile</span></span>

* <span data-ttu-id="95c8c-654">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="95c8c-654">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="95c8c-655">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-655">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="95c8c-656">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="95c8c-656">RDBMS</span></span>

* <span data-ttu-id="95c8c-657">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="95c8c-657">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="95c8c-658">Служебная шина Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-658">Service Bus</span></span>

* <span data-ttu-id="95c8c-659">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="95c8c-659">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-660">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-660">Storage</span></span>

* <span data-ttu-id="95c8c-661">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="95c8c-661">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="95c8c-662">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286): при пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="95c8c-662">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-663">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-663">VM</span></span>

* <span data-ttu-id="95c8c-664">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="95c8c-664">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="95c8c-665">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="95c8c-665">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="95c8c-666">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-666">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="95c8c-667">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="95c8c-667">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="95c8c-668">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="95c8c-668">February 27, 2018</span></span>

<span data-ttu-id="95c8c-669">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="95c8c-669">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-670">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-670">Core</span></span>

* <span data-ttu-id="95c8c-671">Исправлена ошибка с установкой Homebrew [№ 5184](https://github.com/Azure/azure-cli/issues/5184).</span><span class="sxs-lookup"><span data-stu-id="95c8c-671">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="95c8c-672">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="95c8c-672">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="95c8c-673">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-673">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-674">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-674">ACS</span></span>

* <span data-ttu-id="95c8c-675">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95c8c-675">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="95c8c-676">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="95c8c-676">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="95c8c-677">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-677">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="95c8c-678">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-678">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-679">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-679">Appservice</span></span>

* <span data-ttu-id="95c8c-680">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="95c8c-680">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="95c8c-681">Исправлена ошибка с сообщением `Free` о недопустимом SKU [№ 5538](https://github.com/Azure/azure-cli/issues/5538)</span><span class="sxs-lookup"><span data-stu-id="95c8c-681">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="95c8c-682">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="95c8c-682">Cognitive Services</span></span>

* <span data-ttu-id="95c8c-683">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="95c8c-683">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="95c8c-684">Потребление</span><span class="sxs-lookup"><span data-stu-id="95c8c-684">Consumption</span></span>

* <span data-ttu-id="95c8c-685">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="95c8c-685">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="95c8c-686">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="95c8c-686">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-687">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-687">Container</span></span>

* <span data-ttu-id="95c8c-688">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="95c8c-688">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-689">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-689">Network</span></span>

* <span data-ttu-id="95c8c-690">Исправлена ошибка с отсутствующим клиентом в `network vnet-gateway vpn-client generate` [№ 5559](https://github.com/Azure/azure-cli/issues/5559).</span><span class="sxs-lookup"><span data-stu-id="95c8c-690">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-691">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-691">Resource</span></span>

* <span data-ttu-id="95c8c-692">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="95c8c-692">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="95c8c-693">Роль</span><span class="sxs-lookup"><span data-stu-id="95c8c-693">Role</span></span>

* <span data-ttu-id="95c8c-694">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="95c8c-694">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-695">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-695">SQL</span></span>

* <span data-ttu-id="95c8c-696">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-696">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-697">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-697">Storage</span></span>

* <span data-ttu-id="95c8c-698">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-698">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-699">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-699">VM</span></span>

* <span data-ttu-id="95c8c-700">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="95c8c-700">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="95c8c-701">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-701">February 13, 2018</span></span>

<span data-ttu-id="95c8c-702">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="95c8c-702">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-703">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-703">Core</span></span>

* <span data-ttu-id="95c8c-704">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="95c8c-704">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-705">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-705">ACS</span></span>

* <span data-ttu-id="95c8c-706">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="95c8c-706">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="95c8c-707">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-707">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="95c8c-708">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="95c8c-708">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="95c8c-709">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="95c8c-709">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="95c8c-710">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="95c8c-710">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="95c8c-711">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-711">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="95c8c-712">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="95c8c-712">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="95c8c-713">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-713">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-714">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-714">Appservice</span></span>

* <span data-ttu-id="95c8c-715">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-715">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="95c8c-716">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-716">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="95c8c-717">CDN</span><span class="sxs-lookup"><span data-stu-id="95c8c-717">CDN</span></span>

* <span data-ttu-id="95c8c-718">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-718">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-719">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-719">Container</span></span>

* <span data-ttu-id="95c8c-720">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="95c8c-720">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="95c8c-721">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-721">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="95c8c-722">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="95c8c-722">CosmosDB</span></span>

* <span data-ttu-id="95c8c-723">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-723">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="95c8c-724">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="95c8c-724">Extension</span></span>

* <span data-ttu-id="95c8c-725">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-725">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="95c8c-726">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-726">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="95c8c-727">Отзыв</span><span class="sxs-lookup"><span data-stu-id="95c8c-727">Feedback</span></span>

* <span data-ttu-id="95c8c-728">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="95c8c-728">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="95c8c-729">Interactive</span><span class="sxs-lookup"><span data-stu-id="95c8c-729">Interactive</span></span>

* <span data-ttu-id="95c8c-730">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="95c8c-730">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="95c8c-731">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-731">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="95c8c-732">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="95c8c-732">IoT</span></span>

* <span data-ttu-id="95c8c-733">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="95c8c-733">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="95c8c-734">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="95c8c-734">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="95c8c-735">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-735">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="95c8c-736">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="95c8c-736">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="95c8c-737">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="95c8c-737">Monitor</span></span>

* <span data-ttu-id="95c8c-738">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-738">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-739">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-739">Network</span></span>

* <span data-ttu-id="95c8c-740">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="95c8c-740">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="95c8c-741">Профиль</span><span class="sxs-lookup"><span data-stu-id="95c8c-741">Profile</span></span>

* <span data-ttu-id="95c8c-742">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="95c8c-742">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-743">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-743">Resource</span></span>

* <span data-ttu-id="95c8c-744">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-744">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="95c8c-745">Роль</span><span class="sxs-lookup"><span data-stu-id="95c8c-745">Role</span></span>

* <span data-ttu-id="95c8c-746">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="95c8c-746">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-747">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-747">SQL</span></span>

* <span data-ttu-id="95c8c-748">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-748">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="95c8c-749">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-749">Added `sql db rename`</span></span>
* <span data-ttu-id="95c8c-750">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="95c8c-750">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-751">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-751">Storage</span></span>

* <span data-ttu-id="95c8c-752">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="95c8c-752">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-753">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-753">VM</span></span>

* <span data-ttu-id="95c8c-754">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="95c8c-754">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="95c8c-755">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="95c8c-755">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="95c8c-756">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="95c8c-756">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="95c8c-757">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-757">January 31, 2018</span></span>

<span data-ttu-id="95c8c-758">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="95c8c-758">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-759">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-759">Core</span></span>

* <span data-ttu-id="95c8c-760">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="95c8c-760">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="95c8c-761">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="95c8c-761">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="95c8c-762">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="95c8c-762">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="95c8c-763">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="95c8c-763">Use `--verbose` to see</span></span>
* <span data-ttu-id="95c8c-764">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="95c8c-764">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-765">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-765">ACS</span></span>

* <span data-ttu-id="95c8c-766">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-766">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="95c8c-767">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-767">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-768">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-768">Appservice</span></span>

* <span data-ttu-id="95c8c-769">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="95c8c-769">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="95c8c-770">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="95c8c-770">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="95c8c-771">CDN</span><span class="sxs-lookup"><span data-stu-id="95c8c-771">CDN</span></span>

* <span data-ttu-id="95c8c-772">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-772">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="95c8c-773">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="95c8c-773">CosmosDB</span></span>

* <span data-ttu-id="95c8c-774">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="95c8c-774">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="95c8c-775">Interactive</span><span class="sxs-lookup"><span data-stu-id="95c8c-775">Interactive</span></span>

* <span data-ttu-id="95c8c-776">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="95c8c-776">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-777">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-777">Network</span></span>

* <span data-ttu-id="95c8c-778">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-778">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="95c8c-779">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95c8c-779">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="95c8c-780">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-780">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="95c8c-781">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-781">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="95c8c-782">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-782">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="95c8c-783">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="95c8c-783">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="95c8c-784">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="95c8c-784">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="95c8c-785">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="95c8c-785">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="95c8c-786">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-786">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="95c8c-787">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-787">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="95c8c-788">Профиль</span><span class="sxs-lookup"><span data-stu-id="95c8c-788">Profile</span></span>

* <span data-ttu-id="95c8c-789">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="95c8c-789">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-790">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-790">Resource</span></span>

* <span data-ttu-id="95c8c-791">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="95c8c-791">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-792">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-792">Storage</span></span>

* <span data-ttu-id="95c8c-793">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="95c8c-793">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="95c8c-794">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="95c8c-794">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="95c8c-795">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-795">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="95c8c-796">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-796">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="95c8c-797">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="95c8c-797">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-798">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-798">VM</span></span>

* <span data-ttu-id="95c8c-799">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="95c8c-799">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="95c8c-800">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-800">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="95c8c-801">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="95c8c-801">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="95c8c-802">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-802">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="95c8c-803">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-803">January 17, 2018</span></span>

<span data-ttu-id="95c8c-804">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="95c8c-804">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-805">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-805">ACR</span></span>

* <span data-ttu-id="95c8c-806">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="95c8c-806">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="95c8c-807">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="95c8c-807">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-808">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-808">ACS</span></span>

* <span data-ttu-id="95c8c-809">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-809">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="95c8c-810">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="95c8c-810">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-811">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-811">Appservice</span></span>

* <span data-ttu-id="95c8c-812">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="95c8c-812">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="95c8c-813">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-813">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="95c8c-814">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-814">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="95c8c-815">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="95c8c-815">Backup</span></span>

* <span data-ttu-id="95c8c-816">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="95c8c-816">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="95c8c-817">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="95c8c-817">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="95c8c-818">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="95c8c-818">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="95c8c-819">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="95c8c-819">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="95c8c-820">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="95c8c-820">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="95c8c-821">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-821">Batch</span></span>

* <span data-ttu-id="95c8c-822">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="95c8c-822">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="95c8c-823">Облако</span><span class="sxs-lookup"><span data-stu-id="95c8c-823">Cloud</span></span>

* <span data-ttu-id="95c8c-824">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-824">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="95c8c-825">Потребление</span><span class="sxs-lookup"><span data-stu-id="95c8c-825">Consumption</span></span>

* <span data-ttu-id="95c8c-826">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-826">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="95c8c-827">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-827">Event Grid</span></span>

* <span data-ttu-id="95c8c-828">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-828">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="95c8c-829">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-829">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="95c8c-830">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-830">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="95c8c-831">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-831">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="95c8c-832">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-832">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="95c8c-833">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-833">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="95c8c-834">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-834">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="95c8c-835">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-835">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="95c8c-836">Interactive</span><span class="sxs-lookup"><span data-stu-id="95c8c-836">Interactive</span></span>

* <span data-ttu-id="95c8c-837">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="95c8c-837">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="95c8c-838">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="95c8c-838">Fixed errors on startup</span></span>
* <span data-ttu-id="95c8c-839">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="95c8c-839">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="95c8c-840">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="95c8c-840">IoT</span></span>

* <span data-ttu-id="95c8c-841">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="95c8c-841">Added support for device provisioning service</span></span>
* <span data-ttu-id="95c8c-842">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="95c8c-842">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="95c8c-843">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="95c8c-843">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="95c8c-844">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="95c8c-844">Monitor</span></span>

* <span data-ttu-id="95c8c-845">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="95c8c-845">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="95c8c-846">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-846">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="95c8c-847">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="95c8c-847">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-848">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-848">Network</span></span>

* <span data-ttu-id="95c8c-849">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="95c8c-849">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="95c8c-850">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="95c8c-850">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="95c8c-851">Профиль</span><span class="sxs-lookup"><span data-stu-id="95c8c-851">Profile</span></span>

* <span data-ttu-id="95c8c-852">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-852">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="95c8c-853">Роль</span><span class="sxs-lookup"><span data-stu-id="95c8c-853">Role</span></span>

* <span data-ttu-id="95c8c-854">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-854">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="95c8c-855">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="95c8c-855">Service Fabric</span></span>

* <span data-ttu-id="95c8c-856">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="95c8c-856">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="95c8c-857">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="95c8c-857">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-858">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-858">VM</span></span>

* <span data-ttu-id="95c8c-859">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-859">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="95c8c-860">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="95c8c-860">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="95c8c-861">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-861">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="95c8c-862">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="95c8c-862">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="95c8c-863">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="95c8c-863">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="95c8c-864">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-864">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="95c8c-865">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-865">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="95c8c-866">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-866">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="95c8c-867">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-867">December 19, 2017</span></span>

<span data-ttu-id="95c8c-868">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="95c8c-868">Version 2.0.23</span></span>

* <span data-ttu-id="95c8c-869">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-869">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-870">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-870">Container</span></span>

* <span data-ttu-id="95c8c-871">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-871">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-872">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-872">Network</span></span>

* <span data-ttu-id="95c8c-873">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="95c8c-873">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="95c8c-874">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="95c8c-874">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-875">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-875">Storage</span></span>

* <span data-ttu-id="95c8c-876">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="95c8c-876">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-877">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-877">VM</span></span>

* <span data-ttu-id="95c8c-878">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="95c8c-878">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="95c8c-879">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-879">December 5, 2017</span></span>

<span data-ttu-id="95c8c-880">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="95c8c-880">Version 2.0.22</span></span>

* <span data-ttu-id="95c8c-881">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-881">Removed `az component` commands.</span></span> <span data-ttu-id="95c8c-882">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-882">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-883">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-883">Core</span></span>
* <span data-ttu-id="95c8c-884">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="95c8c-884">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="95c8c-885">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="95c8c-885">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-886">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-886">ACS</span></span>

* <span data-ttu-id="95c8c-887">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-887">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="95c8c-888">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-888">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="95c8c-889">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="95c8c-889">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="95c8c-890">Помощник</span><span class="sxs-lookup"><span data-stu-id="95c8c-890">Advisor</span></span>

* <span data-ttu-id="95c8c-891">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="95c8c-891">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-892">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-892">Appservice</span></span>

* <span data-ttu-id="95c8c-893">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-893">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="95c8c-894">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-894">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="95c8c-895">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-895">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="95c8c-896">Потребление</span><span class="sxs-lookup"><span data-stu-id="95c8c-896">Consumption</span></span>

* <span data-ttu-id="95c8c-897">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="95c8c-897">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-898">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-898">Container</span></span>

* <span data-ttu-id="95c8c-899">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="95c8c-899">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="95c8c-900">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="95c8c-900">Monitor</span></span>

* <span data-ttu-id="95c8c-901">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="95c8c-901">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-902">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-902">Resource</span></span>

* <span data-ttu-id="95c8c-903">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="95c8c-903">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="95c8c-904">Роль</span><span class="sxs-lookup"><span data-stu-id="95c8c-904">Role</span></span>

* <span data-ttu-id="95c8c-905">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-905">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="95c8c-906">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="95c8c-906">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="95c8c-907">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-907">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-908">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-908">SQL</span></span>

* <span data-ttu-id="95c8c-909">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-909">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="95c8c-910">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-910">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-911">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-911">VM</span></span>

* <span data-ttu-id="95c8c-912">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-912">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="95c8c-913">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-913">November 14, 2017</span></span>

<span data-ttu-id="95c8c-914">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="95c8c-914">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-915">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-915">ACR</span></span>

* <span data-ttu-id="95c8c-916">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="95c8c-916">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="95c8c-917">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-917">ACS</span></span>

* <span data-ttu-id="95c8c-918">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="95c8c-918">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="95c8c-919">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="95c8c-919">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="95c8c-920">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-920">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="95c8c-921">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="95c8c-921">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="95c8c-922">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="95c8c-922">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-923">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-923">Appservice</span></span>

* <span data-ttu-id="95c8c-924">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="95c8c-924">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="95c8c-925">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-925">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="95c8c-926">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-926">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="95c8c-927">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-927">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="95c8c-928">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="95c8c-928">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="95c8c-929">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="95c8c-929">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="95c8c-930">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-930">Batch</span></span>

* <span data-ttu-id="95c8c-931">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-931">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="95c8c-932">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="95c8c-932">Batchai</span></span>

* <span data-ttu-id="95c8c-933">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-933">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="95c8c-934">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-934">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="95c8c-935">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-935">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="95c8c-936">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-936">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="95c8c-937">Облако</span><span class="sxs-lookup"><span data-stu-id="95c8c-937">Cloud</span></span>

* <span data-ttu-id="95c8c-938">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-938">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-939">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-939">Container</span></span>

* <span data-ttu-id="95c8c-940">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-940">Added support to open multiple ports</span></span>
* <span data-ttu-id="95c8c-941">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-941">Added container group restart policy</span></span>
* <span data-ttu-id="95c8c-942">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="95c8c-942">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="95c8c-943">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="95c8c-943">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="95c8c-944">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="95c8c-944">Data Lake Analytics</span></span>

* <span data-ttu-id="95c8c-945">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-945">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="95c8c-946">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="95c8c-946">Data Lake Store</span></span>

* <span data-ttu-id="95c8c-947">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-947">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="95c8c-948">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="95c8c-948">Extension</span></span>

* <span data-ttu-id="95c8c-949">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="95c8c-949">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="95c8c-950">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="95c8c-950">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="95c8c-951">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="95c8c-951">IoT</span></span>

* <span data-ttu-id="95c8c-952">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-952">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="95c8c-953">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="95c8c-953">Monitor</span></span>

* <span data-ttu-id="95c8c-954">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-954">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-955">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-955">Network</span></span>

* <span data-ttu-id="95c8c-956">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="95c8c-956">Added support for CAA DNS records</span></span>
* <span data-ttu-id="95c8c-957">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-957">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="95c8c-958">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="95c8c-958">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="95c8c-959">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-959">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="95c8c-960">Резервирование</span><span class="sxs-lookup"><span data-stu-id="95c8c-960">Reservations</span></span>

* <span data-ttu-id="95c8c-961">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="95c8c-961">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-962">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-962">Resource</span></span>

* <span data-ttu-id="95c8c-963">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-963">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-964">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-964">SQL</span></span>

* <span data-ttu-id="95c8c-965">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-965">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-966">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-966">Storage</span></span>

* <span data-ttu-id="95c8c-967">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95c8c-967">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="95c8c-968">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="95c8c-968">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="95c8c-969">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-969">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="95c8c-970">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-970">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="95c8c-971">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-971">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="95c8c-972">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-972">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="95c8c-973">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-973">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-974">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-974">VM</span></span>

* <span data-ttu-id="95c8c-975">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-975">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="95c8c-976">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-976">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="95c8c-977">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-977">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="95c8c-978">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-978">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="95c8c-979">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="95c8c-979">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="95c8c-980">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-980">October 24, 2017</span></span>

<span data-ttu-id="95c8c-981">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="95c8c-981">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-982">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-982">Core</span></span>

* <span data-ttu-id="95c8c-983">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="95c8c-983">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-984">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-984">ACR</span></span>

* <span data-ttu-id="95c8c-985">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="95c8c-985">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="95c8c-986">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="95c8c-986">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="95c8c-987">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="95c8c-987">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-988">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-988">ACS</span></span>

* <span data-ttu-id="95c8c-989">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="95c8c-989">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="95c8c-990">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="95c8c-990">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-991">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-991">Appservice</span></span>

* <span data-ttu-id="95c8c-992">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="95c8c-992">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="95c8c-993">Компонент</span><span class="sxs-lookup"><span data-stu-id="95c8c-993">Component</span></span>

* <span data-ttu-id="95c8c-994">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="95c8c-994">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="95c8c-995">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="95c8c-995">Monitor</span></span>

* <span data-ttu-id="95c8c-996">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-996">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-997">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-997">Resource</span></span>

* <span data-ttu-id="95c8c-998">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="95c8c-998">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="95c8c-999">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="95c8c-999">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-1000">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-1000">VM</span></span>

* <span data-ttu-id="95c8c-1001">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1001">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="95c8c-1002">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1002">October 9, 2017</span></span>

<span data-ttu-id="95c8c-1003">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="95c8c-1003">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-1004">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-1004">Core</span></span>

* <span data-ttu-id="95c8c-1005">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1005">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-1006">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-1006">Appservice</span></span>

* <span data-ttu-id="95c8c-1007">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1007">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="95c8c-1008">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-1008">Batch</span></span>

* <span data-ttu-id="95c8c-1009">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="95c8c-1009">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="95c8c-1010">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1010">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="95c8c-1011">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1011">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="95c8c-1012">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1012">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="95c8c-1013">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="95c8c-1013">Batchai</span></span>

* <span data-ttu-id="95c8c-1014">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="95c8c-1014">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="95c8c-1015">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="95c8c-1015">Keyvault</span></span>

* <span data-ttu-id="95c8c-1016">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1016">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="95c8c-1017">(#4448)</span><span class="sxs-lookup"><span data-stu-id="95c8c-1017">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="95c8c-1018">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-1018">Network</span></span>

* <span data-ttu-id="95c8c-1019">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1019">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="95c8c-1020">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1020">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-1021">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-1021">Resource</span></span>

* <span data-ttu-id="95c8c-1022">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1022">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="95c8c-1023">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1023">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="95c8c-1024">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1024">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="95c8c-1025">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1025">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-1026">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-1026">Sql</span></span>

* <span data-ttu-id="95c8c-1027">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1027">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="95c8c-1028">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1028">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="95c8c-1029">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1029">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-1030">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-1030">Storage</span></span>

* <span data-ttu-id="95c8c-1031">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1031">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-1032">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="95c8c-1032">Vm</span></span>

* <span data-ttu-id="95c8c-1033">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1033">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="95c8c-1034">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1034">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="95c8c-1035">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1035">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="95c8c-1036">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1036">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="95c8c-1037">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1037">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="95c8c-1038">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1038">September 22, 2017</span></span>

<span data-ttu-id="95c8c-1039">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="95c8c-1039">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-1040">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-1040">Resource</span></span>

* <span data-ttu-id="95c8c-1041">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="95c8c-1041">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="95c8c-1042">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="95c8c-1042">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="95c8c-1043">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1043">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="95c8c-1044">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1044">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-1045">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-1045">Network</span></span>

* <span data-ttu-id="95c8c-1046">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1046">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="95c8c-1047">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1047">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="95c8c-1048">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1048">Added `asg` application security group commands</span></span>
* <span data-ttu-id="95c8c-1049">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1049">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="95c8c-1050">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1050">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="95c8c-1051">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1051">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="95c8c-1052">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1052">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-1053">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-1053">Storage</span></span>

* <span data-ttu-id="95c8c-1054">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="95c8c-1054">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="95c8c-1055">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="95c8c-1055">Eventgrid</span></span>

* <span data-ttu-id="95c8c-1056">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="95c8c-1056">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-1057">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-1057">SQL</span></span>

* <span data-ttu-id="95c8c-1058">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1058">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="95c8c-1059">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="95c8c-1059">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="95c8c-1060">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1060">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="95c8c-1061">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="95c8c-1061">Keyvault</span></span>

* <span data-ttu-id="95c8c-1062">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="95c8c-1062">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-1063">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-1063">VM</span></span>

* <span data-ttu-id="95c8c-1064">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1064">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="95c8c-1065">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="95c8c-1065">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="95c8c-1066">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1066">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="95c8c-1067">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1067">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="95c8c-1068">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1068">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="95c8c-1069">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1069">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-1070">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-1070">ACS</span></span>

* <span data-ttu-id="95c8c-1071">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="95c8c-1071">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-1072">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-1072">Appservice</span></span>

* <span data-ttu-id="95c8c-1073">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="95c8c-1073">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="95c8c-1074">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="95c8c-1074">Backup</span></span>

* <span data-ttu-id="95c8c-1075">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1075">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="95c8c-1076">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1076">September 11, 2017</span></span>

<span data-ttu-id="95c8c-1077">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="95c8c-1077">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="95c8c-1078">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-1078">Core</span></span>

* <span data-ttu-id="95c8c-1079">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1079">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="95c8c-1080">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1080">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-1081">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-1081">Acs</span></span>

* <span data-ttu-id="95c8c-1082">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1082">Added `acs list-locations` command</span></span>
* <span data-ttu-id="95c8c-1083">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1083">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-1084">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-1084">Appservice</span></span>

* <span data-ttu-id="95c8c-1085">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1085">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="95c8c-1086">CDN</span><span class="sxs-lookup"><span data-stu-id="95c8c-1086">CDN</span></span>

* <span data-ttu-id="95c8c-1087">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1087">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="95c8c-1088">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="95c8c-1088">Extension</span></span>

* <span data-ttu-id="95c8c-1089">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="95c8c-1089">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="95c8c-1090">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="95c8c-1090">Keyvault</span></span>

* <span data-ttu-id="95c8c-1091">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1091">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-1092">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-1092">Network</span></span>

* <span data-ttu-id="95c8c-1093">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1093">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="95c8c-1094">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1094">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="95c8c-1095">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1095">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="95c8c-1096">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1096">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="95c8c-1097">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1097">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-1098">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-1098">Resource</span></span>

* <span data-ttu-id="95c8c-1099">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1099">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="95c8c-1100">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1100">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="95c8c-1101">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1101">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="95c8c-1102">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1102">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-1103">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-1103">SQL</span></span>

* <span data-ttu-id="95c8c-1104">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1104">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-1105">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-1105">VM</span></span>

* <span data-ttu-id="95c8c-1106">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1106">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="95c8c-1107">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1107">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="95c8c-1108">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1108">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="95c8c-1109">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1109">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="95c8c-1110">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1110">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="95c8c-1111">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1111">August 31, 2017</span></span>

<span data-ttu-id="95c8c-1112">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="95c8c-1112">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="95c8c-1113">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="95c8c-1113">Keyvault</span></span>

* <span data-ttu-id="95c8c-1114">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1114">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="95c8c-1115">Sf</span><span class="sxs-lookup"><span data-stu-id="95c8c-1115">Sf</span></span>

* <span data-ttu-id="95c8c-1116">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1116">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-1117">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-1117">Storage</span></span>

* <span data-ttu-id="95c8c-1118">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1118">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="95c8c-1119">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1119">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="95c8c-1120">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1120">August 28, 2017</span></span>

<span data-ttu-id="95c8c-1121">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="95c8c-1121">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="95c8c-1122">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="95c8c-1122">CLI</span></span>

* <span data-ttu-id="95c8c-1123">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1123">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-1124">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-1124">ACS</span></span>

* <span data-ttu-id="95c8c-1125">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1125">Corrected preview regions</span></span>
* <span data-ttu-id="95c8c-1126">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1126">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="95c8c-1127">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1127">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-1128">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-1128">Appservice</span></span>

* <span data-ttu-id="95c8c-1129">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1129">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="95c8c-1130">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1130">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="95c8c-1131">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1131">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="95c8c-1132">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1132">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="95c8c-1133">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1133">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="95c8c-1134">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="95c8c-1134">IoT</span></span>

* <span data-ttu-id="95c8c-1135">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1135">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-1136">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-1136">Network</span></span>

* <span data-ttu-id="95c8c-1137">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1137">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="95c8c-1138">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1138">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="95c8c-1139">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1139">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="95c8c-1140">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1140">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="95c8c-1141">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1141">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="95c8c-1142">Профиль</span><span class="sxs-lookup"><span data-stu-id="95c8c-1142">Profile</span></span>

* <span data-ttu-id="95c8c-1143">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1143">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="95c8c-1144">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="95c8c-1144">Service Fabric</span></span>

* <span data-ttu-id="95c8c-1145">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1145">Preview release</span></span>
* <span data-ttu-id="95c8c-1146">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1146">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="95c8c-1147">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1147">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="95c8c-1148">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1148">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-1149">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-1149">Storage</span></span>

* <span data-ttu-id="95c8c-1150">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1150">Enabled setting blob tier</span></span>
* <span data-ttu-id="95c8c-1151">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1151">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="95c8c-1152">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1152">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="95c8c-1153">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1153">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="95c8c-1154">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1154">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="95c8c-1155">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1155">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-1156">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-1156">VM</span></span>

* <span data-ttu-id="95c8c-1157">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1157">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="95c8c-1158">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1158">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="95c8c-1159">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1159">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="95c8c-1160">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1160">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="95c8c-1161">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1161">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="95c8c-1162">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1162">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="95c8c-1163">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1163">August 15, 2017</span></span>

<span data-ttu-id="95c8c-1164">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="95c8c-1164">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-1165">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-1165">ACS</span></span>

* <span data-ttu-id="95c8c-1166">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1166">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-1167">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-1167">Appservice</span></span>

* <span data-ttu-id="95c8c-1168">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1168">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="95c8c-1169">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-1169">Event Grid</span></span>

* <span data-ttu-id="95c8c-1170">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1170">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="95c8c-1171">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1171">August 11, 2017</span></span>

<span data-ttu-id="95c8c-1172">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="95c8c-1172">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-1173">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-1173">ACS</span></span>

* <span data-ttu-id="95c8c-1174">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1174">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="95c8c-1175">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-1175">Batch</span></span>

* <span data-ttu-id="95c8c-1176">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1176">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="95c8c-1177">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1177">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="95c8c-1178">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1178">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="95c8c-1179">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1179">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="95c8c-1180">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1180">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="95c8c-1181">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1181">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="95c8c-1182">Компонент</span><span class="sxs-lookup"><span data-stu-id="95c8c-1182">Component</span></span>

* <span data-ttu-id="95c8c-1183">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1183">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="95c8c-1184">Контейнер</span><span class="sxs-lookup"><span data-stu-id="95c8c-1184">Container</span></span>

* <span data-ttu-id="95c8c-1185">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1185">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="95c8c-1186">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="95c8c-1186">Data Lake Store</span></span>

* <span data-ttu-id="95c8c-1187">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1187">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="95c8c-1188">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-1188">Event Grid</span></span>

* <span data-ttu-id="95c8c-1189">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="95c8c-1189">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-1190">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-1190">Network</span></span>

* <span data-ttu-id="95c8c-1191">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1191">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="95c8c-1192">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1192">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="95c8c-1193">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1193">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="95c8c-1194">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1194">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="95c8c-1195">Профиль</span><span class="sxs-lookup"><span data-stu-id="95c8c-1195">Profile</span></span>

* <span data-ttu-id="95c8c-1196">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1196">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-1197">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-1197">Storage</span></span>

* <span data-ttu-id="95c8c-1198">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1198">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-1199">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-1199">VM</span></span>

* <span data-ttu-id="95c8c-1200">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1200">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="95c8c-1201">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1201">Exposed `list-skus` command</span></span>
* <span data-ttu-id="95c8c-1202">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1202">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="95c8c-1203">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1203">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="95c8c-1204">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1204">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="95c8c-1205">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1205">July 28, 2017</span></span>

<span data-ttu-id="95c8c-1206">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="95c8c-1206">Version 2.0.12</span></span>

* <span data-ttu-id="95c8c-1207">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1207">Added container commands</span></span>
* <span data-ttu-id="95c8c-1208">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1208">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="95c8c-1209">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-1209">Core</span></span>

* <span data-ttu-id="95c8c-1210">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1210">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="95c8c-1211">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1211">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="95c8c-1212">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1212">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="95c8c-1213">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1213">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="95c8c-1214">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1214">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="95c8c-1215">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1215">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="95c8c-1216">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1216">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="95c8c-1217">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1217">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="95c8c-1218">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1218">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="95c8c-1219">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1219">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="95c8c-1220">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1220">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="95c8c-1221">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1221">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="95c8c-1222">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1222">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="95c8c-1223">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1223">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="95c8c-1224">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1224">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="95c8c-1225">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1225">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="95c8c-1226">ACR</span><span class="sxs-lookup"><span data-stu-id="95c8c-1226">ACR</span></span>

* <span data-ttu-id="95c8c-1227">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1227">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="95c8c-1228">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1228">Support SKU update for managed registries</span></span>
* <span data-ttu-id="95c8c-1229">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1229">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="95c8c-1230">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1230">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="95c8c-1231">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1231">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="95c8c-1232">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1232">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-1233">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-1233">ACS</span></span>

* <span data-ttu-id="95c8c-1234">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1234">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-1235">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="95c8c-1235">Appservice</span></span>

* <span data-ttu-id="95c8c-1236">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1236">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="95c8c-1237">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1237">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="95c8c-1238">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1238">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="95c8c-1239">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1239">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="95c8c-1240">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1240">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="95c8c-1241">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1241">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="95c8c-1242">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1242">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="95c8c-1243">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1243">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="95c8c-1244">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1244">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="95c8c-1245">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1245">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="95c8c-1246">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="95c8c-1246">Batch</span></span>

* <span data-ttu-id="95c8c-1247">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1247">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="95c8c-1248">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1248">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="95c8c-1249">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1249">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="95c8c-1250">CDN</span><span class="sxs-lookup"><span data-stu-id="95c8c-1250">CDN</span></span>

* <span data-ttu-id="95c8c-1251">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1251">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="95c8c-1252">Облако</span><span class="sxs-lookup"><span data-stu-id="95c8c-1252">Cloud</span></span>

* <span data-ttu-id="95c8c-1253">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1253">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="95c8c-1254">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1254">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="95c8c-1255">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1255">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="95c8c-1256">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1256">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="95c8c-1257">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1257">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="95c8c-1258">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="95c8c-1258">CosmosDB</span></span>

* <span data-ttu-id="95c8c-1259">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1259">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="95c8c-1260">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1260">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="95c8c-1261">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="95c8c-1261">Data Lake Analytics</span></span>

* <span data-ttu-id="95c8c-1262">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1262">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="95c8c-1263">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1263">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="95c8c-1264">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1264">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="95c8c-1265">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="95c8c-1265">Data Lake Store</span></span>

* <span data-ttu-id="95c8c-1266">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1266">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="95c8c-1267">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1267">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="95c8c-1268">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1268">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="95c8c-1269">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1269">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="95c8c-1270">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="95c8c-1270">Interactive</span></span>

* <span data-ttu-id="95c8c-1271">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1271">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="95c8c-1272">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1272">Increased test coverage</span></span>
* <span data-ttu-id="95c8c-1273">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1273">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="95c8c-1274">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1274">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="95c8c-1275">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1275">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="95c8c-1276">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1276">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="95c8c-1277">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1277">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="95c8c-1278">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1278">Added `--progress` flag</span></span>
* <span data-ttu-id="95c8c-1279">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1279">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="95c8c-1280">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1280">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="95c8c-1281">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="95c8c-1281">IoT</span></span>

* <span data-ttu-id="95c8c-1282">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="95c8c-1282">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="95c8c-1283">(3934).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1283">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="95c8c-1284">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="95c8c-1284">Key vault</span></span>

* <span data-ttu-id="95c8c-1285">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="95c8c-1285">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="95c8c-1286">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1286">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="95c8c-1287">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="95c8c-1287">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="95c8c-1288">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="95c8c-1288">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="95c8c-1289">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1289">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="95c8c-1290">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1290">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="95c8c-1291">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="95c8c-1291">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="95c8c-1292">(3307).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1292">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="95c8c-1293">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="95c8c-1293">Lab</span></span>

* <span data-ttu-id="95c8c-1294">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1294">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="95c8c-1295">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1295">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="95c8c-1296">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="95c8c-1296">Monitor</span></span>

* <span data-ttu-id="95c8c-1297">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1297">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="95c8c-1298">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1298">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="95c8c-1299">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1299">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="95c8c-1300">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1300">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="95c8c-1301">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1301">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="95c8c-1302">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="95c8c-1302">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="95c8c-1303">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="95c8c-1303">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="95c8c-1304">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="95c8c-1304">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="95c8c-1305">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="95c8c-1305">`location` no longer required</span></span>
  * <span data-ttu-id="95c8c-1306">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="95c8c-1306">Add name and ID support for target</span></span>
  * <span data-ttu-id="95c8c-1307">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="95c8c-1307">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="95c8c-1308">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="95c8c-1308">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="95c8c-1309">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="95c8c-1309">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="95c8c-1310">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1310">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="95c8c-1311">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1311">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="95c8c-1312">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1312">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-1313">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-1313">Network</span></span>

* <span data-ttu-id="95c8c-1314">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1314">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="95c8c-1315">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1315">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="95c8c-1316">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1316">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="95c8c-1317">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1317">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="95c8c-1318">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1318">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="95c8c-1319">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1319">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="95c8c-1320">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1320">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="95c8c-1321">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1321">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="95c8c-1322">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1322">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="95c8c-1323">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1323">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="95c8c-1324">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1324">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="95c8c-1325">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1325">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="95c8c-1326">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1326">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="95c8c-1327">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1327">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="95c8c-1328">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1328">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="95c8c-1329">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1329">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="95c8c-1330">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1330">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="95c8c-1331">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1331">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="95c8c-1332">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1332">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="95c8c-1333">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1333">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="95c8c-1334">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1334">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="95c8c-1335">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1335">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="95c8c-1336">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1336">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="95c8c-1337">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1337">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="95c8c-1338">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1338">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="95c8c-1339">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1339">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="95c8c-1340">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1340">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="95c8c-1341">Профиль</span><span class="sxs-lookup"><span data-stu-id="95c8c-1341">Profile</span></span>

* <span data-ttu-id="95c8c-1342">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1342">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="95c8c-1343">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1343">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="95c8c-1344">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1344">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="95c8c-1345">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1345">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="95c8c-1346">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1346">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="95c8c-1347">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="95c8c-1347">RDBMS</span></span>

* <span data-ttu-id="95c8c-1348">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1348">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="95c8c-1349">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1349">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="95c8c-1350">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1350">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="95c8c-1351">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1351">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-1352">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-1352">Resource</span></span>

* <span data-ttu-id="95c8c-1353">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1353">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="95c8c-1354">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1354">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="95c8c-1355">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1355">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="95c8c-1356">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1356">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="95c8c-1357">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1357">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="95c8c-1358">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1358">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="95c8c-1359">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1359">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="95c8c-1360">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1360">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="95c8c-1361">Роль</span><span class="sxs-lookup"><span data-stu-id="95c8c-1361">Role</span></span>

* <span data-ttu-id="95c8c-1362">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1362">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="95c8c-1363">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1363">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="95c8c-1364">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1364">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="95c8c-1365">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1365">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="95c8c-1366">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1366">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="95c8c-1367">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="95c8c-1367">Service Fabric</span></span>
* <span data-ttu-id="95c8c-1368">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1368">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="95c8c-1369">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1369">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="95c8c-1370">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1370">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-1371">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-1371">SQL</span></span>

* <span data-ttu-id="95c8c-1372">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1372">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="95c8c-1373">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1373">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="95c8c-1374">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1374">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-1375">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-1375">Storage</span></span>

* <span data-ttu-id="95c8c-1376">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1376">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="95c8c-1377">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1377">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="95c8c-1378">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1378">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="95c8c-1379">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="95c8c-1379">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="95c8c-1380">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1380">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="95c8c-1381">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1381">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-1382">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-1382">VM</span></span>

* <span data-ttu-id="95c8c-1383">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1383">Support configuring nsg</span></span>
* <span data-ttu-id="95c8c-1384">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1384">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="95c8c-1385">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1385">Support managed service identities</span></span>
* <span data-ttu-id="95c8c-1386">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1386">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="95c8c-1387">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1387">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="95c8c-1388">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1388">May 10, 2017</span></span>

<span data-ttu-id="95c8c-1389">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="95c8c-1389">Version 2.0.6</span></span>

* <span data-ttu-id="95c8c-1390">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1390">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="95c8c-1391">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1391">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="95c8c-1392">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1392">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="95c8c-1393">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1393">Include Cognitive Services module</span></span>
* <span data-ttu-id="95c8c-1394">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1394">Include Service Fabric module</span></span>
* <span data-ttu-id="95c8c-1395">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1395">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="95c8c-1396">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1396">Add support for CDN commands</span></span>
* <span data-ttu-id="95c8c-1397">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1397">Remove Container module</span></span>
* <span data-ttu-id="95c8c-1398">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1398">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="95c8c-1399">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1399">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="95c8c-1400">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-1400">Core</span></span>

* <span data-ttu-id="95c8c-1401">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1401">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="95c8c-1402">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1402">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="95c8c-1403">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1403">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="95c8c-1404">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1404">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="95c8c-1405">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1405">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="95c8c-1406">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1406">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="95c8c-1407">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1407">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="95c8c-1408">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1408">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="95c8c-1409">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1409">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="95c8c-1410">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1410">core: Improved performance</span></span>
* <span data-ttu-id="95c8c-1411">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1411">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="95c8c-1412">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1412">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-1413">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-1413">ACS</span></span>

* <span data-ttu-id="95c8c-1414">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1414">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="95c8c-1415">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1415">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="95c8c-1416">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1416">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="95c8c-1417">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1417">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-1418">AppService</span><span class="sxs-lookup"><span data-stu-id="95c8c-1418">AppService</span></span>

* <span data-ttu-id="95c8c-1419">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1419">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="95c8c-1420">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1420">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="95c8c-1421">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1421">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="95c8c-1422">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1422">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="95c8c-1423">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1423">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="95c8c-1424">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1424">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="95c8c-1425">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1425">support slot swap with preview</span></span>
* <span data-ttu-id="95c8c-1426">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1426">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="95c8c-1427">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1427">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="95c8c-1428">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="95c8c-1428">CosmosDB</span></span>

* <span data-ttu-id="95c8c-1429">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1429">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="95c8c-1430">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1430">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="95c8c-1431">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1431">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="95c8c-1432">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1432">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="95c8c-1433">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="95c8c-1433">Data Lake Analytics</span></span>

* <span data-ttu-id="95c8c-1434">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1434">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="95c8c-1435">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1435">Add support for new catalog item type: package.</span></span> <span data-ttu-id="95c8c-1436">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1436">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="95c8c-1437">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="95c8c-1437">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="95c8c-1438">Таблица</span><span class="sxs-lookup"><span data-stu-id="95c8c-1438">Table</span></span>
  * <span data-ttu-id="95c8c-1439">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="95c8c-1439">Table valued function</span></span>
  * <span data-ttu-id="95c8c-1440">Просмотр</span><span class="sxs-lookup"><span data-stu-id="95c8c-1440">View</span></span>
  * <span data-ttu-id="95c8c-1441">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1441">Table Statistics.</span></span> <span data-ttu-id="95c8c-1442">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1442">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="95c8c-1443">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="95c8c-1443">Data Lake Store</span></span>

* <span data-ttu-id="95c8c-1444">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1444">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="95c8c-1445">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1445">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="95c8c-1446">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1446">missed help for access show.</span></span> <span data-ttu-id="95c8c-1447">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1447">adding it.</span></span> <span data-ttu-id="95c8c-1448">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="95c8c-1448">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="95c8c-1449">Поиск</span><span class="sxs-lookup"><span data-stu-id="95c8c-1449">Find</span></span>

* <span data-ttu-id="95c8c-1450">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1450">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="95c8c-1451">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="95c8c-1451">KeyVault</span></span>

* <span data-ttu-id="95c8c-1452">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1452">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="95c8c-1453">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1453">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="95c8c-1454">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1454">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="95c8c-1455">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1455">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="95c8c-1456">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1456">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="95c8c-1457">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="95c8c-1457">Lab</span></span>

* <span data-ttu-id="95c8c-1458">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1458">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="95c8c-1459">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1459">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="95c8c-1460">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1460">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="95c8c-1461">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1461">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="95c8c-1462">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1462">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="95c8c-1463">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="95c8c-1463">Monitor</span></span>

* <span data-ttu-id="95c8c-1464">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1464">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="95c8c-1465">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1465">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="95c8c-1466">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-1466">Network</span></span>

* <span data-ttu-id="95c8c-1467">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1467">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="95c8c-1468">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1468">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="95c8c-1469">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1469">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="95c8c-1470">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1470">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="95c8c-1471">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1471">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="95c8c-1472">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1472">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="95c8c-1473">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1473">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="95c8c-1474">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1474">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="95c8c-1475">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1475">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="95c8c-1476">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="95c8c-1476">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="95c8c-1477">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1477">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="95c8c-1478">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1478">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="95c8c-1479">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1479">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="95c8c-1480">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1480">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="95c8c-1481">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1481">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="95c8c-1482">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1482">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="95c8c-1483">Профиль</span><span class="sxs-lookup"><span data-stu-id="95c8c-1483">Profile</span></span>

* <span data-ttu-id="95c8c-1484">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1484">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="95c8c-1485">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1485">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="95c8c-1486">Redis</span><span class="sxs-lookup"><span data-stu-id="95c8c-1486">Redis</span></span>

* <span data-ttu-id="95c8c-1487">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1487">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="95c8c-1488">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1488">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="95c8c-1489">Ресурс</span><span class="sxs-lookup"><span data-stu-id="95c8c-1489">Resource</span></span>

* <span data-ttu-id="95c8c-1490">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1490">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="95c8c-1491">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1491">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="95c8c-1492">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1492">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="95c8c-1493">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1493">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="95c8c-1494">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="95c8c-1494">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="95c8c-1495">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1495">Add docs for az lock update.</span></span> <span data-ttu-id="95c8c-1496">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="95c8c-1496">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="95c8c-1497">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1497">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="95c8c-1498">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="95c8c-1498">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="95c8c-1499">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1499">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="95c8c-1500">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="95c8c-1500">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="95c8c-1501">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1501">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="95c8c-1502">Роль</span><span class="sxs-lookup"><span data-stu-id="95c8c-1502">Role</span></span>

* <span data-ttu-id="95c8c-1503">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1503">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="95c8c-1504">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1504">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="95c8c-1505">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1505">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="95c8c-1506">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1506">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="95c8c-1507">SQL</span><span class="sxs-lookup"><span data-stu-id="95c8c-1507">SQL</span></span>

* <span data-ttu-id="95c8c-1508">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1508">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="95c8c-1509">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1509">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="95c8c-1510">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-1510">Storage</span></span>

* <span data-ttu-id="95c8c-1511">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1511">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="95c8c-1512">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1512">Add support for incremental blob copy</span></span>
* <span data-ttu-id="95c8c-1513">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1513">Add support for large block blob upload</span></span>
* <span data-ttu-id="95c8c-1514">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1514">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-1515">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-1515">VM</span></span>

* <span data-ttu-id="95c8c-1516">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1516">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="95c8c-1517">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="95c8c-1517">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="95c8c-1518">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="95c8c-1518">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="95c8c-1519">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="95c8c-1519">az vm/vmss disk</span></span>
  3. <span data-ttu-id="95c8c-1520">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1520">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="95c8c-1521">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1521">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="95c8c-1522">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1522">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="95c8c-1523">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1523">April 3, 2017</span></span>

<span data-ttu-id="95c8c-1524">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="95c8c-1524">Version 2.0.2</span></span>

<span data-ttu-id="95c8c-1525">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1525">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="95c8c-1526">Core</span><span class="sxs-lookup"><span data-stu-id="95c8c-1526">Core</span></span>

* <span data-ttu-id="95c8c-1527">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1527">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="95c8c-1528">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1528">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="95c8c-1529">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1529">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="95c8c-1530">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1530">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="95c8c-1531">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1531">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="95c8c-1532">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="95c8c-1532">Add prompting for missing template parameters.</span></span> <span data-ttu-id="95c8c-1533">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1533">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="95c8c-1534">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1534">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="95c8c-1535">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1535">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="95c8c-1536">ACS</span><span class="sxs-lookup"><span data-stu-id="95c8c-1536">ACS</span></span>

* <span data-ttu-id="95c8c-1537">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1537">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="95c8c-1538">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="95c8c-1538">Add support for ssh key password prompting.</span></span> <span data-ttu-id="95c8c-1539">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1539">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="95c8c-1540">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="95c8c-1540">Add support for windows clusters.</span></span> <span data-ttu-id="95c8c-1541">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1541">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="95c8c-1542">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="95c8c-1542">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="95c8c-1543">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1543">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="95c8c-1544">AppService</span><span class="sxs-lookup"><span data-stu-id="95c8c-1544">AppService</span></span>

* <span data-ttu-id="95c8c-1545">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1545">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="95c8c-1546">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1546">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="95c8c-1547">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1547">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="95c8c-1548">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1548">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="95c8c-1549">Data Lake</span><span class="sxs-lookup"><span data-stu-id="95c8c-1549">DataLake</span></span>

* <span data-ttu-id="95c8c-1550">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1550">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="95c8c-1551">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1551">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="95c8c-1552">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="95c8c-1552">DocuemntDB</span></span>

* <span data-ttu-id="95c8c-1553">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1553">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="95c8c-1554">ВМ</span><span class="sxs-lookup"><span data-stu-id="95c8c-1554">VM</span></span>

* <span data-ttu-id="95c8c-1555">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1555">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="95c8c-1556">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1556">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="95c8c-1557">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1557">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="95c8c-1558">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1558">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="95c8c-1559">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1559">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="95c8c-1560">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1560">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="95c8c-1561">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1561">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="95c8c-1562">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1562">February 27, 2017</span></span>

<span data-ttu-id="95c8c-1563">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="95c8c-1563">Version 2.0.0</span></span>

<span data-ttu-id="95c8c-1564">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="95c8c-1564">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="95c8c-1565">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="95c8c-1565">Container Service (acs)</span></span>
- <span data-ttu-id="95c8c-1566">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="95c8c-1566">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="95c8c-1567">Сеть</span><span class="sxs-lookup"><span data-stu-id="95c8c-1567">Networking</span></span>
- <span data-ttu-id="95c8c-1568">Хранилище</span><span class="sxs-lookup"><span data-stu-id="95c8c-1568">Storage</span></span>

<span data-ttu-id="95c8c-1569">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1569">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="95c8c-1570">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1570">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="95c8c-1571">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1571">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="95c8c-1572">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1572">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="95c8c-1573">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="95c8c-1573">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="95c8c-1574">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="95c8c-1574">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="95c8c-1575">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="95c8c-1575">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="95c8c-1576">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="95c8c-1576">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="95c8c-1577">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="95c8c-1577">Provide feedback from the command line with the `az feedback` command</span></span>

