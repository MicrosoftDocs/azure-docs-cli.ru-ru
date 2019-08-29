---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: sptramer
ms.author: sttramer
manager: carmonm
ms.date: 08/27/2019
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: 156ff2e6d011104ebbb1608ff33bad8ebb6396ed
ms.sourcegitcommit: df2be5609a6cbeecb9f8ef0928a9fabfb207e7f9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/27/2019
ms.locfileid: "70047269"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="550f1-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="550f1-103">Azure CLI release notes</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="550f1-104">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-104">August 27, 2019</span></span>

<span data-ttu-id="550f1-105">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="550f1-105">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-106">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-106">ACR</span></span>

* <span data-ttu-id="550f1-107">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="550f1-107">[BREAKING CHNAGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="550f1-108">Управление API</span><span class="sxs-lookup"><span data-stu-id="550f1-108">API Management</span></span>

* <span data-ttu-id="550f1-109">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="550f1-109">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-110">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-110">AppService</span></span>

* <span data-ttu-id="550f1-111">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="550f1-111">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="550f1-112">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="550f1-112">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="550f1-113">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="550f1-113">Keyvault</span></span>

* <span data-ttu-id="550f1-114">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="550f1-114">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="550f1-115">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-115">Network</span></span>

* <span data-ttu-id="550f1-116">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="550f1-116">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="550f1-117">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="550f1-117">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="550f1-118">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="550f1-118">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="550f1-119">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="550f1-119">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="550f1-120">RBAC</span><span class="sxs-lookup"><span data-stu-id="550f1-120">RBAC</span></span>

* <span data-ttu-id="550f1-121">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="550f1-121">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="550f1-122">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="550f1-122">ServiceFabric</span></span>

* <span data-ttu-id="550f1-123">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="550f1-123">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="550f1-124">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="550f1-124">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="550f1-125">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="550f1-125">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="550f1-126">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="550f1-126">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="550f1-127">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="550f1-127">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="550f1-128">SignalR</span><span class="sxs-lookup"><span data-stu-id="550f1-128">SignalR</span></span>

* <span data-ttu-id="550f1-129">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="550f1-129">Added new commands:</span></span>
  * <span data-ttu-id="550f1-130">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="550f1-130">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="550f1-131">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="550f1-131">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="550f1-132">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="550f1-132">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="550f1-133">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="550f1-133">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-134">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-134">Storage</span></span>

* <span data-ttu-id="550f1-135">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="550f1-135">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="550f1-136">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-136">August 13, 2019</span></span>

<span data-ttu-id="550f1-137">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="550f1-137">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-138">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-138">AppService</span></span>

* <span data-ttu-id="550f1-139">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="550f1-139">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="550f1-140">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="550f1-140">BotService</span></span>

* <span data-ttu-id="550f1-141">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="550f1-141">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="550f1-142">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="550f1-142">CognitiveServices</span></span>

* <span data-ttu-id="550f1-143">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="550f1-143">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="550f1-144">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-144">Cosmos DB</span></span>

* <span data-ttu-id="550f1-145">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="550f1-145">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="550f1-146">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-146">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="550f1-147">HDInsight</span><span class="sxs-lookup"><span data-stu-id="550f1-147">HDInsight</span></span>

<span data-ttu-id="550f1-148">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="550f1-148">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="550f1-149">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="550f1-149">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="550f1-150">Команда `--storage-default-container` переименована в `--storage-container`.</span><span class="sxs-lookup"><span data-stu-id="550f1-150">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="550f1-151">Команда `--storage-default-filesystem` переименована в `--storage-filesystem`.</span><span class="sxs-lookup"><span data-stu-id="550f1-151">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="550f1-152">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="550f1-152">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="550f1-153">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-153">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="550f1-154">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="550f1-154">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="550f1-155">Команда `--application-type` переименована в `--type`.</span><span class="sxs-lookup"><span data-stu-id="550f1-155">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="550f1-156">Команда `--marketplace-identifier` переименована в `--marketplace-id`.</span><span class="sxs-lookup"><span data-stu-id="550f1-156">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="550f1-157">Команда `--https-endpoint-access-mode` переименована в `--access-mode`.</span><span class="sxs-lookup"><span data-stu-id="550f1-157">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="550f1-158">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="550f1-158">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="550f1-159">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="550f1-159">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="550f1-160">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="550f1-160">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="550f1-161">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="550f1-161">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="550f1-162">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-162">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="550f1-163">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="550f1-163">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="550f1-164">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="550f1-164">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="550f1-165">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="550f1-165">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="550f1-166">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-166">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="550f1-167">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="550f1-167">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="550f1-168">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="550f1-168">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="550f1-169">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="550f1-169">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="550f1-170">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="550f1-170">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="550f1-171">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="550f1-171">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-172">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-172">Interactive</span></span>

* <span data-ttu-id="550f1-173">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="550f1-173">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="550f1-174">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="550f1-174">Kubernetes</span></span>

* <span data-ttu-id="550f1-175">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="550f1-175">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-176">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-176">Network</span></span>

* <span data-ttu-id="550f1-177">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="550f1-177">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-178">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-178">Profile</span></span>

* <span data-ttu-id="550f1-179">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="550f1-179">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="550f1-180">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="550f1-180">ServiceFabric</span></span>

* <span data-ttu-id="550f1-181">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="550f1-181">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="550f1-182">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="550f1-182">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-183">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-183">Storage</span></span>

* <span data-ttu-id="550f1-184">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="550f1-184">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="550f1-185">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-185">July 30, 2019</span></span>

<span data-ttu-id="550f1-186">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="550f1-186">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-187">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-187">ACR</span></span>

* <span data-ttu-id="550f1-188">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="550f1-188">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="550f1-189">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="550f1-189">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-190">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-190">Appservice</span></span>

* <span data-ttu-id="550f1-191">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="550f1-191">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="550f1-192">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="550f1-192">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="550f1-193">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="550f1-193">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="550f1-194">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-194">Network</span></span>

* <span data-ttu-id="550f1-195">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="550f1-195">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="550f1-196">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="550f1-196">Fixes #9604.</span></span> <span data-ttu-id="550f1-197">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="550f1-197">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="550f1-198">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="550f1-198">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="550f1-199">RBAC</span><span class="sxs-lookup"><span data-stu-id="550f1-199">RBAC</span></span>

* <span data-ttu-id="550f1-200">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-200">Added `user update` command</span></span>
* <span data-ttu-id="550f1-201">[УСТАРЕЛО] `--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="550f1-201">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="550f1-202">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="550f1-202">Use replacement argument `--id`</span></span>
* <span data-ttu-id="550f1-203">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="550f1-203">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-204">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-204">SQL</span></span>

* <span data-ttu-id="550f1-205">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="550f1-205">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-206">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-206">Storage</span></span>

* <span data-ttu-id="550f1-207">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="550f1-207">Added `storage remove` command</span></span>
* <span data-ttu-id="550f1-208">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-208">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-209">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-209">VM</span></span>

* <span data-ttu-id="550f1-210">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="550f1-210">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="550f1-211">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-211">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="550f1-212">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-212">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="550f1-213">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="550f1-213">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="550f1-214">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="550f1-214">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="550f1-215">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-215">July 16, 2019</span></span>

<span data-ttu-id="550f1-216">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="550f1-216">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-217">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-217">Appservice</span></span>

* <span data-ttu-id="550f1-218">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="550f1-218">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="550f1-219">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="550f1-219">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="550f1-220">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-220">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="550f1-221">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-221">Core</span></span>

* <span data-ttu-id="550f1-222">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="550f1-222">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-223">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-223">Batch</span></span>

* <span data-ttu-id="550f1-224">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-224">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="550f1-225">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="550f1-225">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="550f1-226">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-226">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="550f1-227">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-227">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="550f1-228">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="550f1-228">Eventhubs</span></span>

* <span data-ttu-id="550f1-229">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="550f1-229">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-230">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="550f1-230">RDBMS</span></span>

* <span data-ttu-id="550f1-231">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="550f1-231">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="550f1-232">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="550f1-232">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="550f1-233">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="550f1-233">Relay</span></span>

* <span data-ttu-id="550f1-234">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="550f1-234">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="550f1-235">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-235">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="550f1-236">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="550f1-236">Servicebus</span></span>

* <span data-ttu-id="550f1-237">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="550f1-237">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-238">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-238">Storage</span></span>

* <span data-ttu-id="550f1-239">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="550f1-239">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="550f1-240">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="550f1-240">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="550f1-241">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-241">July 2, 2019</span></span>

<span data-ttu-id="550f1-242">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="550f1-242">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="550f1-243">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-243">Core</span></span>

* <span data-ttu-id="550f1-244">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="550f1-244">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="550f1-245">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="550f1-245">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="550f1-246">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="550f1-246">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-247">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-247">ACR</span></span>

* <span data-ttu-id="550f1-248">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="550f1-248">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-249">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-249">Appservice</span></span>

* <span data-ttu-id="550f1-250">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-250">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="550f1-251">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="550f1-251">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="550f1-252">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="550f1-252">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="550f1-253">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="550f1-253">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="550f1-254">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-254">Cosmos DB</span></span>

* <span data-ttu-id="550f1-255">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="550f1-255">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="550f1-256">DLS</span><span class="sxs-lookup"><span data-stu-id="550f1-256">DLS</span></span>

* <span data-ttu-id="550f1-257">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="550f1-257">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="550f1-258">Отзыв</span><span class="sxs-lookup"><span data-stu-id="550f1-258">Feedback</span></span>

* <span data-ttu-id="550f1-259">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="550f1-259">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="550f1-260">HDInsight</span><span class="sxs-lookup"><span data-stu-id="550f1-260">HDInsight</span></span>

* <span data-ttu-id="550f1-261">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="550f1-261">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="550f1-262">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="550f1-262">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="550f1-263">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="550f1-263">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="550f1-264">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="550f1-264">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="550f1-265">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="550f1-265">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="550f1-266">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="550f1-266">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="550f1-267">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-267">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="550f1-268">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="550f1-268">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="550f1-269">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-269">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="550f1-270">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="550f1-270">Managed Services</span></span>

* <span data-ttu-id="550f1-271">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="550f1-271">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-272">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-272">Profile</span></span>
* <span data-ttu-id="550f1-273">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="550f1-273">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="550f1-274">RBAC</span><span class="sxs-lookup"><span data-stu-id="550f1-274">RBAC</span></span>

* <span data-ttu-id="550f1-275">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="550f1-275">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="550f1-276">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="550f1-276">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="550f1-277">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="550f1-277">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="550f1-278">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="550f1-278">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-279">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="550f1-279">RDBMS</span></span>

* <span data-ttu-id="550f1-280">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="550f1-280">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-281">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-281">SQL</span></span>

* <span data-ttu-id="550f1-282">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-282">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-283">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-283">Storage</span></span>

* <span data-ttu-id="550f1-284">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="550f1-284">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="550f1-285">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="550f1-285">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="550f1-286">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-286">VM</span></span>

* <span data-ttu-id="550f1-287">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-287">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="550f1-288">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="550f1-288">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="550f1-289">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="550f1-289">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="550f1-290">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="550f1-290">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="550f1-291">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-291">June 18, 2019</span></span>

<span data-ttu-id="550f1-292">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="550f1-292">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="550f1-293">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-293">Core</span></span>

<span data-ttu-id="550f1-294">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="550f1-294">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="550f1-295">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="550f1-295">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="550f1-296">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="550f1-296">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="550f1-297">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="550f1-297">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="550f1-298">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="550f1-298">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="550f1-299">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="550f1-299">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="550f1-300">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="550f1-300">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-301">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-301">ACR</span></span>
* <span data-ttu-id="550f1-302">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="550f1-302">Added 'acr check-health' command</span></span>
* <span data-ttu-id="550f1-303">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-303">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-304">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-304">ACS</span></span>
* <span data-ttu-id="550f1-305">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="550f1-305">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="550f1-306">AMS</span><span class="sxs-lookup"><span data-stu-id="550f1-306">AMS</span></span>
* <span data-ttu-id="550f1-307">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="550f1-307">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-308">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-308">AppService</span></span>
* <span data-ttu-id="550f1-309">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="550f1-309">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="550f1-310">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="550f1-310">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="550f1-311">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="550f1-311">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="550f1-312">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-312">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="550f1-313">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="550f1-313">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="550f1-314">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="550f1-314">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-315">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-315">Batch</span></span>
* <span data-ttu-id="550f1-316">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="550f1-316">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="550f1-317">Batch AI</span><span class="sxs-lookup"><span data-stu-id="550f1-317">BatchAI</span></span>
* <span data-ttu-id="550f1-318">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="550f1-318">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="550f1-319">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="550f1-319">BotService</span></span>
* <span data-ttu-id="550f1-320">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="550f1-320">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="550f1-321">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-321">CosmosDB</span></span>
* <span data-ttu-id="550f1-322">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="550f1-322">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="550f1-323">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="550f1-323">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="550f1-324">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="550f1-324">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="550f1-325">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="550f1-325">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="550f1-326">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="550f1-326">EventGrid</span></span>
* <span data-ttu-id="550f1-327">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="550f1-327">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="550f1-328">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="550f1-328">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="550f1-329">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="550f1-329">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="550f1-330">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="550f1-330">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="550f1-331">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-331">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="550f1-332">HDInsight</span><span class="sxs-lookup"><span data-stu-id="550f1-332">HDInsight</span></span>
* <span data-ttu-id="550f1-333">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-333">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-334">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-334">IoT</span></span>
* <span data-ttu-id="550f1-335">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="550f1-335">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="550f1-336">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="550f1-336">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="550f1-337">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-337">Network</span></span>
* <span data-ttu-id="550f1-338">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="550f1-338">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="550f1-339">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="550f1-339">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="550f1-340">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="550f1-340">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="550f1-341">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="550f1-341">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-342">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-342">Resource</span></span>
* <span data-ttu-id="550f1-343">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="550f1-343">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="550f1-344">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="550f1-344">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="550f1-345">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="550f1-345">ServiceBus</span></span>
* <span data-ttu-id="550f1-346">Исправлена ошибка [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="550f1-346">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-347">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-347">SQL</span></span>
* <span data-ttu-id="550f1-348">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-348">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="550f1-349">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="550f1-349">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="550f1-350">SQLVm</span><span class="sxs-lookup"><span data-stu-id="550f1-350">SQLVm</span></span>
* <span data-ttu-id="550f1-351">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="550f1-351">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="550f1-352">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="550f1-352">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-353">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-353">Storage</span></span>
* <span data-ttu-id="550f1-354">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="550f1-354">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="550f1-355">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="550f1-355">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-356">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-356">VM</span></span>
* <span data-ttu-id="550f1-357">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="550f1-357">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="550f1-358">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-358">June 4, 2019</span></span>

<span data-ttu-id="550f1-359">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="550f1-359">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="550f1-360">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-360">Core</span></span>
* <span data-ttu-id="550f1-361">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="550f1-361">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-362">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-362">ACR</span></span>
* <span data-ttu-id="550f1-363">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="550f1-363">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-364">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-364">ACS</span></span>
* <span data-ttu-id="550f1-365">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="550f1-365">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="550f1-366">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="550f1-366">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-367">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-367">Batch</span></span>
* <span data-ttu-id="550f1-368">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="550f1-368">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-369">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-369">IoT</span></span>
* <span data-ttu-id="550f1-370">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="550f1-370">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="550f1-371">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-371">Network</span></span>
* <span data-ttu-id="550f1-372">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="550f1-372">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="550f1-373">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="550f1-373">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="550f1-374">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-374">Resource</span></span>
* <span data-ttu-id="550f1-375">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="550f1-375">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="550f1-376">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-376">Role</span></span>
* <span data-ttu-id="550f1-377">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="550f1-377">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="550f1-378">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="550f1-378">Compute</span></span>
* <span data-ttu-id="550f1-379">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="550f1-379">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="550f1-380">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-380">May 21, 2019</span></span>

<span data-ttu-id="550f1-381">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="550f1-381">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="550f1-382">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-382">Core</span></span>
* <span data-ttu-id="550f1-383">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="550f1-383">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="550f1-384">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="550f1-384">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="550f1-385">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="550f1-385">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-386">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-386">ACR</span></span>
* <span data-ttu-id="550f1-387">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="550f1-387">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-388">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-388">ACS</span></span>
* <span data-ttu-id="550f1-389">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="550f1-389">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-390">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-390">AppService</span></span>
* <span data-ttu-id="550f1-391">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="550f1-391">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="550f1-392">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="550f1-392">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="550f1-393">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="550f1-393">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="550f1-394">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="550f1-394">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="550f1-395">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="550f1-395">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="550f1-396">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="550f1-396">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="550f1-397">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="550f1-397">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="550f1-398">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="550f1-398">BotService</span></span>
* <span data-ttu-id="550f1-399">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-399">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="550f1-400">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="550f1-400">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="550f1-401">Потребление</span><span class="sxs-lookup"><span data-stu-id="550f1-401">Consumption</span></span>
* <span data-ttu-id="550f1-402">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-402">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-403">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-403">IoT</span></span>
* <span data-ttu-id="550f1-404">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="550f1-404">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="550f1-405">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-405">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="550f1-407">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="550f1-407">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="550f1-408">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="550f1-408">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-409">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="550f1-409">RDBMS</span></span>
* <span data-ttu-id="550f1-410">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="550f1-410">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="550f1-411">RBAC</span><span class="sxs-lookup"><span data-stu-id="550f1-411">RBAC</span></span>
* <span data-ttu-id="550f1-412">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="550f1-412">Added support for mangement group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-413">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-413">Storage</span></span>
* <span data-ttu-id="550f1-414">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="550f1-414">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="550f1-415">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="550f1-415">Compute</span></span>
* <span data-ttu-id="550f1-416">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="550f1-416">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="550f1-417">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="550f1-417">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="550f1-418">__Примечание__. Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="550f1-418">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="550f1-419">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="550f1-419">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="550f1-420">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-420">May 6, 2019</span></span>

<span data-ttu-id="550f1-421">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="550f1-421">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-422">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-422">ACS</span></span>
* <span data-ttu-id="550f1-423">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="550f1-423">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="550f1-424">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="550f1-424">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="550f1-425">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-425">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="550f1-426">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="550f1-426">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-427">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-427">Appservice</span></span>
* <span data-ttu-id="550f1-428">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="550f1-428">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="550f1-429">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="550f1-429">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="550f1-430">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="550f1-430">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="550f1-431">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="550f1-431">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="550f1-432">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="550f1-432">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="550f1-433">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="550f1-433">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="550f1-434">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="550f1-434">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="550f1-435">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="550f1-435">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="550f1-436">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="550f1-436">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="550f1-437">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="550f1-437">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-438">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-438">Batch</span></span>
* <span data-ttu-id="550f1-439">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="550f1-439">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="550f1-440">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="550f1-440">Botservice</span></span>
* <span data-ttu-id="550f1-441">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="550f1-441">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="550f1-442">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="550f1-442">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="550f1-443">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="550f1-443">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="550f1-444">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-444">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="550f1-445">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-445">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="550f1-446">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="550f1-446">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="550f1-447">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-447">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="550f1-448">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="550f1-448">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="550f1-449">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="550f1-449">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="550f1-450">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="550f1-450">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="550f1-451">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="550f1-451">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="550f1-452">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="550f1-452">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="550f1-453">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="550f1-453">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="550f1-454">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="550f1-454">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="550f1-455">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-455">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="550f1-456">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="550f1-456">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="550f1-457">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="550f1-457">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="550f1-458">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="550f1-458">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="550f1-459">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="550f1-459">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="550f1-460">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="550f1-460">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="550f1-461">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="550f1-461">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="550f1-462">Настройка</span><span class="sxs-lookup"><span data-stu-id="550f1-462">Configure</span></span>
* <span data-ttu-id="550f1-463">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="550f1-463">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="550f1-464">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="550f1-464">Eventhubs</span></span>
* <span data-ttu-id="550f1-465">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="550f1-465">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="550f1-466">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-466">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-467">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-467">Network</span></span>
* <span data-ttu-id="550f1-468">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-468">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="550f1-469">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="550f1-469">Policy Insights</span></span>
* <span data-ttu-id="550f1-470">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="550f1-470">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="550f1-471">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-471">Role</span></span>
* <span data-ttu-id="550f1-472">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="550f1-472">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="550f1-473">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="550f1-473">Service Bus</span></span>
* <span data-ttu-id="550f1-474">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="550f1-474">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="550f1-475">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-475">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="550f1-476">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="550f1-476">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-477">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-477">SQL</span></span>
* <span data-ttu-id="550f1-478">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-478">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-479">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-479">VM</span></span>
* <span data-ttu-id="550f1-480">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="550f1-480">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="550f1-481">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="550f1-481">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="550f1-482">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-482">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="550f1-483">Добавлена новая группа команд `ppg` для управления группами размещения близкого расположения.</span><span class="sxs-lookup"><span data-stu-id="550f1-483">Added new `ppg` command group for manging Proximity Placement Groups</span></span>
* <span data-ttu-id="550f1-484">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="550f1-484">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="550f1-485">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-485">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="550f1-486">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-486">April 23, 2019</span></span>

<span data-ttu-id="550f1-487">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="550f1-487">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-488">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-488">ACS</span></span>
* <span data-ttu-id="550f1-489">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="550f1-489">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="550f1-490">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="550f1-490">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="550f1-491">AMS</span><span class="sxs-lookup"><span data-stu-id="550f1-491">AMS</span></span>
* <span data-ttu-id="550f1-492">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="550f1-492">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-493">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-493">AppService</span></span>
* <span data-ttu-id="550f1-494">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="550f1-494">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="550f1-495">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="550f1-495">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="550f1-496">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="550f1-496">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="550f1-497">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="550f1-497">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="550f1-498">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-498">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="550f1-499">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="550f1-499">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="550f1-500">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="550f1-500">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="550f1-501">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="550f1-501">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="550f1-502">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="550f1-502">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="550f1-503">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="550f1-503">Deployment Manager</span></span>
* <span data-ttu-id="550f1-504">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="550f1-504">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="550f1-505">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="550f1-505">Lab</span></span>
* <span data-ttu-id="550f1-506">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="550f1-506">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="550f1-507">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-507">Network</span></span>
* <span data-ttu-id="550f1-508">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="550f1-508">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-509">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-509">Resource</span></span>
* <span data-ttu-id="550f1-510">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="550f1-510">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="550f1-511">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="550f1-511">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="550f1-512">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="550f1-512">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="550f1-513">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="550f1-513">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-514">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-514">SQL</span></span>
* <span data-ttu-id="550f1-515">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="550f1-515">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="550f1-516">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-516">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="550f1-517">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-517">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="550f1-518">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-518">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-519">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-519">Storage</span></span>
* <span data-ttu-id="550f1-520">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="550f1-520">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-521">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-521">VM</span></span>
* <span data-ttu-id="550f1-522">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="550f1-522">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="550f1-523">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="550f1-523">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="550f1-524">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="550f1-524">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="550f1-525">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-525">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="550f1-526">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-526">Core</span></span>
* <span data-ttu-id="550f1-527">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="550f1-527">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-528">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-528">ACR</span></span>
* <span data-ttu-id="550f1-529">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="550f1-529">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="550f1-530">AMS</span><span class="sxs-lookup"><span data-stu-id="550f1-530">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="550f1-533">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-533">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="550f1-534">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-534">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-535">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-535">AppService</span></span>
* <span data-ttu-id="550f1-536">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="550f1-536">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="550f1-537">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="550f1-537">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="550f1-538">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-538">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="550f1-539">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="550f1-539">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="550f1-540">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="550f1-540">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="550f1-541">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="550f1-541">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="550f1-542">Добавлена поддержка параметров масштабирования плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="550f1-542">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="550f1-543">CDN</span><span class="sxs-lookup"><span data-stu-id="550f1-543">CDN</span></span>
* <span data-ttu-id="550f1-544">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="550f1-544">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="550f1-545">Отзыв</span><span class="sxs-lookup"><span data-stu-id="550f1-545">Feedback</span></span>
* <span data-ttu-id="550f1-546">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-546">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="550f1-547">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="550f1-547">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="550f1-548">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="550f1-548">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-549">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-549">Monitor</span></span>
* <span data-ttu-id="550f1-550">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-550">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="550f1-551">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-551">Network</span></span>
* <span data-ttu-id="550f1-552">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="550f1-552">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="550f1-553">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="550f1-553">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="550f1-554">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="550f1-554">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="550f1-555">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-555">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="550f1-556">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="550f1-556">PrivateDNS</span></span>
* <span data-ttu-id="550f1-557">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="550f1-557">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-558">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-558">Resource</span></span>
* <span data-ttu-id="550f1-559">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="550f1-559">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="550f1-560">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-560">Role</span></span>
* <span data-ttu-id="550f1-561">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="550f1-561">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="550f1-562">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="550f1-562">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-563">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-563">SQL</span></span>
* <span data-ttu-id="550f1-564">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="550f1-564">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-565">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-565">Storage</span></span>
* <span data-ttu-id="550f1-566">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="550f1-566">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="550f1-567">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="550f1-567">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="550f1-568">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="550f1-568">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="550f1-569">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="550f1-569">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="550f1-570">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-570">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="550f1-571">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-571">Core</span></span>
* <span data-ttu-id="550f1-572">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="550f1-572">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="550f1-573">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="550f1-573">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="550f1-574">Облако</span><span class="sxs-lookup"><span data-stu-id="550f1-574">Cloud</span></span>
* <span data-ttu-id="550f1-575">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="550f1-575">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-576">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-576">ACR</span></span>
* <span data-ttu-id="550f1-577">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="550f1-577">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="550f1-578">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-578">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="550f1-579">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="550f1-579">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="550f1-580">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="550f1-580">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-581">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-581">AppService</span></span>
* <span data-ttu-id="550f1-582">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="550f1-582">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="550f1-583">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="550f1-583">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="550f1-584">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="550f1-584">BOT Service</span></span>
* <span data-ttu-id="550f1-585">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="550f1-585">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="550f1-586">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="550f1-586">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="550f1-587">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="550f1-587">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="550f1-588">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="550f1-588">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="550f1-589">CDN</span><span class="sxs-lookup"><span data-stu-id="550f1-589">CDN</span></span>
* <span data-ttu-id="550f1-590">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-590">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="550f1-591">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-591">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="550f1-592">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-592">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="550f1-593">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="550f1-593">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="550f1-594">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-594">Cosmosdb</span></span>
* <span data-ttu-id="550f1-595">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="550f1-595">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="550f1-596">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="550f1-596">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-597">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-597">Interactive</span></span>
* <span data-ttu-id="550f1-598">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="550f1-598">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-599">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-599">Monitor</span></span>
* <span data-ttu-id="550f1-600">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-600">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-601">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-601">Network</span></span>
* <span data-ttu-id="550f1-602">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="550f1-602">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-603">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-603">Profile</span></span>
* <span data-ttu-id="550f1-604">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="550f1-604">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="550f1-605">Postgres</span><span class="sxs-lookup"><span data-stu-id="550f1-605">Postgres</span></span> 
* <span data-ttu-id="550f1-606">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="550f1-606">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="550f1-607">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="550f1-607">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-608">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-608">Resource</span></span>
* <span data-ttu-id="550f1-609">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-609">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="550f1-610">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="550f1-610">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="550f1-611">График</span><span class="sxs-lookup"><span data-stu-id="550f1-611">Graph</span></span>
* <span data-ttu-id="550f1-612">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="550f1-612">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="550f1-613">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="550f1-613">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="550f1-614">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="550f1-614">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="550f1-615">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="550f1-615">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="550f1-616">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="550f1-616">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-617">storage</span><span class="sxs-lookup"><span data-stu-id="550f1-617">storage</span></span>
* <span data-ttu-id="550f1-618">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="550f1-618">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="550f1-619">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="550f1-619">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="550f1-620">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="550f1-620">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="550f1-621">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="550f1-621">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-622">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-622">VM</span></span>
* <span data-ttu-id="550f1-623">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-623">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="550f1-624">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-624">March 12, 2019</span></span>

<span data-ttu-id="550f1-625">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="550f1-625">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="550f1-626">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-626">Core</span></span>

* <span data-ttu-id="550f1-627">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="550f1-627">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-628">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-628">ACR</span></span>

* <span data-ttu-id="550f1-629">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="550f1-629">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-630">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-630">ACS</span></span>

* <span data-ttu-id="550f1-631">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="550f1-631">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="550f1-632">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-632">AppService</span></span>

* <span data-ttu-id="550f1-633">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="550f1-633">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="550f1-634">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-634">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="550f1-635">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="550f1-635">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="550f1-636">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="550f1-636">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="550f1-637">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="550f1-637">Botservice</span></span>

* <span data-ttu-id="550f1-638">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="550f1-638">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="550f1-639">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="550f1-639">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="550f1-640">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-640">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="550f1-641">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="550f1-641">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="550f1-642">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-642">Container</span></span>

* <span data-ttu-id="550f1-643">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="550f1-643">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="550f1-644">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="550f1-644">EventHub</span></span>

* <span data-ttu-id="550f1-645">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="550f1-645">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="550f1-646">Поиск</span><span class="sxs-lookup"><span data-stu-id="550f1-646">Find</span></span>

* <span data-ttu-id="550f1-647">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="550f1-647">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="550f1-648">HDInsight</span><span class="sxs-lookup"><span data-stu-id="550f1-648">HDInsight</span></span>

* <span data-ttu-id="550f1-649">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="550f1-649">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="550f1-650">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-650">Network</span></span>

* <span data-ttu-id="550f1-651">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="550f1-651">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-652">Rdbms</span><span class="sxs-lookup"><span data-stu-id="550f1-652">Rdbms</span></span>

* <span data-ttu-id="550f1-653">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="550f1-653">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="550f1-654">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-654">Role</span></span>

* <span data-ttu-id="550f1-655">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="550f1-655">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="550f1-656">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="550f1-656">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="550f1-657">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="550f1-657">Service Fabric</span></span>

* <span data-ttu-id="550f1-658">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="550f1-658">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="550f1-659">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-659">February 26, 2019</span></span>

<span data-ttu-id="550f1-660">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="550f1-660">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="550f1-661">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-661">Core</span></span>

* <span data-ttu-id="550f1-662">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="550f1-662">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-663">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-663">ACR</span></span>

* <span data-ttu-id="550f1-664">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-664">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="550f1-665">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="550f1-665">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-666">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-666">ACS</span></span>

* <span data-ttu-id="550f1-667">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="550f1-667">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-668">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-668">AppService</span></span>

* <span data-ttu-id="550f1-669">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="550f1-669">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-670">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-670">Batch</span></span>
* <span data-ttu-id="550f1-671">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="550f1-671">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="550f1-672">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="550f1-672">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="550f1-673">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="550f1-673">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="550f1-674">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="550f1-674">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="550f1-675">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="550f1-675">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="550f1-676">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="550f1-676">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="550f1-677">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-677">CosmosDB</span></span>

* <span data-ttu-id="550f1-678">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="550f1-678">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="550f1-679">Kusto</span><span class="sxs-lookup"><span data-stu-id="550f1-679">Kusto</span></span>

* <span data-ttu-id="550f1-680">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="550f1-680">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="550f1-681">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-681">Network</span></span>

* <span data-ttu-id="550f1-682">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="550f1-682">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="550f1-683">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="550f1-683">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="550f1-684">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="550f1-684">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="550f1-685">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-685">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="550f1-686">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-686">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="550f1-687">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="550f1-687">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="550f1-688">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="550f1-688">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-689">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-689">Resource</span></span>

* <span data-ttu-id="550f1-690">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="550f1-690">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="550f1-691">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-691">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="550f1-692">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-692">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="550f1-693">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-693">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="550f1-694">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="550f1-694">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="550f1-695">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-695">Role</span></span>

* <span data-ttu-id="550f1-696">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-696">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-697">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-697">VM</span></span>

* <span data-ttu-id="550f1-698">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="550f1-698">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="550f1-699">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-699">February 12, 2019</span></span>

<span data-ttu-id="550f1-700">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="550f1-700">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="550f1-701">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-701">Core</span></span>

* <span data-ttu-id="550f1-702">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="550f1-702">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="550f1-703">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="550f1-703">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-704">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-704">ACR</span></span>
* <span data-ttu-id="550f1-705">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="550f1-705">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="550f1-706">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="550f1-706">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-707">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-707">ACS</span></span>
* <span data-ttu-id="550f1-708">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="550f1-708">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="550f1-709">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="550f1-709">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="550f1-710">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="550f1-710">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="550f1-711">AMS</span><span class="sxs-lookup"><span data-stu-id="550f1-711">AMS</span></span>
* <span data-ttu-id="550f1-712">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-712">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="550f1-713">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-713">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-714">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-714">Appservice</span></span>
* <span data-ttu-id="550f1-715">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="550f1-715">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="550f1-716">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="550f1-716">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="550f1-717">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-717">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="550f1-718">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="550f1-718">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="550f1-719">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="550f1-719">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="550f1-720">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="550f1-720">Botservice</span></span>
* <span data-ttu-id="550f1-721">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="550f1-721">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="550f1-722">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="550f1-722">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="550f1-723">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-723">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="550f1-724">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="550f1-724">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="550f1-725">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="550f1-725">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="550f1-726">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="550f1-726">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="550f1-727">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="550f1-727">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="550f1-728">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="550f1-728">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="550f1-729">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="550f1-729">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="550f1-730">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="550f1-730">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="550f1-731">Key Vault</span><span class="sxs-lookup"><span data-stu-id="550f1-731">Key Vault</span></span>
* <span data-ttu-id="550f1-732">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="550f1-732">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-733">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-733">Monitor</span></span>
* <span data-ttu-id="550f1-734">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="550f1-734">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-735">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-735">Network</span></span>
* <span data-ttu-id="550f1-736">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="550f1-736">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="550f1-737">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="550f1-737">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="550f1-738">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="550f1-738">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="550f1-739">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="550f1-739">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="550f1-740">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="550f1-740">Policy Insights</span></span>
* <span data-ttu-id="550f1-741">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-741">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-742">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="550f1-742">RDBMS</span></span>
* <span data-ttu-id="550f1-743">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="550f1-743">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="550f1-744">Redis</span><span class="sxs-lookup"><span data-stu-id="550f1-744">Redis</span></span>
* <span data-ttu-id="550f1-745">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="550f1-745">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="550f1-746">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="550f1-746">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="550f1-747">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="550f1-747">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="550f1-748">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="550f1-748">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="550f1-749">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="550f1-749">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="550f1-750">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="550f1-750">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="550f1-751">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="550f1-751">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="550f1-752">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-752">Role</span></span>
* <span data-ttu-id="550f1-753">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="550f1-753">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="550f1-754">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-754">SQL VM</span></span>
* <span data-ttu-id="550f1-755">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="550f1-755">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-756">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-756">VM</span></span>
* <span data-ttu-id="550f1-757">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="550f1-757">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="550f1-758">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-758">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="550f1-759">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="550f1-759">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="550f1-760">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="550f1-760">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="550f1-761">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-761">January 31, 2019</span></span>

<span data-ttu-id="550f1-762">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="550f1-762">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="550f1-763">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-763">Core</span></span>

* <span data-ttu-id="550f1-764">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="550f1-764">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="550f1-765">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-765">January 28, 2019</span></span>

<span data-ttu-id="550f1-766">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="550f1-766">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-767">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-767">ACR</span></span>
* <span data-ttu-id="550f1-768">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="550f1-768">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-769">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-769">ACS</span></span>
* <span data-ttu-id="550f1-770">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="550f1-770">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="550f1-771">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="550f1-771">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="550f1-772">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="550f1-772">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="550f1-773">AMS</span><span class="sxs-lookup"><span data-stu-id="550f1-773">AMS</span></span>
* <span data-ttu-id="550f1-774">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="550f1-774">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="550f1-775">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="550f1-775">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-776">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-776">Appservice</span></span>
* <span data-ttu-id="550f1-777">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-777">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="550f1-778">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="550f1-778">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="550f1-779">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="550f1-779">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="550f1-780">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-780">Container</span></span>
* <span data-ttu-id="550f1-781">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="550f1-781">Added `container start` command</span></span>
* <span data-ttu-id="550f1-782">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-782">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="550f1-783">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="550f1-783">EventGrid</span></span>
* <span data-ttu-id="550f1-784">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-784">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="550f1-785">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="550f1-785">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="550f1-786">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="550f1-786">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="550f1-787">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="550f1-787">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="550f1-788">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="550f1-788">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="550f1-789">HDInsight</span><span class="sxs-lookup"><span data-stu-id="550f1-789">HDInsight</span></span>
* <span data-ttu-id="550f1-790">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-790">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="550f1-791">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="550f1-791">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="550f1-792">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-792">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="550f1-793">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="550f1-793">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="550f1-794">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="550f1-794">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="550f1-795">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-795">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-796">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-796">IoT</span></span>
* <span data-ttu-id="550f1-797">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="550f1-797">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="550f1-798">Kusto</span><span class="sxs-lookup"><span data-stu-id="550f1-798">Kusto</span></span>
* <span data-ttu-id="550f1-799">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="550f1-799">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-800">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-800">Monitor</span></span>
* <span data-ttu-id="550f1-801">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="550f1-801">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-802">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-802">Profile</span></span>
* <span data-ttu-id="550f1-803">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-803">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-804">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-804">Network</span></span>
* <span data-ttu-id="550f1-805">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="550f1-805">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="550f1-806">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="550f1-806">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-807">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-807">Resource</span></span>
* <span data-ttu-id="550f1-808">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-808">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="550f1-809">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-809">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="550f1-810">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-810">SQL Virtual Machine</span></span>
* <span data-ttu-id="550f1-811">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="550f1-811">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-812">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-812">Storage</span></span>
* <span data-ttu-id="550f1-813">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="550f1-813">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="550f1-814">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="550f1-814">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-815">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-815">VM</span></span>
* <span data-ttu-id="550f1-816">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="550f1-816">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="550f1-817">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="550f1-817">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="550f1-818">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-818">January 15, 2019</span></span>

<span data-ttu-id="550f1-819">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="550f1-819">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-820">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-820">ACR</span></span>
* <span data-ttu-id="550f1-821">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="550f1-821">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="550f1-822">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="550f1-822">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="550f1-823">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="550f1-823">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="550f1-824">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-824">ACS</span></span>
* <span data-ttu-id="550f1-825">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="550f1-825">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-826">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-826">Appservice</span></span>
* <span data-ttu-id="550f1-827">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="550f1-827">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="550f1-828">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="550f1-828">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="550f1-829">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="550f1-829">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="550f1-830">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="550f1-830">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="550f1-831">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="550f1-831">Botservice</span></span>
* <span data-ttu-id="550f1-832">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-832">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="550f1-833">Настройка</span><span class="sxs-lookup"><span data-stu-id="550f1-833">Configure</span></span>
* <span data-ttu-id="550f1-834">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="550f1-834">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="550f1-835">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-835">CosmosDB</span></span>
* <span data-ttu-id="550f1-836">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="550f1-836">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="550f1-837">HDInsight</span><span class="sxs-lookup"><span data-stu-id="550f1-837">HDInsight</span></span>
* <span data-ttu-id="550f1-838">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="550f1-838">Added commands for managing applications</span></span>
* <span data-ttu-id="550f1-839">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="550f1-839">Added commands for managing script actions</span></span>
* <span data-ttu-id="550f1-840">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="550f1-840">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="550f1-841">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="550f1-841">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="550f1-842">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-842">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-843">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-843">Network</span></span>
* <span data-ttu-id="550f1-844">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="550f1-844">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="550f1-845">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="550f1-845">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="550f1-846">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="550f1-846">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="550f1-847">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-847">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="550f1-848">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-848">Role</span></span>
* <span data-ttu-id="550f1-849">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="550f1-849">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="550f1-850">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="550f1-850">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="550f1-851">Безопасность</span><span class="sxs-lookup"><span data-stu-id="550f1-851">Security</span></span>
* <span data-ttu-id="550f1-852">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="550f1-852">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-853">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-853">Storage</span></span>
* <span data-ttu-id="550f1-854">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="550f1-854">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="550f1-855">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="550f1-855">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="550f1-856">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-856">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="550f1-857">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-857">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="550f1-858">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="550f1-858">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-859">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-859">VM</span></span>
* <span data-ttu-id="550f1-860">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="550f1-860">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="550f1-861">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-861">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="550f1-862">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="550f1-862">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="550f1-863">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="550f1-863">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="550f1-864">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-864">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="550f1-865">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="550f1-865">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="550f1-866">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-866">December 20, 2018</span></span>

<span data-ttu-id="550f1-867">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="550f1-867">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="550f1-868">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-868">Appservice</span></span>
* <span data-ttu-id="550f1-869">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="550f1-869">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="550f1-870">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="550f1-870">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="550f1-871">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="550f1-871">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="550f1-872">IoT Central</span><span class="sxs-lookup"><span data-stu-id="550f1-872">IoTCentral</span></span>
* <span data-ttu-id="550f1-873">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="550f1-873">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="550f1-874">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-874">Role</span></span>
* <span data-ttu-id="550f1-875">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="550f1-875">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-876">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-876">SQL</span></span>
* <span data-ttu-id="550f1-877">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="550f1-877">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-878">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-878">VM</span></span>
* <span data-ttu-id="550f1-879">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-879">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="550f1-880">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-880">December 18, 2018</span></span>

<span data-ttu-id="550f1-881">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="550f1-881">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="550f1-882">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-882">ACR</span></span>
* <span data-ttu-id="550f1-883">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-883">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="550f1-884">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="550f1-884">Condensed the table layout for task list</span></span>
* <span data-ttu-id="550f1-885">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="550f1-885">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-886">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-886">ACS</span></span>
* <span data-ttu-id="550f1-887">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="550f1-887">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="550f1-888">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="550f1-888">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="550f1-889">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="550f1-889">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="550f1-890">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-890">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="550f1-891">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="550f1-891">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="550f1-892">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="550f1-892">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-893">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-893">Appservice</span></span>
* <span data-ttu-id="550f1-894">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="550f1-894">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="550f1-895">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="550f1-895">Botservice</span></span>
* <span data-ttu-id="550f1-896">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-896">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="550f1-897">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="550f1-897">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="550f1-898">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="550f1-898">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="550f1-899">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="550f1-899">Reduced Kudu network calls</span></span>
* <span data-ttu-id="550f1-900">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-900">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="550f1-901">Потребление</span><span class="sxs-lookup"><span data-stu-id="550f1-901">Consumption</span></span>
* <span data-ttu-id="550f1-902">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="550f1-902">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="550f1-903">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-903">CosmosDB</span></span>
* <span data-ttu-id="550f1-904">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="550f1-904">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="550f1-905">Maps</span><span class="sxs-lookup"><span data-stu-id="550f1-905">Maps</span></span>
* <span data-ttu-id="550f1-906">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="550f1-906">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-907">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-907">Network</span></span>
* <span data-ttu-id="550f1-908">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="550f1-908">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="550f1-909">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="550f1-909">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-910">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-910">Resource</span></span>
* <span data-ttu-id="550f1-911">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-911">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="550f1-912">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-912">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-913">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-913">Storage</span></span>
*  <span data-ttu-id="550f1-914">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="550f1-914">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-915">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-915">VM</span></span>
* <span data-ttu-id="550f1-916">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-916">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="550f1-917">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-917">December 4, 2018</span></span>

<span data-ttu-id="550f1-918">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="550f1-918">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="550f1-919">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-919">Core</span></span>
* <span data-ttu-id="550f1-920">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-920">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="550f1-921">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="550f1-921">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-922">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-922">Appservice</span></span>
* <span data-ttu-id="550f1-923">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="550f1-923">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="550f1-924">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="550f1-924">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="550f1-925">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-925">Network</span></span>
* <span data-ttu-id="550f1-926">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="550f1-926">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="550f1-927">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-927">Role</span></span>
* <span data-ttu-id="550f1-928">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="550f1-928">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="550f1-929">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-929">VM</span></span>
* <span data-ttu-id="550f1-930">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="550f1-930">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="550f1-931">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="550f1-931">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="550f1-932">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="550f1-932">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="550f1-933">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="550f1-933">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="550f1-934">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-934">November 20, 2018</span></span>

<span data-ttu-id="550f1-935">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="550f1-935">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="550f1-936">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-936">Core</span></span>
* <span data-ttu-id="550f1-937">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="550f1-937">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-938">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-938">ACR</span></span>
* <span data-ttu-id="550f1-939">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="550f1-939">Added context token to task step</span></span>
* <span data-ttu-id="550f1-940">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="550f1-940">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="550f1-941">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="550f1-941">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-942">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-942">Appservice</span></span>
* <span data-ttu-id="550f1-943">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="550f1-943">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="550f1-944">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-944">Updated the default `node_version`.</span></span> <span data-ttu-id="550f1-945">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="550f1-945">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="550f1-946">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="550f1-946">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="550f1-947">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="550f1-947">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="550f1-948">IotCentral</span><span class="sxs-lookup"><span data-stu-id="550f1-948">IotCentral</span></span>
* <span data-ttu-id="550f1-949">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="550f1-949">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="550f1-950">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="550f1-950">KeyVault</span></span>
* <span data-ttu-id="550f1-951">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="550f1-951">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="550f1-952">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-952">Network</span></span>
* <span data-ttu-id="550f1-953">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="550f1-953">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="550f1-954">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="550f1-954">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="550f1-955">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="550f1-955">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="550f1-956">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="550f1-956">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-957">Rdbms</span><span class="sxs-lookup"><span data-stu-id="550f1-957">Rdbms</span></span>
* <span data-ttu-id="550f1-958">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="550f1-958">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="550f1-959">RBAC:</span><span class="sxs-lookup"><span data-stu-id="550f1-959">Rbac</span></span>
* <span data-ttu-id="550f1-960">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-960">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="550f1-961">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="550f1-961">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="550f1-962">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-962">Storage</span></span>
* <span data-ttu-id="550f1-963">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="550f1-963">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="550f1-964">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="550f1-964">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="550f1-965">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="550f1-965">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="550f1-966">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="550f1-966">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-967">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-967">VM</span></span>
* <span data-ttu-id="550f1-968">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="550f1-968">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="550f1-969">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="550f1-969">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="550f1-970">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="550f1-970">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="550f1-971">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="550f1-971">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="550f1-972">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-972">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="550f1-973">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-973">Added `snapshot wait` command</span></span>
* <span data-ttu-id="550f1-974">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-974">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="550f1-975">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-975">November 6, 2018</span></span>

<span data-ttu-id="550f1-976">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="550f1-976">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="550f1-977">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-977">Core</span></span>
* <span data-ttu-id="550f1-978">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="550f1-978">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-979">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-979">ACR</span></span>
* <span data-ttu-id="550f1-980">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="550f1-980">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="550f1-981">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="550f1-981">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-982">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-982">ACS</span></span>
* <span data-ttu-id="550f1-983">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-983">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="550f1-984">Помощник</span><span class="sxs-lookup"><span data-stu-id="550f1-984">Advisor</span></span>
* <span data-ttu-id="550f1-985">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="550f1-985">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="550f1-986">AMS</span><span class="sxs-lookup"><span data-stu-id="550f1-986">AMS</span></span>
* <span data-ttu-id="550f1-987">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="550f1-987">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="550f1-988">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="550f1-988">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="550f1-989">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-989">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="550f1-990">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="550f1-990">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="550f1-991">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="550f1-991">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="550f1-992">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="550f1-992">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="550f1-993">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="550f1-993">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="550f1-994">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="550f1-994">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="550f1-995">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="550f1-995">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="550f1-996">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-996">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="550f1-997">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="550f1-997">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="550f1-998">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="550f1-998">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="550f1-999">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="550f1-999">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="550f1-1000">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="550f1-1000">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="550f1-1001">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1001">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="550f1-1002">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="550f1-1002">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="550f1-1003">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="550f1-1003">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1004">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-1004">AppService</span></span>
* <span data-ttu-id="550f1-1005">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="550f1-1005">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="550f1-1006">Настройка</span><span class="sxs-lookup"><span data-stu-id="550f1-1006">Configure</span></span>
* <span data-ttu-id="550f1-1007">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="550f1-1007">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1008">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1008">Container</span></span>
* <span data-ttu-id="550f1-1009">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="550f1-1009">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="550f1-1010">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="550f1-1010">EventHub</span></span>
* <span data-ttu-id="550f1-1011">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1011">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-1012">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-1012">Interactive</span></span>
* <span data-ttu-id="550f1-1013">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="550f1-1013">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-1014">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-1014">Monitor</span></span>
* <span data-ttu-id="550f1-1015">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1015">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1016">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1016">Network</span></span>
* <span data-ttu-id="550f1-1017">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1017">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="550f1-1018">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="550f1-1018">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="550f1-1019">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1019">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="550f1-1020">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-1020">Profile</span></span>
* <span data-ttu-id="550f1-1021">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1021">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-1022">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="550f1-1022">RDBMS</span></span>
* <span data-ttu-id="550f1-1023">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="550f1-1023">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-1024">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-1024">Resource</span></span>
* <span data-ttu-id="550f1-1025">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1025">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="550f1-1026">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-1026">Role</span></span>
* <span data-ttu-id="550f1-1027">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="550f1-1027">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="550f1-1028">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-1028">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="550f1-1029">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="550f1-1029">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1030">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1030">Storage</span></span>
* <span data-ttu-id="550f1-1031">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1031">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1032">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1032">VM</span></span>
* <span data-ttu-id="550f1-1033">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="550f1-1033">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="550f1-1034">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="550f1-1034">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="550f1-1035">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="550f1-1035">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="550f1-1036">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="550f1-1036">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="550f1-1037">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="550f1-1037">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="550f1-1038">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1038">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="550f1-1039">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1039">October 23, 2018</span></span>

<span data-ttu-id="550f1-1040">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="550f1-1040">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1041">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1041">Core</span></span>
* <span data-ttu-id="550f1-1042">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1042">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="550f1-1043">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1043">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1044">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1044">ACR</span></span>
* <span data-ttu-id="550f1-1045">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="550f1-1045">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="550f1-1046">CDN</span><span class="sxs-lookup"><span data-stu-id="550f1-1046">CDN</span></span>
* <span data-ttu-id="550f1-1047">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-1047">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="550f1-1048">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="550f1-1048">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1049">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1049">Container</span></span>
* <span data-ttu-id="550f1-1050">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="550f1-1050">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="550f1-1051">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="550f1-1051">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="550f1-1052">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1052">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="550f1-1053">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1053">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="550f1-1054">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="550f1-1054">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="550f1-1055">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="550f1-1055">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="550f1-1056">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1056">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="550f1-1057">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-1057">CosmosDB</span></span>
* <span data-ttu-id="550f1-1058">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1058">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-1059">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-1059">Interactive</span></span>
* <span data-ttu-id="550f1-1060">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1060">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="550f1-1061">IoT Central</span><span class="sxs-lookup"><span data-stu-id="550f1-1061">IoT Central</span></span>
* <span data-ttu-id="550f1-1062">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="550f1-1062">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="550f1-1063">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="550f1-1063">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-1064">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-1064">Monitor</span></span>
* <span data-ttu-id="550f1-1065">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="550f1-1065">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="550f1-1066">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1066">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="550f1-1067">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="550f1-1067">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="550f1-1068">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="550f1-1068">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="550f1-1069">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1069">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="550f1-1070">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="550f1-1070">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="550f1-1071">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="550f1-1071">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="550f1-1072">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="550f1-1072">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="550f1-1073">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="550f1-1073">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="550f1-1074">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1074">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1075">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1075">Network</span></span>
* <span data-ttu-id="550f1-1076">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="550f1-1076">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="550f1-1077">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="550f1-1077">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="550f1-1078">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="550f1-1078">ServiceBus</span></span>
* <span data-ttu-id="550f1-1079">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="550f1-1079">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-1080">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-1080">SQL</span></span>
* <span data-ttu-id="550f1-1081">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="550f1-1081">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1082">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1082">Storage</span></span>
* <span data-ttu-id="550f1-1083">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-1083">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="550f1-1084">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="550f1-1084">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1085">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1085">VM</span></span>
* <span data-ttu-id="550f1-1086">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="550f1-1086">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="550f1-1087">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="550f1-1087">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="550f1-1088">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="550f1-1088">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="550f1-1089">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1089">October 16, 2018</span></span>

<span data-ttu-id="550f1-1090">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="550f1-1090">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1091">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1091">VM</span></span>
* <span data-ttu-id="550f1-1092">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="550f1-1092">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="550f1-1093">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1093">October 9, 2018</span></span>

<span data-ttu-id="550f1-1094">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="550f1-1094">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1095">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1095">Core</span></span>
* <span data-ttu-id="550f1-1096">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="550f1-1096">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1097">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1097">ACR</span></span>
* <span data-ttu-id="550f1-1098">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="550f1-1098">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1099">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1099">ACS</span></span>
* <span data-ttu-id="550f1-1100">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="550f1-1100">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="550f1-1101">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="550f1-1101">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="550f1-1102">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1102">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="550f1-1103">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="550f1-1103">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1104">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1104">Container</span></span>
* <span data-ttu-id="550f1-1105">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="550f1-1105">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="550f1-1106">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="550f1-1106">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="550f1-1107">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="550f1-1107">Event Hub</span></span>
* <span data-ttu-id="550f1-1108">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1108">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="550f1-1109">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="550f1-1109">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="550f1-1110">расширения.</span><span class="sxs-lookup"><span data-stu-id="550f1-1110">Extensions</span></span>
* <span data-ttu-id="550f1-1111">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="550f1-1111">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="550f1-1112">HDInsight</span><span class="sxs-lookup"><span data-stu-id="550f1-1112">HDInsight</span></span>
* <span data-ttu-id="550f1-1113">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="550f1-1113">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-1114">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-1114">IoT</span></span>
* <span data-ttu-id="550f1-1115">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="550f1-1115">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="550f1-1116">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="550f1-1116">KeyVault</span></span>
* <span data-ttu-id="550f1-1117">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="550f1-1117">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1118">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1118">Network</span></span>
* <span data-ttu-id="550f1-1119">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-1119">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="550f1-1120">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="550f1-1120">See #6052</span></span>
* <span data-ttu-id="550f1-1121">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1121">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="550f1-1122">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="550f1-1122">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="550f1-1123">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1123">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="550f1-1124">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1124">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="550f1-1125">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1125">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="550f1-1126">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1126">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="550f1-1127">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-1127">Role</span></span>
* <span data-ttu-id="550f1-1128">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1128">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="550f1-1129">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1129">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="550f1-1130">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="550f1-1130">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="550f1-1131">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="550f1-1131">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="550f1-1132">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="550f1-1132">Service Bus</span></span>
* <span data-ttu-id="550f1-1133">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="550f1-1133">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1134">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1134">VM</span></span>
* <span data-ttu-id="550f1-1135">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1135">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="550f1-1136">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1136">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="550f1-1137">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1137">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="550f1-1138">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1138">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="550f1-1139">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="550f1-1139">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="550f1-1140">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="550f1-1140">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="550f1-1141">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1141">September 21, 2018</span></span>

<span data-ttu-id="550f1-1142">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="550f1-1142">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1143">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1143">ACR</span></span>
* <span data-ttu-id="550f1-1144">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="550f1-1144">Added ACR Task commands</span></span>
* <span data-ttu-id="550f1-1145">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="550f1-1145">Added quick run command</span></span>
* <span data-ttu-id="550f1-1146">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="550f1-1146">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="550f1-1147">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="550f1-1147">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="550f1-1148">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="550f1-1148">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="550f1-1149">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1149">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1150">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1150">ACS</span></span>
* <span data-ttu-id="550f1-1151">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="550f1-1151">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="550f1-1152">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="550f1-1152">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1153">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-1153">AppService</span></span>

* <span data-ttu-id="550f1-1154">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="550f1-1154">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="550f1-1155">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="550f1-1155">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="550f1-1156">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="550f1-1156">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="550f1-1157">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="550f1-1157">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-1158">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-1158">Batch</span></span>
* <span data-ttu-id="550f1-1159">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="550f1-1159">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="550f1-1160">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1160">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="550f1-1161">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1161">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="550f1-1162">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="550f1-1162">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="550f1-1163">Batch AI</span><span class="sxs-lookup"><span data-stu-id="550f1-1163">Batch AI</span></span> 
* <span data-ttu-id="550f1-1164">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1164">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="550f1-1165">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="550f1-1165">Cognitive Services</span></span>
* <span data-ttu-id="550f1-1166">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1166">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="550f1-1167">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1167">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="550f1-1168">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1168">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="550f1-1169">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1169">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="550f1-1170">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="550f1-1170">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="550f1-1171">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1171">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1172">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1172">Container</span></span>
* <span data-ttu-id="550f1-1173">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1173">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="550f1-1174">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="550f1-1174">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="550f1-1175">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="550f1-1175">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="550f1-1176">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1176">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="550f1-1177">Data Lake</span><span class="sxs-lookup"><span data-stu-id="550f1-1177">Datalake</span></span>
* <span data-ttu-id="550f1-1178">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="550f1-1178">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="550f1-1179">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="550f1-1179">Interactive Shell</span></span>
* <span data-ttu-id="550f1-1180">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-1180">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="550f1-1181">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1181">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-1182">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-1182">IoT</span></span>
* <span data-ttu-id="550f1-1183">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="550f1-1183">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="550f1-1184">Key Vault</span><span class="sxs-lookup"><span data-stu-id="550f1-1184">Key Vault</span></span>
* <span data-ttu-id="550f1-1185">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="550f1-1185">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1186">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1186">Network</span></span>
* <span data-ttu-id="550f1-1187">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1187">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="550f1-1188">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-1188">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="550f1-1189">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="550f1-1189">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="550f1-1190">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1190">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="550f1-1191">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1191">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="550f1-1192">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1192">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="550f1-1193">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="550f1-1193">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="550f1-1194">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1194">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="550f1-1195">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1195">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="550f1-1196">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1196">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="550f1-1197">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1197">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="550f1-1198">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1198">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="550f1-1199">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1199">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="550f1-1200">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="550f1-1200">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="550f1-1201">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1201">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="550f1-1202">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="550f1-1202">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="550f1-1203">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="550f1-1203">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="550f1-1204">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="550f1-1204">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-1205">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="550f1-1205">RDBMS</span></span>
* <span data-ttu-id="550f1-1206">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="550f1-1206">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="550f1-1207">резервирование.</span><span class="sxs-lookup"><span data-stu-id="550f1-1207">Reservation</span></span>
* <span data-ttu-id="550f1-1208">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1208">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="550f1-1209">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="550f1-1209">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="550f1-1210">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="550f1-1210">Manage App</span></span>
* <span data-ttu-id="550f1-1211">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="550f1-1211">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="550f1-1212">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="550f1-1212">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="550f1-1213">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-1213">Role</span></span>
* <span data-ttu-id="550f1-1214">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="550f1-1214">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="550f1-1215">SignalR</span><span class="sxs-lookup"><span data-stu-id="550f1-1215">SignalR</span></span>
* <span data-ttu-id="550f1-1216">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="550f1-1216">First release</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1217">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1217">Storage</span></span>
* <span data-ttu-id="550f1-1218">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="550f1-1218">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="550f1-1219">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="550f1-1219">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1220">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1220">VM</span></span>
* <span data-ttu-id="550f1-1221">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="550f1-1221">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="550f1-1222">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1222">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="550f1-1223">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1223">August 28, 2018</span></span>

<span data-ttu-id="550f1-1224">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="550f1-1224">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1225">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1225">Core</span></span>

* <span data-ttu-id="550f1-1226">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="550f1-1226">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="550f1-1227">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="550f1-1227">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1228">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1228">ACR</span></span>

* <span data-ttu-id="550f1-1229">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="550f1-1229">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="550f1-1230">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1230">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1231">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1231">ACS</span></span>

* <span data-ttu-id="550f1-1232">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1232">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="550f1-1233">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="550f1-1233">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1234">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-1234">AppService</span></span>

* <span data-ttu-id="550f1-1235">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="550f1-1235">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="550f1-1236">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="550f1-1236">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="550f1-1237">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="550f1-1237">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="550f1-1238">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="550f1-1238">Backup</span></span>

* <span data-ttu-id="550f1-1239">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="550f1-1239">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="550f1-1240">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="550f1-1240">Bot Service</span></span>

* <span data-ttu-id="550f1-1241">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="550f1-1241">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="550f1-1242">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="550f1-1242">Cognitive Services</span></span>

* <span data-ttu-id="550f1-1243">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="550f1-1243">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-1244">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-1244">IoT</span></span>

* <span data-ttu-id="550f1-1245">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1245">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-1246">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-1246">Monitor</span></span>

* <span data-ttu-id="550f1-1247">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="550f1-1247">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="550f1-1248">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="550f1-1248">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1249">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1249">Network</span></span>

* <span data-ttu-id="550f1-1250">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="550f1-1250">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-1251">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-1251">Resource</span></span>

* <span data-ttu-id="550f1-1252">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="550f1-1252">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1253">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1253">Storage</span></span>

* <span data-ttu-id="550f1-1254">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="550f1-1254">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1255">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1255">VM</span></span>

* <span data-ttu-id="550f1-1256">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="550f1-1256">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="550f1-1257">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1257">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="550f1-1258">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1258">Auguest 14, 2018</span></span>

<span data-ttu-id="550f1-1259">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="550f1-1259">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1260">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1260">Core</span></span>

* <span data-ttu-id="550f1-1261">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1261">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="550f1-1262">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="550f1-1262">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="550f1-1263">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="550f1-1263">Telemetry</span></span>

* <span data-ttu-id="550f1-1264">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="550f1-1264">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1265">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1265">ACR</span></span>

* <span data-ttu-id="550f1-1266">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1266">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="550f1-1267">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1267">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1268">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1268">ACS</span></span>

* <span data-ttu-id="550f1-1269">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="550f1-1269">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="550f1-1270">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="550f1-1270">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="550f1-1271">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="550f1-1271">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="550f1-1272">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="550f1-1272">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="550f1-1273">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="550f1-1273">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="550f1-1274">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-1274">AppService</span></span>

* <span data-ttu-id="550f1-1275">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1275">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="550f1-1276">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="550f1-1276">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="550f1-1277">Batch AI</span><span class="sxs-lookup"><span data-stu-id="550f1-1277">BatchAI</span></span>

* <span data-ttu-id="550f1-1278">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="550f1-1278">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="550f1-1279">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1279">Container</span></span>

* <span data-ttu-id="550f1-1280">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="550f1-1280">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="550f1-1281">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-1281">IoT</span></span>

* <span data-ttu-id="550f1-1282">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="550f1-1282">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="550f1-1283">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1283">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="550f1-1284">IoT Central</span><span class="sxs-lookup"><span data-stu-id="550f1-1284">Iot Central</span></span>

* <span data-ttu-id="550f1-1285">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="550f1-1285">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="550f1-1286">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="550f1-1286">KeyVault</span></span>


* <span data-ttu-id="550f1-1287">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="550f1-1287">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="550f1-1288">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="550f1-1288">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="550f1-1289">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="550f1-1289">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="550f1-1290">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="550f1-1290">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="550f1-1291">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="550f1-1291">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="550f1-1292">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="550f1-1292">Relay</span></span>

* <span data-ttu-id="550f1-1293">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="550f1-1293">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-1294">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-1294">Sql</span></span>

* <span data-ttu-id="550f1-1295">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1295">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1296">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1296">Storage</span></span>

* <span data-ttu-id="550f1-1297">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="550f1-1297">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="550f1-1298">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="550f1-1298">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="550f1-1299">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="550f1-1299">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="550f1-1300">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="550f1-1300">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="550f1-1301">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="550f1-1301">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1302">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1302">VM</span></span>

* <span data-ttu-id="550f1-1303">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="550f1-1303">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="550f1-1304">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1304">July 31, 2018</span></span>

<span data-ttu-id="550f1-1305">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="550f1-1305">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1306">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1306">ACR</span></span>

* <span data-ttu-id="550f1-1307">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1307">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="550f1-1308">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1308">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1309">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1309">ACS</span></span>

* <span data-ttu-id="550f1-1310">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="550f1-1310">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-1311">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-1311">Batch</span></span>

* <span data-ttu-id="550f1-1312">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="550f1-1312">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1313">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1313">Container</span></span>

* <span data-ttu-id="550f1-1314">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1314">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1315">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1315">Network</span></span>

* <span data-ttu-id="550f1-1316">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="550f1-1316">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="550f1-1317">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-1317">Resource</span></span>

* <span data-ttu-id="550f1-1318">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1318">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="550f1-1319">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="550f1-1319">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="550f1-1320">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-1320">Role</span></span>

* <span data-ttu-id="550f1-1321">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="550f1-1321">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="550f1-1322">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="550f1-1322">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="550f1-1323">Поиск</span><span class="sxs-lookup"><span data-stu-id="550f1-1323">Search</span></span>

* <span data-ttu-id="550f1-1324">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="550f1-1324">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="550f1-1325">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="550f1-1325">Service Bus</span></span>

* <span data-ttu-id="550f1-1326">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="550f1-1326">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="550f1-1327">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="550f1-1327">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="550f1-1328">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="550f1-1328">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="550f1-1329">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1329">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1330">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1330">Storage</span></span>

* <span data-ttu-id="550f1-1331">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="550f1-1331">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="550f1-1332">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="550f1-1332">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1333">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1333">VM</span></span>

* <span data-ttu-id="550f1-1334">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="550f1-1334">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="550f1-1335">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1335">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="550f1-1336">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="550f1-1336">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="550f1-1337">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="550f1-1337">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="550f1-1338">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1338">July 18, 2018</span></span>

<span data-ttu-id="550f1-1339">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="550f1-1339">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1340">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1340">Core</span></span>

* <span data-ttu-id="550f1-1341">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="550f1-1341">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="550f1-1342">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="550f1-1342">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="550f1-1343">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="550f1-1343">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1344">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1344">ACR</span></span>

* <span data-ttu-id="550f1-1345">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="550f1-1345">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="550f1-1346">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1346">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="550f1-1347">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="550f1-1347">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="550f1-1348">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="550f1-1348">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1349">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1349">ACS</span></span>

* <span data-ttu-id="550f1-1350">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="550f1-1350">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1351">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-1351">AppService</span></span>

* <span data-ttu-id="550f1-1352">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="550f1-1352">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-1353">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-1353">Batch</span></span>

* <span data-ttu-id="550f1-1354">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="550f1-1354">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="550f1-1355">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="550f1-1355">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="550f1-1356">Batch AI</span><span class="sxs-lookup"><span data-stu-id="550f1-1356">Batch AI</span></span>

* <span data-ttu-id="550f1-1357">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1357">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1358">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1358">Container</span></span>

* <span data-ttu-id="550f1-1359">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="550f1-1359">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="550f1-1360">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="550f1-1360">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1361">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1361">Network</span></span>

* <span data-ttu-id="550f1-1362">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1362">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="550f1-1363">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1363">Added `network nic wait`</span></span>
* <span data-ttu-id="550f1-1364">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="550f1-1364">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="550f1-1365">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="550f1-1365">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="550f1-1366">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-1366">Resource</span></span>

* <span data-ttu-id="550f1-1367">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1367">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="550f1-1368">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1368">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="550f1-1369">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1369">Added `deployment wait` command</span></span>
* <span data-ttu-id="550f1-1370">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="550f1-1370">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-1371">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-1371">SQL</span></span>

* <span data-ttu-id="550f1-1372">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1372">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="550f1-1373">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1373">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="550f1-1374">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1374">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1375">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1375">Storage</span></span>

* <span data-ttu-id="550f1-1376">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1376">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1377">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1377">VM</span></span>

* <span data-ttu-id="550f1-1378">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-1378">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="550f1-1379">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1379">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="550f1-1380">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1380">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="550f1-1381">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1381">July 3, 2018</span></span>

<span data-ttu-id="550f1-1382">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="550f1-1382">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="550f1-1383">AKS</span><span class="sxs-lookup"><span data-stu-id="550f1-1383">AKS</span></span>

* <span data-ttu-id="550f1-1384">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1384">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="550f1-1385">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1385">July 3, 2018</span></span>

<span data-ttu-id="550f1-1386">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="550f1-1386">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1387">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1387">Core</span></span>

* <span data-ttu-id="550f1-1388">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="550f1-1388">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1389">ACR</span></span>

* <span data-ttu-id="550f1-1390">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="550f1-1390">Added polling build status</span></span>
* <span data-ttu-id="550f1-1391">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="550f1-1391">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="550f1-1392">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1392">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1393">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1393">ACS</span></span>

* <span data-ttu-id="550f1-1394">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-1394">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="550f1-1395">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-1395">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="550f1-1396">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1396">Updated options for `aks browse` command.</span></span> <span data-ttu-id="550f1-1397">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1397">Added `--listen-port` support</span></span>
* <span data-ttu-id="550f1-1398">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1398">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="550f1-1399">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="550f1-1399">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="550f1-1400">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1400">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1401">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-1401">AppService</span></span>

* <span data-ttu-id="550f1-1402">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1402">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="550f1-1403">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="550f1-1403">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="550f1-1404">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="550f1-1404">Backup</span></span>

* <span data-ttu-id="550f1-1405">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="550f1-1405">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="550f1-1406">Batch AI</span><span class="sxs-lookup"><span data-stu-id="550f1-1406">BatchAI</span></span>

* <span data-ttu-id="550f1-1407">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1407">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="550f1-1408">Облако</span><span class="sxs-lookup"><span data-stu-id="550f1-1408">Cloud</span></span>

* <span data-ttu-id="550f1-1409">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1409">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1410">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1410">Container</span></span>

* <span data-ttu-id="550f1-1411">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="550f1-1411">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="550f1-1412">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1412">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="550f1-1413">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="550f1-1413">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="550f1-1414">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="550f1-1414">Extension</span></span>

* <span data-ttu-id="550f1-1415">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="550f1-1415">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1416">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1416">Network</span></span>

* <span data-ttu-id="550f1-1417">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="550f1-1417">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-1418">Rdbms</span><span class="sxs-lookup"><span data-stu-id="550f1-1418">Rdbms</span></span>

* <span data-ttu-id="550f1-1419">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1419">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-1420">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-1420">Resource</span></span>

* <span data-ttu-id="550f1-1421">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1421">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1422">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1422">VM</span></span>

* <span data-ttu-id="550f1-1423">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="550f1-1423">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="550f1-1424">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1424">June 25, 2018</span></span>

<span data-ttu-id="550f1-1425">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="550f1-1425">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="550f1-1426">CLI</span><span class="sxs-lookup"><span data-stu-id="550f1-1426">CLI</span></span>

* <span data-ttu-id="550f1-1427">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="550f1-1427">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="550f1-1428">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1428">June 19, 2018</span></span>

<span data-ttu-id="550f1-1429">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="550f1-1429">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1430">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1430">Core</span></span>

* <span data-ttu-id="550f1-1431">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-1431">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1432">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1432">ACR</span></span>

* <span data-ttu-id="550f1-1433">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1433">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="550f1-1434">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="550f1-1434">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1435">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1435">ACS</span></span>

* <span data-ttu-id="550f1-1436">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1436">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="550f1-1437">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1437">Added `--update` support</span></span>
* <span data-ttu-id="550f1-1438">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1438">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="550f1-1439">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1439">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="550f1-1440">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1440">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="550f1-1441">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1441">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="550f1-1442">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1442">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="550f1-1443">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1443">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1444">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-1444">AppService</span></span>

* <span data-ttu-id="550f1-1445">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="550f1-1445">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="550f1-1446">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1446">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-1447">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-1447">Batch</span></span>

* <span data-ttu-id="550f1-1448">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1448">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="550f1-1449">Batch AI</span><span class="sxs-lookup"><span data-stu-id="550f1-1449">Batch AI</span></span>

* <span data-ttu-id="550f1-1450">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="550f1-1450">Added support for workspaces.</span></span> <span data-ttu-id="550f1-1451">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1451">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="550f1-1452">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1452">Added support for experiments.</span></span> <span data-ttu-id="550f1-1453">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="550f1-1453">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="550f1-1454">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="550f1-1454">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="550f1-1455">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1455">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="550f1-1456">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1456">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="550f1-1457">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1457">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="550f1-1458">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="550f1-1458">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="550f1-1459">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1459">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="550f1-1460">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1460">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="550f1-1461">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1461">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="550f1-1462">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1462">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="550f1-1463">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1463">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="550f1-1464">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1464">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="550f1-1465">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="550f1-1465">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="550f1-1466">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1466">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="550f1-1467">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="550f1-1467">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="550f1-1468">[`--config`, `-c`] переименовано в [`--config-file`, `-f`];</span><span class="sxs-lookup"><span data-stu-id="550f1-1468">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="550f1-1469">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="550f1-1469">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="550f1-1470">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`];</span><span class="sxs-lookup"><span data-stu-id="550f1-1470">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="550f1-1471">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="550f1-1471">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="550f1-1472">Maps</span><span class="sxs-lookup"><span data-stu-id="550f1-1472">Maps</span></span>

* <span data-ttu-id="550f1-1473">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1473">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1474">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1474">Network</span></span>

* <span data-ttu-id="550f1-1475">Добавлена поддержка `https` для `network lb probe create`. [#6571](https://github.com/Azure/azure-cli/issues/6571).</span><span class="sxs-lookup"><span data-stu-id="550f1-1475">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="550f1-1476">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="550f1-1476">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="550f1-1477">#6502</span><span class="sxs-lookup"><span data-stu-id="550f1-1477">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="550f1-1478">Резервирование</span><span class="sxs-lookup"><span data-stu-id="550f1-1478">Reservations</span></span>

* <span data-ttu-id="550f1-1479">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1479">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="550f1-1480">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1480">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="550f1-1481">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1481">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="550f1-1482">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1482">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="550f1-1483">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1483">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="550f1-1484">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1484">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="550f1-1485">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-1485">Role</span></span>

* <span data-ttu-id="550f1-1486">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="550f1-1486">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-1487">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-1487">SQL</span></span>

* <span data-ttu-id="550f1-1488">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1488">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1489">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1489">Storage</span></span>

* <span data-ttu-id="550f1-1490">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="550f1-1490">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1491">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1491">VM</span></span>

* <span data-ttu-id="550f1-1492">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1492">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="550f1-1493">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1493">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="550f1-1494">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="550f1-1494">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="550f1-1495">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1495">June 13, 2018</span></span>

<span data-ttu-id="550f1-1496">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="550f1-1496">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1497">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1497">Core</span></span>

* <span data-ttu-id="550f1-1498">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="550f1-1498">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="550f1-1499">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1499">June 13, 2018</span></span>

<span data-ttu-id="550f1-1500">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="550f1-1500">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="550f1-1501">AKS</span><span class="sxs-lookup"><span data-stu-id="550f1-1501">AKS</span></span>

* <span data-ttu-id="550f1-1502">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="550f1-1502">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="550f1-1503">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="550f1-1503">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="550f1-1504">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="550f1-1504">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="550f1-1505">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="550f1-1505">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="550f1-1506">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="550f1-1506">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1507">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-1507">AppService</span></span>

* <span data-ttu-id="550f1-1508">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="550f1-1508">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="550f1-1509">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1509">June 5, 2018</span></span>

<span data-ttu-id="550f1-1510">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="550f1-1510">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-1511">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-1511">Interactive</span></span>

* <span data-ttu-id="550f1-1512">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="550f1-1512">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="550f1-1513">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1513">June 5, 2018</span></span>

<span data-ttu-id="550f1-1514">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="550f1-1514">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1515">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1515">Core</span></span>

* <span data-ttu-id="550f1-1516">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="550f1-1516">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="550f1-1517">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="550f1-1517">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1518">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1518">ACR</span></span>

* <span data-ttu-id="550f1-1519">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="550f1-1519">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="550f1-1520">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1520">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="550f1-1521">AKS</span><span class="sxs-lookup"><span data-stu-id="550f1-1521">AKS</span></span>

* <span data-ttu-id="550f1-1522">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="550f1-1522">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-1523">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-1523">Batch</span></span>

* <span data-ttu-id="550f1-1524">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="550f1-1524">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-1525">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-1525">IOT</span></span>

* <span data-ttu-id="550f1-1526">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="550f1-1526">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1527">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1527">Network</span></span>

* <span data-ttu-id="550f1-1528">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1528">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="550f1-1529">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="550f1-1529">Policy Insights</span></span>

* <span data-ttu-id="550f1-1530">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="550f1-1530">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="550f1-1531">ARM</span><span class="sxs-lookup"><span data-stu-id="550f1-1531">ARM</span></span>

* <span data-ttu-id="550f1-1532">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1532">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-1533">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-1533">SQL</span></span>

* <span data-ttu-id="550f1-1534">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="550f1-1534">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="550f1-1535">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="550f1-1535">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="550f1-1536">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1536">Storage</span></span>

* <span data-ttu-id="550f1-1537">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1537">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1538">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1538">VM</span></span>

* <span data-ttu-id="550f1-1539">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1539">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="550f1-1540">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1540">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="550f1-1541">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1541">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="550f1-1542">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1542">May 22, 2018</span></span>

<span data-ttu-id="550f1-1543">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="550f1-1543">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1544">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1544">Core</span></span>

* <span data-ttu-id="550f1-1545">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1545">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1546">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1546">ACS</span></span>

* <span data-ttu-id="550f1-1547">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1547">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="550f1-1548">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="550f1-1548">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1549">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-1549">AppService</span></span>

* <span data-ttu-id="550f1-1550">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="550f1-1550">Improved generic update commands</span></span>
* <span data-ttu-id="550f1-1551">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1551">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1552">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1552">Container</span></span>

* <span data-ttu-id="550f1-1553">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="550f1-1553">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="550f1-1554">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1554">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="550f1-1555">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="550f1-1555">Extension</span></span>

* <span data-ttu-id="550f1-1556">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="550f1-1556">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-1557">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-1557">Interactive</span></span>

* <span data-ttu-id="550f1-1558">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="550f1-1558">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="550f1-1559">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1559">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="550f1-1560">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="550f1-1560">KeyVault</span></span>

* <span data-ttu-id="550f1-1561">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="550f1-1561">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1562">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1562">Network</span></span>

* <span data-ttu-id="550f1-1563">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="550f1-1563">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="550f1-1564">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="550f1-1564">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-1565">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-1565">SQL</span></span>

* <span data-ttu-id="550f1-1566">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="550f1-1566">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="550f1-1567">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1567">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="550f1-1568">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1568">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="550f1-1569">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="550f1-1569">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="550f1-1570">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="550f1-1570">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="550f1-1571">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1571">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="550f1-1572">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1572">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="550f1-1573">`edition`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1573">`edition`.</span></span> <span data-ttu-id="550f1-1574">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1574">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="550f1-1575">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1575">`elasticPoolName`.</span></span> <span data-ttu-id="550f1-1576">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1576">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="550f1-1577">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="550f1-1577">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="550f1-1578">`edition`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1578">`edition`.</span></span> <span data-ttu-id="550f1-1579">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1579">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="550f1-1580">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1580">`dtu`.</span></span> <span data-ttu-id="550f1-1581">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1581">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="550f1-1582">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1582">`databaseDtuMin`.</span></span> <span data-ttu-id="550f1-1583">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1583">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="550f1-1584">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1584">`databaseDtuMax`.</span></span> <span data-ttu-id="550f1-1585">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1585">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="550f1-1586">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1586">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="550f1-1587">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1587">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1588">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1588">Storage</span></span>

* <span data-ttu-id="550f1-1589">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1589">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="550f1-1590">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1590">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1591">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1591">VM</span></span>

* <span data-ttu-id="550f1-1592">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1592">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="550f1-1593">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1593">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="550f1-1594">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1594">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="550f1-1595">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1595">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="550f1-1596">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1596">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="550f1-1597">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1597">May 7, 2018</span></span>

<span data-ttu-id="550f1-1598">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="550f1-1598">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1599">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1599">Core</span></span>

* <span data-ttu-id="550f1-1600">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="550f1-1600">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="550f1-1601">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1601">Added limited support for positional arguments</span></span>
* <span data-ttu-id="550f1-1602">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1602">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="550f1-1603">#5591</span><span class="sxs-lookup"><span data-stu-id="550f1-1603">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="550f1-1604">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1604">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="550f1-1605">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="550f1-1605">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="550f1-1606">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="550f1-1606">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="550f1-1607">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1607">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="550f1-1608">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="550f1-1608">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1609">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1609">ACR</span></span>

* <span data-ttu-id="550f1-1610">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="550f1-1610">Added ACR Build commands</span></span>
* <span data-ttu-id="550f1-1611">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="550f1-1611">Improved resource not found error messages</span></span>
* <span data-ttu-id="550f1-1612">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="550f1-1612">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="550f1-1613">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="550f1-1613">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="550f1-1614">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="550f1-1614">Improved repository commands error messages</span></span>
* <span data-ttu-id="550f1-1615">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="550f1-1615">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1616">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1616">ACS</span></span>

* <span data-ttu-id="550f1-1617">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-1617">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="550f1-1618">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="550f1-1618">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="550f1-1619">AMS</span><span class="sxs-lookup"><span data-stu-id="550f1-1619">AMS</span></span>

* <span data-ttu-id="550f1-1620">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="550f1-1620">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1621">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-1621">Appservice</span></span>

* <span data-ttu-id="550f1-1622">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="550f1-1622">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="550f1-1623">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1623">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="550f1-1624">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="550f1-1624">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="550f1-1625">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1625">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="550f1-1626">Batch AI</span><span class="sxs-lookup"><span data-stu-id="550f1-1626">Batch AI</span></span>

* <span data-ttu-id="550f1-1627">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="550f1-1627">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="550f1-1628">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="550f1-1628">Cognitive Services</span></span>

* <span data-ttu-id="550f1-1629">Исправлена опечатка в примере для `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603).</span><span class="sxs-lookup"><span data-stu-id="550f1-1629">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="550f1-1630">Потребление</span><span class="sxs-lookup"><span data-stu-id="550f1-1630">Consumption</span></span>

* <span data-ttu-id="550f1-1631">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="550f1-1631">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1632">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1632">Container</span></span>

* <span data-ttu-id="550f1-1633">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="550f1-1633">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="550f1-1634">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-1634">Cosmos DB</span></span>

* <span data-ttu-id="550f1-1635">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-1635">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="550f1-1636">DMS</span><span class="sxs-lookup"><span data-stu-id="550f1-1636">DMS</span></span>

* <span data-ttu-id="550f1-1637">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="550f1-1637">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="550f1-1638">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="550f1-1638">Extension</span></span>

* <span data-ttu-id="550f1-1639">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="550f1-1639">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-1640">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-1640">Interactive</span></span>

* <span data-ttu-id="550f1-1641">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="550f1-1641">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="550f1-1642">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="550f1-1642">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="550f1-1643">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1643">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="550f1-1644">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-1644">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="550f1-1645">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="550f1-1645">Lab</span></span>

* <span data-ttu-id="550f1-1646">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="550f1-1646">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1647">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1647">Network</span></span>

* <span data-ttu-id="550f1-1648">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="550f1-1648">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="550f1-1649">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-1649">Profile</span></span>

* <span data-ttu-id="550f1-1650">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1650">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="550f1-1651">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="550f1-1651">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="550f1-1652">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1652">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="550f1-1653">Redis</span><span class="sxs-lookup"><span data-stu-id="550f1-1653">Redis</span></span>

* <span data-ttu-id="550f1-1654">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1654">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="550f1-1655">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="550f1-1655">Deprecated `redis list-all`.</span></span> <span data-ttu-id="550f1-1656">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1656">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="550f1-1657">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1657">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="550f1-1658">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-1658">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="550f1-1659">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-1659">Role</span></span>

* <span data-ttu-id="550f1-1660">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="550f1-1660">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1661">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1661">Storage</span></span>

* <span data-ttu-id="550f1-1662">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="550f1-1662">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="550f1-1663">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="550f1-1663">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="550f1-1664">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="550f1-1664">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="550f1-1665">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="550f1-1665">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="550f1-1666">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="550f1-1666">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1667">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1667">VM</span></span>

* <span data-ttu-id="550f1-1668">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="550f1-1668">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="550f1-1669">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="550f1-1669">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="550f1-1670">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="550f1-1670">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="550f1-1671">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1671">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="550f1-1672">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="550f1-1672">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="550f1-1673">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="550f1-1673">Added write accelerator support</span></span>
* <span data-ttu-id="550f1-1674">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1674">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="550f1-1675">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="550f1-1675">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="550f1-1676">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="550f1-1676">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="550f1-1677">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1677">April 10, 2018</span></span>

<span data-ttu-id="550f1-1678">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="550f1-1678">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1679">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1679">ACR</span></span>

* <span data-ttu-id="550f1-1680">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="550f1-1680">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1681">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1681">ACS</span></span>

* <span data-ttu-id="550f1-1682">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="550f1-1682">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1683">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-1683">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="550f1-1685">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="550f1-1685">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="550f1-1686">Batch AI</span><span class="sxs-lookup"><span data-stu-id="550f1-1686">BatchAI</span></span>

* <span data-ttu-id="550f1-1687">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="550f1-1687">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="550f1-1688">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="550f1-1688">Job level mounting</span></span>
  - <span data-ttu-id="550f1-1689">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1689">Environment variables with secret values</span></span>
  - <span data-ttu-id="550f1-1690">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="550f1-1690">Performance counters settings</span></span>
  - <span data-ttu-id="550f1-1691">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="550f1-1691">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="550f1-1692">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1692">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="550f1-1693">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="550f1-1693">Usage and limits reporting</span></span>
  - <span data-ttu-id="550f1-1694">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1694">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="550f1-1695">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1695">Support for custom images</span></span>
  - <span data-ttu-id="550f1-1696">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="550f1-1696">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="550f1-1697">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="550f1-1697">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="550f1-1698">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1698">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="550f1-1699">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="550f1-1699">National clouds are supported</span></span>
* <span data-ttu-id="550f1-1700">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="550f1-1700">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="550f1-1701">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="550f1-1701">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="550f1-1702">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="550f1-1702">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="550f1-1703">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="550f1-1703">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="550f1-1704">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="550f1-1704">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="550f1-1705">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="550f1-1705">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="550f1-1706">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1706">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="550f1-1707">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="550f1-1707">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="550f1-1708">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="550f1-1708">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="550f1-1709">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1709">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="550f1-1710">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="550f1-1710">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="550f1-1711">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1711">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="550f1-1712">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1712">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="550f1-1713">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="550f1-1713">Billing</span></span>

* <span data-ttu-id="550f1-1714">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="550f1-1714">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="550f1-1715">Потребление</span><span class="sxs-lookup"><span data-stu-id="550f1-1715">Consumption</span></span>

* <span data-ttu-id="550f1-1716">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1716">Added `marketplace` commands</span></span>
* <span data-ttu-id="550f1-1717">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1717">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="550f1-1718">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1718">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="550f1-1719">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1719">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="550f1-1720">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1720">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="550f1-1721">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1721">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1722">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1722">Container</span></span>

* <span data-ttu-id="550f1-1723">Добавлены параметры подключения тома репозитория git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1723">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="550f1-1724">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="550f1-1724">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="550f1-1725">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="550f1-1725">Extension</span></span>

* <span data-ttu-id="550f1-1726">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1726">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-1727">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-1727">Interactive</span></span>

* <span data-ttu-id="550f1-1728">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="550f1-1728">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="550f1-1729">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-1729">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="550f1-1730">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1730">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1731">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1731">Network</span></span>

* <span data-ttu-id="550f1-1732">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1732">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="550f1-1733">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1733">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="550f1-1734">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="550f1-1734">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="550f1-1735">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="550f1-1735">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="550f1-1736">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="550f1-1736">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="550f1-1737">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1737">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="550f1-1738">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1738">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="550f1-1739">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="550f1-1739">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-1740">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-1740">Profile</span></span>

* <span data-ttu-id="550f1-1741">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1741">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="550f1-1742">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi`  &  `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1742">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-1743">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="550f1-1743">RDBMS</span></span>

* <span data-ttu-id="550f1-1744">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1744">Added `georestore` command</span></span>
* <span data-ttu-id="550f1-1745">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="550f1-1745">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-1746">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-1746">Resource</span></span>

* <span data-ttu-id="550f1-1747">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1747">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="550f1-1748">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1748">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-1749">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-1749">SQL</span></span>

* <span data-ttu-id="550f1-1750">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1750">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1751">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1751">Storage</span></span>

* <span data-ttu-id="550f1-1752">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="550f1-1752">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1753">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1753">VM</span></span>

* <span data-ttu-id="550f1-1754">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="550f1-1754">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="550f1-1755">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="550f1-1755">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="550f1-1757">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1757">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="550f1-1758">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="550f1-1758">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="550f1-1759">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="550f1-1759">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="550f1-1760">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="550f1-1760">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="550f1-1761">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1761">March 27, 2018</span></span>

<span data-ttu-id="550f1-1762">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="550f1-1762">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1763">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1763">Core</span></span>

* <span data-ttu-id="550f1-1764">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="550f1-1764">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1765">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1765">ACS</span></span>

* <span data-ttu-id="550f1-1766">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="550f1-1766">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1767">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-1767">Appservice</span></span>

* <span data-ttu-id="550f1-1768">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1768">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="550f1-1769">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1769">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="550f1-1770">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="550f1-1770">Backup</span></span>

* <span data-ttu-id="550f1-1771">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1771">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="550f1-1772">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="550f1-1772">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="550f1-1773">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="550f1-1773">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="550f1-1774">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1774">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1775">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1775">Container</span></span>

* <span data-ttu-id="550f1-1776">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1776">Added `container exec` command.</span></span> <span data-ttu-id="550f1-1777">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1777">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="550f1-1778">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1778">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="550f1-1779">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="550f1-1779">Extension</span></span>

* <span data-ttu-id="550f1-1780">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="550f1-1780">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="550f1-1781">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1781">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="550f1-1782">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-1782">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-1783">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-1783">Interactive</span></span>

* <span data-ttu-id="550f1-1784">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-1784">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="550f1-1785">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1785">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="550f1-1786">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-1786">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="550f1-1787">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="550f1-1787">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="550f1-1788">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="550f1-1788">Lab</span></span>

* <span data-ttu-id="550f1-1789">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1789">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-1790">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-1790">Monitor</span></span>

* <span data-ttu-id="550f1-1791">Добавлена поддержка `--top`, `--orderby` и `--namespace` для `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="550f1-1791">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="550f1-1792">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="550f1-1792">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="550f1-1793">Добавлена поддержка `--namespace` для `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785).</span><span class="sxs-lookup"><span data-stu-id="550f1-1793">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1794">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1794">Network</span></span>

* <span data-ttu-id="550f1-1795">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="550f1-1795">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-1796">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-1796">Profile</span></span>

* <span data-ttu-id="550f1-1797">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1797">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-1798">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="550f1-1798">RDBMS</span></span>

* <span data-ttu-id="550f1-1799">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="550f1-1799">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-1800">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-1800">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="550f1-1802">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-1802">Role</span></span>

* <span data-ttu-id="550f1-1803">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1803">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="550f1-1804">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="550f1-1804">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="550f1-1805">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="550f1-1805">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="550f1-1806">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1806">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="550f1-1807">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1807">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1808">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1808">Storage</span></span>

* <span data-ttu-id="550f1-1809">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="550f1-1809">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="550f1-1810">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="550f1-1810">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1811">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1811">VM</span></span>

* <span data-ttu-id="550f1-1812">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1812">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="550f1-1813">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1813">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="550f1-1814">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="550f1-1814">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="550f1-1815">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] `vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="550f1-1815">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="550f1-1816">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1816">March 13, 2018</span></span>

<span data-ttu-id="550f1-1817">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="550f1-1817">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-1818">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-1818">ACR</span></span>

* <span data-ttu-id="550f1-1819">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1819">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="550f1-1820">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="550f1-1820">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="550f1-1821">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="550f1-1821">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1822">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1822">ACS</span></span>

* <span data-ttu-id="550f1-1823">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="550f1-1823">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="550f1-1824">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1824">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="550f1-1825">Помощник</span><span class="sxs-lookup"><span data-stu-id="550f1-1825">Advisor</span></span>

* <span data-ttu-id="550f1-1826">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1826">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="550f1-1827">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1827">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="550f1-1828">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1828">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="550f1-1829">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1829">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="550f1-1830">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1830">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1831">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-1831">Appservice</span></span>

* <span data-ttu-id="550f1-1832">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="550f1-1832">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="550f1-1833">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1833">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="550f1-1834">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="550f1-1834">Eventhubs</span></span>

* <span data-ttu-id="550f1-1835">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="550f1-1835">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="550f1-1836">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="550f1-1836">Extension</span></span>

* <span data-ttu-id="550f1-1837">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="550f1-1837">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-1838">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-1838">Interactive</span></span>

* <span data-ttu-id="550f1-1839">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="550f1-1839">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="550f1-1840">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="550f1-1840">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="550f1-1841">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="550f1-1841">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="550f1-1842">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="550f1-1842">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-1843">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-1843">Monitor</span></span>

* <span data-ttu-id="550f1-1844">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="550f1-1844">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="550f1-1845">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1845">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="550f1-1846">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1846">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="550f1-1847">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1847">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1848">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1848">Network</span></span>

* <span data-ttu-id="550f1-1849">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1849">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="550f1-1850">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="550f1-1850">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="550f1-1851">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1851">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="550f1-1852">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1852">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-1853">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-1853">Profile</span></span>

* <span data-ttu-id="550f1-1854">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="550f1-1854">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="550f1-1855">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1855">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-1856">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="550f1-1856">RDBMS</span></span>

* <span data-ttu-id="550f1-1857">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="550f1-1857">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="550f1-1858">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="550f1-1858">Service Bus</span></span>

* <span data-ttu-id="550f1-1859">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="550f1-1859">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1860">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1860">Storage</span></span>

* <span data-ttu-id="550f1-1861">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="550f1-1861">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="550f1-1862">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="550f1-1862">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1863">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1863">VM</span></span>

* <span data-ttu-id="550f1-1864">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="550f1-1864">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="550f1-1865">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="550f1-1865">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="550f1-1866">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1866">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="550f1-1867">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="550f1-1867">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="550f1-1868">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="550f1-1868">February 27, 2018</span></span>

<span data-ttu-id="550f1-1869">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="550f1-1869">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1870">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1870">Core</span></span>

* <span data-ttu-id="550f1-1871">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="550f1-1871">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="550f1-1872">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="550f1-1872">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="550f1-1873">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1873">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1874">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1874">ACS</span></span>

* <span data-ttu-id="550f1-1875">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-1875">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="550f1-1876">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="550f1-1876">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="550f1-1877">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1877">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="550f1-1878">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1878">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1879">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-1879">Appservice</span></span>

* <span data-ttu-id="550f1-1880">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="550f1-1880">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="550f1-1881">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="550f1-1881">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="550f1-1882">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="550f1-1882">Cognitive Services</span></span>

* <span data-ttu-id="550f1-1883">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="550f1-1883">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="550f1-1884">Потребление</span><span class="sxs-lookup"><span data-stu-id="550f1-1884">Consumption</span></span>

* <span data-ttu-id="550f1-1885">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="550f1-1885">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="550f1-1886">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="550f1-1886">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1887">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1887">Container</span></span>

* <span data-ttu-id="550f1-1888">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="550f1-1888">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1889">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1889">Network</span></span>

* <span data-ttu-id="550f1-1890">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1890">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-1891">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-1891">Resource</span></span>

* <span data-ttu-id="550f1-1892">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="550f1-1892">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="550f1-1893">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-1893">Role</span></span>

* <span data-ttu-id="550f1-1894">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-1894">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-1895">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-1895">SQL</span></span>

* <span data-ttu-id="550f1-1896">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="550f1-1896">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1897">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1897">Storage</span></span>

* <span data-ttu-id="550f1-1898">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1898">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1899">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1899">VM</span></span>

* <span data-ttu-id="550f1-1900">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="550f1-1900">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="550f1-1901">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1901">February 13, 2018</span></span>

<span data-ttu-id="550f1-1902">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="550f1-1902">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1903">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1903">Core</span></span>

* <span data-ttu-id="550f1-1904">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="550f1-1904">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1905">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1905">ACS</span></span>

* <span data-ttu-id="550f1-1906">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="550f1-1906">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="550f1-1907">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1907">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="550f1-1908">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="550f1-1908">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="550f1-1909">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="550f1-1909">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="550f1-1910">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="550f1-1910">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="550f1-1911">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1911">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="550f1-1912">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="550f1-1912">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="550f1-1913">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1913">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1914">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-1914">Appservice</span></span>

* <span data-ttu-id="550f1-1915">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="550f1-1915">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="550f1-1916">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1916">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="550f1-1917">CDN</span><span class="sxs-lookup"><span data-stu-id="550f1-1917">CDN</span></span>

* <span data-ttu-id="550f1-1918">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1918">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="550f1-1919">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-1919">Container</span></span>

* <span data-ttu-id="550f1-1920">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="550f1-1920">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="550f1-1921">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1921">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="550f1-1922">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-1922">CosmosDB</span></span>

* <span data-ttu-id="550f1-1923">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1923">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="550f1-1924">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="550f1-1924">Extension</span></span>

* <span data-ttu-id="550f1-1925">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1925">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="550f1-1926">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1926">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="550f1-1927">Отзыв</span><span class="sxs-lookup"><span data-stu-id="550f1-1927">Feedback</span></span>

* <span data-ttu-id="550f1-1928">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="550f1-1928">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-1929">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-1929">Interactive</span></span>

* <span data-ttu-id="550f1-1930">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="550f1-1930">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="550f1-1931">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="550f1-1931">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-1932">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-1932">IoT</span></span>

* <span data-ttu-id="550f1-1933">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="550f1-1933">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="550f1-1934">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="550f1-1934">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="550f1-1935">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1935">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="550f1-1936">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="550f1-1936">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-1937">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-1937">Monitor</span></span>

* <span data-ttu-id="550f1-1938">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1938">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1939">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1939">Network</span></span>

* <span data-ttu-id="550f1-1940">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="550f1-1940">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="550f1-1941">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-1941">Profile</span></span>

* <span data-ttu-id="550f1-1942">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="550f1-1942">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-1943">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-1943">Resource</span></span>

* <span data-ttu-id="550f1-1944">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1944">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="550f1-1945">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-1945">Role</span></span>

* <span data-ttu-id="550f1-1946">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="550f1-1946">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-1947">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-1947">SQL</span></span>

* <span data-ttu-id="550f1-1948">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1948">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="550f1-1949">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1949">Added `sql db rename`</span></span>
* <span data-ttu-id="550f1-1950">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="550f1-1950">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1951">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1951">Storage</span></span>

* <span data-ttu-id="550f1-1952">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="550f1-1952">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1953">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1953">VM</span></span>

* <span data-ttu-id="550f1-1954">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="550f1-1954">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="550f1-1955">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="550f1-1955">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="550f1-1956">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="550f1-1956">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="550f1-1957">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-1957">January 31, 2018</span></span>

<span data-ttu-id="550f1-1958">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="550f1-1958">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="550f1-1959">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-1959">Core</span></span>

* <span data-ttu-id="550f1-1960">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="550f1-1960">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="550f1-1961">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="550f1-1961">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="550f1-1962">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="550f1-1962">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="550f1-1963">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="550f1-1963">Use `--verbose` to see</span></span>
* <span data-ttu-id="550f1-1964">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-1964">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-1965">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-1965">ACS</span></span>

* <span data-ttu-id="550f1-1966">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1966">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="550f1-1967">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1967">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-1968">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-1968">Appservice</span></span>

* <span data-ttu-id="550f1-1969">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="550f1-1969">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="550f1-1970">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="550f1-1970">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="550f1-1971">CDN</span><span class="sxs-lookup"><span data-stu-id="550f1-1971">CDN</span></span>

* <span data-ttu-id="550f1-1972">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1972">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="550f1-1973">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-1973">CosmosDB</span></span>

* <span data-ttu-id="550f1-1974">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="550f1-1974">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-1975">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-1975">Interactive</span></span>

* <span data-ttu-id="550f1-1976">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="550f1-1976">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="550f1-1977">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-1977">Network</span></span>

* <span data-ttu-id="550f1-1978">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1978">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="550f1-1979">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-1979">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="550f1-1980">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1980">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="550f1-1981">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1981">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="550f1-1982">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1982">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="550f1-1983">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="550f1-1983">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="550f1-1984">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="550f1-1984">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="550f1-1985">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="550f1-1985">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="550f1-1986">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1986">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="550f1-1987">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1987">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-1988">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-1988">Profile</span></span>

* <span data-ttu-id="550f1-1989">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="550f1-1989">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-1990">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-1990">Resource</span></span>

* <span data-ttu-id="550f1-1991">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="550f1-1991">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-1992">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-1992">Storage</span></span>

* <span data-ttu-id="550f1-1993">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="550f1-1993">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="550f1-1994">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="550f1-1994">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="550f1-1995">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1995">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="550f1-1996">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-1996">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="550f1-1997">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="550f1-1997">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-1998">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-1998">VM</span></span>

* <span data-ttu-id="550f1-1999">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="550f1-1999">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="550f1-2000">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2000">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="550f1-2001">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="550f1-2001">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="550f1-2002">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2002">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="550f1-2003">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2003">January 17, 2018</span></span>

<span data-ttu-id="550f1-2004">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="550f1-2004">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-2005">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-2005">ACR</span></span>

* <span data-ttu-id="550f1-2006">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="550f1-2006">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="550f1-2007">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="550f1-2007">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-2008">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2008">ACS</span></span>

* <span data-ttu-id="550f1-2009">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2009">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="550f1-2010">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-2010">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2011">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-2011">Appservice</span></span>

* <span data-ttu-id="550f1-2012">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="550f1-2012">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="550f1-2013">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2013">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="550f1-2014">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2014">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="550f1-2015">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="550f1-2015">Backup</span></span>

* <span data-ttu-id="550f1-2016">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="550f1-2016">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="550f1-2017">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="550f1-2017">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="550f1-2018">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="550f1-2018">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="550f1-2019">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="550f1-2019">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="550f1-2020">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="550f1-2020">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-2021">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-2021">Batch</span></span>

* <span data-ttu-id="550f1-2022">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="550f1-2022">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="550f1-2023">Облако</span><span class="sxs-lookup"><span data-stu-id="550f1-2023">Cloud</span></span>

* <span data-ttu-id="550f1-2024">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="550f1-2024">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="550f1-2025">Потребление</span><span class="sxs-lookup"><span data-stu-id="550f1-2025">Consumption</span></span>

* <span data-ttu-id="550f1-2026">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2026">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="550f1-2027">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-2027">Event Grid</span></span>

* <span data-ttu-id="550f1-2028">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2028">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="550f1-2029">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2029">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="550f1-2030">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2030">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="550f1-2031">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2031">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="550f1-2032">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2032">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="550f1-2033">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2033">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="550f1-2034">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2034">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="550f1-2035">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2035">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-2036">Interactive</span><span class="sxs-lookup"><span data-stu-id="550f1-2036">Interactive</span></span>

* <span data-ttu-id="550f1-2037">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="550f1-2037">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="550f1-2038">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="550f1-2038">Fixed errors on startup</span></span>
* <span data-ttu-id="550f1-2039">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="550f1-2039">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-2040">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-2040">IoT</span></span>

* <span data-ttu-id="550f1-2041">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="550f1-2041">Added support for device provisioning service</span></span>
* <span data-ttu-id="550f1-2042">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="550f1-2042">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="550f1-2043">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="550f1-2043">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-2044">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-2044">Monitor</span></span>

* <span data-ttu-id="550f1-2045">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="550f1-2045">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="550f1-2046">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2046">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="550f1-2047">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="550f1-2047">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="550f1-2048">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-2048">Network</span></span>

* <span data-ttu-id="550f1-2049">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="550f1-2049">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="550f1-2050">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="550f1-2050">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-2051">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-2051">Profile</span></span>

* <span data-ttu-id="550f1-2052">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="550f1-2052">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="550f1-2053">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-2053">Role</span></span>

* <span data-ttu-id="550f1-2054">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2054">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="550f1-2055">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="550f1-2055">Service Fabric</span></span>

* <span data-ttu-id="550f1-2056">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="550f1-2056">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="550f1-2057">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-2057">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2058">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2058">VM</span></span>

* <span data-ttu-id="550f1-2059">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2059">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="550f1-2060">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="550f1-2060">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="550f1-2061">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2061">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="550f1-2062">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="550f1-2062">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="550f1-2063">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="550f1-2063">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="550f1-2064">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2064">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="550f1-2065">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2065">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="550f1-2066">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2066">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="550f1-2067">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2067">December 19, 2017</span></span>

<span data-ttu-id="550f1-2068">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="550f1-2068">Version 2.0.23</span></span>

* <span data-ttu-id="550f1-2069">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="550f1-2069">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="550f1-2070">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-2070">Container</span></span>

* <span data-ttu-id="550f1-2071">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-2071">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="550f1-2072">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-2072">Network</span></span>

* <span data-ttu-id="550f1-2073">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="550f1-2073">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="550f1-2074">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="550f1-2074">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-2075">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-2075">Storage</span></span>

* <span data-ttu-id="550f1-2076">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="550f1-2076">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2077">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2077">VM</span></span>

* <span data-ttu-id="550f1-2078">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="550f1-2078">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="550f1-2079">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2079">December 5, 2017</span></span>

<span data-ttu-id="550f1-2080">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="550f1-2080">Version 2.0.22</span></span>

* <span data-ttu-id="550f1-2081">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2081">Removed `az component` commands.</span></span> <span data-ttu-id="550f1-2082">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2082">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="550f1-2083">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-2083">Core</span></span>
* <span data-ttu-id="550f1-2084">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="550f1-2084">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="550f1-2085">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="550f1-2085">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-2086">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2086">ACS</span></span>

* <span data-ttu-id="550f1-2087">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2087">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="550f1-2088">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2088">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="550f1-2089">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="550f1-2089">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="550f1-2090">Помощник</span><span class="sxs-lookup"><span data-stu-id="550f1-2090">Advisor</span></span>

* <span data-ttu-id="550f1-2091">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="550f1-2091">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2092">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-2092">Appservice</span></span>

* <span data-ttu-id="550f1-2093">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2093">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="550f1-2094">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="550f1-2094">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="550f1-2095">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2095">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="550f1-2096">Потребление</span><span class="sxs-lookup"><span data-stu-id="550f1-2096">Consumption</span></span>

* <span data-ttu-id="550f1-2097">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="550f1-2097">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="550f1-2098">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-2098">Container</span></span>

* <span data-ttu-id="550f1-2099">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="550f1-2099">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-2100">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-2100">Monitor</span></span>

* <span data-ttu-id="550f1-2101">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="550f1-2101">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-2102">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-2102">Resource</span></span>

* <span data-ttu-id="550f1-2103">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="550f1-2103">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="550f1-2104">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-2104">Role</span></span>

* <span data-ttu-id="550f1-2105">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2105">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="550f1-2106">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="550f1-2106">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="550f1-2107">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2107">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-2108">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-2108">SQL</span></span>

* <span data-ttu-id="550f1-2109">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2109">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="550f1-2110">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2110">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2111">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2111">VM</span></span>

* <span data-ttu-id="550f1-2112">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2112">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="550f1-2113">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2113">November 14, 2017</span></span>

<span data-ttu-id="550f1-2114">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="550f1-2114">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-2115">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-2115">ACR</span></span>

* <span data-ttu-id="550f1-2116">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="550f1-2116">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="550f1-2117">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2117">ACS</span></span>

* <span data-ttu-id="550f1-2118">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="550f1-2118">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="550f1-2119">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="550f1-2119">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="550f1-2120">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2120">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="550f1-2121">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="550f1-2121">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="550f1-2122">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="550f1-2122">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2123">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-2123">Appservice</span></span>

* <span data-ttu-id="550f1-2124">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="550f1-2124">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="550f1-2125">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2125">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="550f1-2126">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2126">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="550f1-2127">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2127">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="550f1-2128">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="550f1-2128">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="550f1-2129">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="550f1-2129">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-2130">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-2130">Batch</span></span>

* <span data-ttu-id="550f1-2131">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2131">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="550f1-2132">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="550f1-2132">Batchai</span></span>

* <span data-ttu-id="550f1-2133">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2133">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="550f1-2134">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2134">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="550f1-2135">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2135">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="550f1-2136">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2136">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="550f1-2137">Облако</span><span class="sxs-lookup"><span data-stu-id="550f1-2137">Cloud</span></span>

* <span data-ttu-id="550f1-2138">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="550f1-2138">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="550f1-2139">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-2139">Container</span></span>

* <span data-ttu-id="550f1-2140">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2140">Added support to open multiple ports</span></span>
* <span data-ttu-id="550f1-2141">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-2141">Added container group restart policy</span></span>
* <span data-ttu-id="550f1-2142">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="550f1-2142">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="550f1-2143">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="550f1-2143">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="550f1-2144">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="550f1-2144">Data Lake Analytics</span></span>

* <span data-ttu-id="550f1-2145">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="550f1-2145">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="550f1-2146">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="550f1-2146">Data Lake Store</span></span>

* <span data-ttu-id="550f1-2147">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="550f1-2147">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="550f1-2148">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="550f1-2148">Extension</span></span>

* <span data-ttu-id="550f1-2149">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="550f1-2149">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="550f1-2150">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="550f1-2150">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-2151">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-2151">IoT</span></span>

* <span data-ttu-id="550f1-2152">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2152">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-2153">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-2153">Monitor</span></span>

* <span data-ttu-id="550f1-2154">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2154">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="550f1-2155">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-2155">Network</span></span>

* <span data-ttu-id="550f1-2156">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="550f1-2156">Added support for CAA DNS records</span></span>
* <span data-ttu-id="550f1-2157">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2157">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="550f1-2158">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="550f1-2158">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="550f1-2159">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2159">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="550f1-2160">Резервирование</span><span class="sxs-lookup"><span data-stu-id="550f1-2160">Reservations</span></span>

* <span data-ttu-id="550f1-2161">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="550f1-2161">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-2162">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-2162">Resource</span></span>

* <span data-ttu-id="550f1-2163">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2163">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-2164">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-2164">SQL</span></span>

* <span data-ttu-id="550f1-2165">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2165">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-2166">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-2166">Storage</span></span>

* <span data-ttu-id="550f1-2167">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-2167">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="550f1-2168">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="550f1-2168">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="550f1-2169">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2169">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="550f1-2170">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2170">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="550f1-2171">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2171">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="550f1-2172">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2172">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="550f1-2173">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2173">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2174">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2174">VM</span></span>

* <span data-ttu-id="550f1-2175">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2175">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="550f1-2176">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2176">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="550f1-2177">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2177">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="550f1-2178">Команда `vm format-secret` переименована в `vm secret format`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2178">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="550f1-2179">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="550f1-2179">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="550f1-2180">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2180">October 24, 2017</span></span>

<span data-ttu-id="550f1-2181">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="550f1-2181">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="550f1-2182">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-2182">Core</span></span>

* <span data-ttu-id="550f1-2183">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="550f1-2183">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-2184">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-2184">ACR</span></span>

* <span data-ttu-id="550f1-2185">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="550f1-2185">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="550f1-2186">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="550f1-2186">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="550f1-2187">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="550f1-2187">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-2188">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2188">ACS</span></span>

* <span data-ttu-id="550f1-2189">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="550f1-2189">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="550f1-2190">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="550f1-2190">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2191">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-2191">Appservice</span></span>

* <span data-ttu-id="550f1-2192">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="550f1-2192">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="550f1-2193">Компонент</span><span class="sxs-lookup"><span data-stu-id="550f1-2193">Component</span></span>

* <span data-ttu-id="550f1-2194">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="550f1-2194">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-2195">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-2195">Monitor</span></span>

* <span data-ttu-id="550f1-2196">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2196">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-2197">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-2197">Resource</span></span>

* <span data-ttu-id="550f1-2198">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="550f1-2198">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="550f1-2199">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="550f1-2199">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2200">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2200">VM</span></span>

* <span data-ttu-id="550f1-2201">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="550f1-2201">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="550f1-2202">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2202">October 9, 2017</span></span>

<span data-ttu-id="550f1-2203">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="550f1-2203">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="550f1-2204">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-2204">Core</span></span>

* <span data-ttu-id="550f1-2205">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="550f1-2205">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2206">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-2206">Appservice</span></span>

* <span data-ttu-id="550f1-2207">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2207">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-2208">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-2208">Batch</span></span>

* <span data-ttu-id="550f1-2209">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="550f1-2209">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="550f1-2210">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="550f1-2210">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="550f1-2211">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-2211">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="550f1-2212">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2212">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="550f1-2213">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="550f1-2213">Batchai</span></span>

* <span data-ttu-id="550f1-2214">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="550f1-2214">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="550f1-2215">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="550f1-2215">Keyvault</span></span>

* <span data-ttu-id="550f1-2216">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="550f1-2216">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="550f1-2217">(#4448)</span><span class="sxs-lookup"><span data-stu-id="550f1-2217">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="550f1-2218">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-2218">Network</span></span>

* <span data-ttu-id="550f1-2219">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="550f1-2219">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="550f1-2220">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="550f1-2220">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-2221">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-2221">Resource</span></span>

* <span data-ttu-id="550f1-2222">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2222">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="550f1-2223">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="550f1-2223">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="550f1-2224">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="550f1-2224">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="550f1-2225">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="550f1-2225">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-2226">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-2226">Sql</span></span>

* <span data-ttu-id="550f1-2227">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="550f1-2227">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="550f1-2228">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="550f1-2228">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="550f1-2229">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="550f1-2229">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-2230">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-2230">Storage</span></span>

* <span data-ttu-id="550f1-2231">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2231">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2232">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="550f1-2232">Vm</span></span>

* <span data-ttu-id="550f1-2233">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2233">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="550f1-2234">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2234">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="550f1-2235">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2235">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="550f1-2236">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2236">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="550f1-2237">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="550f1-2237">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="550f1-2238">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2238">September 22, 2017</span></span>

<span data-ttu-id="550f1-2239">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="550f1-2239">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-2240">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-2240">Resource</span></span>

* <span data-ttu-id="550f1-2241">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="550f1-2241">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="550f1-2242">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="550f1-2242">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="550f1-2243">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="550f1-2243">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="550f1-2244">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2244">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-2245">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-2245">Network</span></span>

* <span data-ttu-id="550f1-2246">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="550f1-2246">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="550f1-2247">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="550f1-2247">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="550f1-2248">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="550f1-2248">Added `asg` application security group commands</span></span>
* <span data-ttu-id="550f1-2249">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="550f1-2249">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="550f1-2250">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="550f1-2250">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="550f1-2251">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="550f1-2251">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="550f1-2252">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2252">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-2253">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-2253">Storage</span></span>

* <span data-ttu-id="550f1-2254">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="550f1-2254">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="550f1-2255">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="550f1-2255">Eventgrid</span></span>

* <span data-ttu-id="550f1-2256">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="550f1-2256">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-2257">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-2257">SQL</span></span>

* <span data-ttu-id="550f1-2258">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="550f1-2258">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="550f1-2259">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="550f1-2259">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="550f1-2260">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="550f1-2260">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="550f1-2261">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="550f1-2261">Keyvault</span></span>

* <span data-ttu-id="550f1-2262">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="550f1-2262">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2263">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2263">VM</span></span>

* <span data-ttu-id="550f1-2264">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="550f1-2264">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="550f1-2265">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="550f1-2265">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="550f1-2266">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="550f1-2266">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="550f1-2267">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="550f1-2267">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="550f1-2268">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="550f1-2268">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="550f1-2269">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="550f1-2269">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-2270">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2270">ACS</span></span>

* <span data-ttu-id="550f1-2271">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="550f1-2271">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2272">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-2272">Appservice</span></span>

* <span data-ttu-id="550f1-2273">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="550f1-2273">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="550f1-2274">Azure Backup</span><span class="sxs-lookup"><span data-stu-id="550f1-2274">Backup</span></span>

* <span data-ttu-id="550f1-2275">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="550f1-2275">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="550f1-2276">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2276">September 11, 2017</span></span>

<span data-ttu-id="550f1-2277">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="550f1-2277">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="550f1-2278">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-2278">Core</span></span>

* <span data-ttu-id="550f1-2279">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="550f1-2279">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="550f1-2280">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="550f1-2280">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-2281">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2281">Acs</span></span>

* <span data-ttu-id="550f1-2282">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2282">Added `acs list-locations` command</span></span>
* <span data-ttu-id="550f1-2283">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-2283">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2284">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-2284">Appservice</span></span>

* <span data-ttu-id="550f1-2285">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="550f1-2285">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="550f1-2286">CDN</span><span class="sxs-lookup"><span data-stu-id="550f1-2286">CDN</span></span>

* <span data-ttu-id="550f1-2287">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2287">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="550f1-2288">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="550f1-2288">Extension</span></span>

* <span data-ttu-id="550f1-2289">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="550f1-2289">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="550f1-2290">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="550f1-2290">Keyvault</span></span>

* <span data-ttu-id="550f1-2291">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2291">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-2292">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-2292">Network</span></span>

* <span data-ttu-id="550f1-2293">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2293">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="550f1-2294">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2294">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="550f1-2295">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2295">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="550f1-2296">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2296">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="550f1-2297">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2297">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-2298">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-2298">Resource</span></span>

* <span data-ttu-id="550f1-2299">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2299">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="550f1-2300">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2300">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="550f1-2301">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="550f1-2301">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="550f1-2302">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="550f1-2302">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-2303">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-2303">SQL</span></span>

* <span data-ttu-id="550f1-2304">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2304">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2305">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2305">VM</span></span>

* <span data-ttu-id="550f1-2306">Исправлено. Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="550f1-2306">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="550f1-2307">Исправлено. Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="550f1-2307">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="550f1-2308">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2308">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="550f1-2309">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="550f1-2309">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="550f1-2310">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="550f1-2310">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="550f1-2311">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2311">August 31, 2017</span></span>

<span data-ttu-id="550f1-2312">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="550f1-2312">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="550f1-2313">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="550f1-2313">Keyvault</span></span>

* <span data-ttu-id="550f1-2314">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2314">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="550f1-2315">Sf</span><span class="sxs-lookup"><span data-stu-id="550f1-2315">Sf</span></span>

* <span data-ttu-id="550f1-2316">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="550f1-2316">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-2317">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-2317">Storage</span></span>

* <span data-ttu-id="550f1-2318">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="550f1-2318">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="550f1-2319">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="550f1-2319">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="550f1-2320">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2320">August 28, 2017</span></span>

<span data-ttu-id="550f1-2321">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="550f1-2321">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="550f1-2322">CLI</span><span class="sxs-lookup"><span data-stu-id="550f1-2322">CLI</span></span>

* <span data-ttu-id="550f1-2323">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="550f1-2323">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-2324">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2324">ACS</span></span>

* <span data-ttu-id="550f1-2325">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="550f1-2325">Corrected preview regions</span></span>
* <span data-ttu-id="550f1-2326">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2326">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="550f1-2327">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="550f1-2327">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2328">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-2328">Appservice</span></span>

* <span data-ttu-id="550f1-2329">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2329">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="550f1-2330">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2330">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="550f1-2331">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2331">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="550f1-2332">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="550f1-2332">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="550f1-2333">Исправлено. Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="550f1-2333">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-2334">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-2334">IoT</span></span>

* <span data-ttu-id="550f1-2335">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="550f1-2335">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="550f1-2336">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-2336">Network</span></span>

* <span data-ttu-id="550f1-2337">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2337">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="550f1-2338">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2338">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="550f1-2339">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2339">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="550f1-2340">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2340">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="550f1-2341">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2341">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-2342">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-2342">Profile</span></span>

* <span data-ttu-id="550f1-2343">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="550f1-2343">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="550f1-2344">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="550f1-2344">Service Fabric</span></span>

* <span data-ttu-id="550f1-2345">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="550f1-2345">Preview release</span></span>
* <span data-ttu-id="550f1-2346">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="550f1-2346">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="550f1-2347">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="550f1-2347">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="550f1-2348">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2348">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-2349">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-2349">Storage</span></span>

* <span data-ttu-id="550f1-2350">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="550f1-2350">Enabled setting blob tier</span></span>
* <span data-ttu-id="550f1-2351">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-2351">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="550f1-2352">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2352">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="550f1-2353">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="550f1-2353">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="550f1-2354">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2354">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="550f1-2355">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2355">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2356">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2356">VM</span></span>

* <span data-ttu-id="550f1-2357">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2357">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="550f1-2358">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2358">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="550f1-2359">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="550f1-2359">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="550f1-2360">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="550f1-2360">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="550f1-2361">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="550f1-2361">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="550f1-2362">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2362">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="550f1-2363">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2363">August 15, 2017</span></span>

<span data-ttu-id="550f1-2364">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="550f1-2364">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-2365">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2365">ACS</span></span>

* <span data-ttu-id="550f1-2366">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="550f1-2366">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2367">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-2367">Appservice</span></span>

* <span data-ttu-id="550f1-2368">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="550f1-2368">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="550f1-2369">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-2369">Event Grid</span></span>

* <span data-ttu-id="550f1-2370">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="550f1-2370">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="550f1-2371">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2371">August 11, 2017</span></span>

<span data-ttu-id="550f1-2372">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="550f1-2372">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-2373">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2373">ACS</span></span>

* <span data-ttu-id="550f1-2374">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="550f1-2374">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-2375">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-2375">Batch</span></span>

* <span data-ttu-id="550f1-2376">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="550f1-2376">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="550f1-2377">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="550f1-2377">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="550f1-2378">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2378">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="550f1-2379">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="550f1-2379">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="550f1-2380">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="550f1-2380">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="550f1-2381">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="550f1-2381">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="550f1-2382">Компонент</span><span class="sxs-lookup"><span data-stu-id="550f1-2382">Component</span></span>

* <span data-ttu-id="550f1-2383">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="550f1-2383">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="550f1-2384">Контейнер</span><span class="sxs-lookup"><span data-stu-id="550f1-2384">Container</span></span>

* <span data-ttu-id="550f1-2385">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="550f1-2385">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="550f1-2386">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="550f1-2386">Data Lake Store</span></span>

* <span data-ttu-id="550f1-2387">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="550f1-2387">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="550f1-2388">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-2388">Event Grid</span></span>

* <span data-ttu-id="550f1-2389">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="550f1-2389">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="550f1-2390">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-2390">Network</span></span>

* <span data-ttu-id="550f1-2391">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="550f1-2391">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="550f1-2392">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2392">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="550f1-2393">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2393">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="550f1-2394">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2394">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-2395">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-2395">Profile</span></span>

* <span data-ttu-id="550f1-2396">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="550f1-2396">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-2397">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-2397">Storage</span></span>

* <span data-ttu-id="550f1-2398">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="550f1-2398">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2399">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2399">VM</span></span>

* <span data-ttu-id="550f1-2400">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="550f1-2400">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="550f1-2401">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2401">Exposed `list-skus` command</span></span>
* <span data-ttu-id="550f1-2402">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="550f1-2402">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="550f1-2403">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="550f1-2403">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="550f1-2404">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="550f1-2404">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="550f1-2405">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2405">July 28, 2017</span></span>

<span data-ttu-id="550f1-2406">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="550f1-2406">Version 2.0.12</span></span>

* <span data-ttu-id="550f1-2407">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="550f1-2407">Added container commands</span></span>
* <span data-ttu-id="550f1-2408">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2408">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="550f1-2409">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-2409">Core</span></span>

* <span data-ttu-id="550f1-2410">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2410">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="550f1-2411">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="550f1-2411">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="550f1-2412">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="550f1-2412">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="550f1-2413">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="550f1-2413">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="550f1-2414">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="550f1-2414">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="550f1-2415">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="550f1-2415">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="550f1-2416">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="550f1-2416">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="550f1-2417">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="550f1-2417">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="550f1-2418">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="550f1-2418">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="550f1-2419">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="550f1-2419">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="550f1-2420">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="550f1-2420">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="550f1-2421">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="550f1-2421">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="550f1-2422">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="550f1-2422">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="550f1-2423">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="550f1-2423">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="550f1-2424">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="550f1-2424">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="550f1-2425">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="550f1-2425">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="550f1-2426">ACR</span><span class="sxs-lookup"><span data-stu-id="550f1-2426">ACR</span></span>

* <span data-ttu-id="550f1-2427">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="550f1-2427">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="550f1-2428">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="550f1-2428">Support SKU update for managed registries</span></span>
* <span data-ttu-id="550f1-2429">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="550f1-2429">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="550f1-2430">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="550f1-2430">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="550f1-2431">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="550f1-2431">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="550f1-2432">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="550f1-2432">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-2433">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2433">ACS</span></span>

* <span data-ttu-id="550f1-2434">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="550f1-2434">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2435">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="550f1-2435">Appservice</span></span>

* <span data-ttu-id="550f1-2436">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="550f1-2436">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="550f1-2437">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="550f1-2437">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="550f1-2438">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2438">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="550f1-2439">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="550f1-2439">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="550f1-2440">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="550f1-2440">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="550f1-2441">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="550f1-2441">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="550f1-2442">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="550f1-2442">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="550f1-2443">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="550f1-2443">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="550f1-2444">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="550f1-2444">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="550f1-2445">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2445">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="550f1-2446">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="550f1-2446">Batch</span></span>

* <span data-ttu-id="550f1-2447">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="550f1-2447">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="550f1-2448">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2448">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="550f1-2449">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2449">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="550f1-2450">CDN</span><span class="sxs-lookup"><span data-stu-id="550f1-2450">CDN</span></span>

* <span data-ttu-id="550f1-2451">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="550f1-2451">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="550f1-2452">Облако</span><span class="sxs-lookup"><span data-stu-id="550f1-2452">Cloud</span></span>

* <span data-ttu-id="550f1-2453">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="550f1-2453">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="550f1-2454">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="550f1-2454">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="550f1-2455">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="550f1-2455">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="550f1-2456">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="550f1-2456">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="550f1-2457">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2457">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="550f1-2458">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-2458">CosmosDB</span></span>

* <span data-ttu-id="550f1-2459">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="550f1-2459">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="550f1-2460">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="550f1-2460">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="550f1-2461">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="550f1-2461">Data Lake Analytics</span></span>

* <span data-ttu-id="550f1-2462">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2462">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="550f1-2463">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2463">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="550f1-2464">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2464">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="550f1-2465">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="550f1-2465">Data Lake Store</span></span>

* <span data-ttu-id="550f1-2466">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2466">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="550f1-2467">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="550f1-2467">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="550f1-2468">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2468">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="550f1-2469">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="550f1-2469">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="550f1-2470">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="550f1-2470">Interactive</span></span>

* <span data-ttu-id="550f1-2471">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="550f1-2471">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="550f1-2472">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="550f1-2472">Increased test coverage</span></span>
* <span data-ttu-id="550f1-2473">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="550f1-2473">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="550f1-2474">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="550f1-2474">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="550f1-2475">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="550f1-2475">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="550f1-2476">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="550f1-2476">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="550f1-2477">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="550f1-2477">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="550f1-2478">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2478">Added `--progress` flag</span></span>
* <span data-ttu-id="550f1-2479">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2479">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="550f1-2480">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="550f1-2480">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="550f1-2481">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="550f1-2481">IoT</span></span>

* <span data-ttu-id="550f1-2482">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="550f1-2482">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="550f1-2483">(3934).</span><span class="sxs-lookup"><span data-stu-id="550f1-2483">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="550f1-2484">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="550f1-2484">Key vault</span></span>

* <span data-ttu-id="550f1-2485">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="550f1-2485">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="550f1-2486">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2486">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="550f1-2487">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="550f1-2487">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="550f1-2488">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="550f1-2488">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="550f1-2489">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2489">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="550f1-2490">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="550f1-2490">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="550f1-2491">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="550f1-2491">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="550f1-2492">(3307).</span><span class="sxs-lookup"><span data-stu-id="550f1-2492">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="550f1-2493">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="550f1-2493">Lab</span></span>

* <span data-ttu-id="550f1-2494">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2494">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="550f1-2495">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2495">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-2496">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-2496">Monitor</span></span>

* <span data-ttu-id="550f1-2497">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="550f1-2497">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="550f1-2498">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2498">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="550f1-2499">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2499">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="550f1-2500">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2500">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="550f1-2501">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2501">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="550f1-2502">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="550f1-2502">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="550f1-2503">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="550f1-2503">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="550f1-2504">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="550f1-2504">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="550f1-2505">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="550f1-2505">`location` no longer required</span></span>
  * <span data-ttu-id="550f1-2506">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="550f1-2506">Add name and ID support for target</span></span>
  * <span data-ttu-id="550f1-2507">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="550f1-2507">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="550f1-2508">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="550f1-2508">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="550f1-2509">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="550f1-2509">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="550f1-2510">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="550f1-2510">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="550f1-2511">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2511">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="550f1-2512">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2512">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="550f1-2513">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-2513">Network</span></span>

* <span data-ttu-id="550f1-2514">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2514">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="550f1-2515">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2515">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="550f1-2516">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="550f1-2516">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="550f1-2517">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2517">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="550f1-2518">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2518">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="550f1-2519">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2519">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="550f1-2520">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2520">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="550f1-2521">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2521">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="550f1-2522">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2522">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="550f1-2523">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2523">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="550f1-2524">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2524">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="550f1-2525">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2525">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="550f1-2526">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2526">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="550f1-2527">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2527">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="550f1-2528">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2528">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="550f1-2529">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2529">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="550f1-2530">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="550f1-2530">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="550f1-2531">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2531">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="550f1-2532">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2532">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="550f1-2533">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2533">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="550f1-2534">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2534">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="550f1-2535">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2535">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="550f1-2536">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2536">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="550f1-2537">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="550f1-2537">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="550f1-2538">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="550f1-2538">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="550f1-2539">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="550f1-2539">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="550f1-2540">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="550f1-2540">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-2541">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-2541">Profile</span></span>

* <span data-ttu-id="550f1-2542">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="550f1-2542">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="550f1-2543">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="550f1-2543">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="550f1-2544">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="550f1-2544">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="550f1-2545">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="550f1-2545">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="550f1-2546">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="550f1-2546">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="550f1-2547">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="550f1-2547">RDBMS</span></span>

* <span data-ttu-id="550f1-2548">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="550f1-2548">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="550f1-2549">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="550f1-2549">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="550f1-2550">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="550f1-2550">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="550f1-2551">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="550f1-2551">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-2552">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-2552">Resource</span></span>

* <span data-ttu-id="550f1-2553">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2553">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="550f1-2554">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2554">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="550f1-2555">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2555">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="550f1-2556">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2556">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="550f1-2557">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="550f1-2557">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="550f1-2558">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2558">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="550f1-2559">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="550f1-2559">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="550f1-2560">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2560">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="550f1-2561">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-2561">Role</span></span>

* <span data-ttu-id="550f1-2562">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="550f1-2562">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="550f1-2563">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="550f1-2563">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="550f1-2564">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="550f1-2564">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="550f1-2565">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="550f1-2565">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="550f1-2566">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2566">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="550f1-2567">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="550f1-2567">Service Fabric</span></span>
* <span data-ttu-id="550f1-2568">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="550f1-2568">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="550f1-2569">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="550f1-2569">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="550f1-2570">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="550f1-2570">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-2571">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-2571">SQL</span></span>

* <span data-ttu-id="550f1-2572">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2572">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="550f1-2573">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2573">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="550f1-2574">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2574">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-2575">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-2575">Storage</span></span>

* <span data-ttu-id="550f1-2576">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="550f1-2576">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="550f1-2577">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="550f1-2577">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="550f1-2578">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="550f1-2578">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="550f1-2579">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="550f1-2579">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="550f1-2580">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="550f1-2580">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="550f1-2581">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="550f1-2581">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2582">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2582">VM</span></span>

* <span data-ttu-id="550f1-2583">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="550f1-2583">Support configuring nsg</span></span>
* <span data-ttu-id="550f1-2584">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="550f1-2584">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="550f1-2585">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="550f1-2585">Support managed service identities</span></span>
* <span data-ttu-id="550f1-2586">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2586">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="550f1-2587">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="550f1-2587">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="550f1-2588">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2588">May 10, 2017</span></span>

<span data-ttu-id="550f1-2589">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="550f1-2589">Version 2.0.6</span></span>

* <span data-ttu-id="550f1-2590">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="550f1-2590">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="550f1-2591">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="550f1-2591">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="550f1-2592">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="550f1-2592">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="550f1-2593">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="550f1-2593">Include Cognitive Services module</span></span>
* <span data-ttu-id="550f1-2594">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="550f1-2594">Include Service Fabric module</span></span>
* <span data-ttu-id="550f1-2595">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="550f1-2595">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="550f1-2596">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="550f1-2596">Add support for CDN commands</span></span>
* <span data-ttu-id="550f1-2597">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="550f1-2597">Remove Container module</span></span>
* <span data-ttu-id="550f1-2598">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2598">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="550f1-2599">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2599">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="550f1-2600">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-2600">Core</span></span>

* <span data-ttu-id="550f1-2601">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="550f1-2601">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="550f1-2602">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2602">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="550f1-2603">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2603">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="550f1-2604">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2604">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="550f1-2605">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2605">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="550f1-2606">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2606">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="550f1-2607">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2607">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="550f1-2608">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2608">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="550f1-2609">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2609">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="550f1-2610">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="550f1-2610">core: Improved performance</span></span>
* <span data-ttu-id="550f1-2611">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="550f1-2611">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="550f1-2612">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="550f1-2612">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-2613">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2613">ACS</span></span>

* <span data-ttu-id="550f1-2614">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="550f1-2614">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="550f1-2615">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="550f1-2615">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="550f1-2616">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="550f1-2616">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="550f1-2617">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2617">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2618">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-2618">AppService</span></span>

* <span data-ttu-id="550f1-2619">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="550f1-2619">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="550f1-2620">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="550f1-2620">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="550f1-2621">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="550f1-2621">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="550f1-2622">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="550f1-2622">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="550f1-2623">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="550f1-2623">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="550f1-2624">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2624">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="550f1-2625">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="550f1-2625">support slot swap with preview</span></span>
* <span data-ttu-id="550f1-2626">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2626">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="550f1-2627">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2627">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="550f1-2628">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="550f1-2628">CosmosDB</span></span>

* <span data-ttu-id="550f1-2629">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="550f1-2629">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="550f1-2630">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="550f1-2630">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="550f1-2631">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="550f1-2631">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="550f1-2632">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="550f1-2632">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="550f1-2633">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="550f1-2633">Data Lake Analytics</span></span>

* <span data-ttu-id="550f1-2634">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="550f1-2634">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="550f1-2635">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="550f1-2635">Add support for new catalog item type: package.</span></span> <span data-ttu-id="550f1-2636">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2636">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="550f1-2637">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="550f1-2637">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="550f1-2638">Таблица</span><span class="sxs-lookup"><span data-stu-id="550f1-2638">Table</span></span>
  * <span data-ttu-id="550f1-2639">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="550f1-2639">Table valued function</span></span>
  * <span data-ttu-id="550f1-2640">Просмотр</span><span class="sxs-lookup"><span data-stu-id="550f1-2640">View</span></span>
  * <span data-ttu-id="550f1-2641">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="550f1-2641">Table Statistics.</span></span> <span data-ttu-id="550f1-2642">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="550f1-2642">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="550f1-2643">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="550f1-2643">Data Lake Store</span></span>

* <span data-ttu-id="550f1-2644">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="550f1-2644">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="550f1-2645">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2645">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="550f1-2646">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="550f1-2646">missed help for access show.</span></span> <span data-ttu-id="550f1-2647">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="550f1-2647">adding it.</span></span> <span data-ttu-id="550f1-2648">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="550f1-2648">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="550f1-2649">Поиск</span><span class="sxs-lookup"><span data-stu-id="550f1-2649">Find</span></span>

* <span data-ttu-id="550f1-2650">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="550f1-2650">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="550f1-2651">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="550f1-2651">KeyVault</span></span>

* <span data-ttu-id="550f1-2652">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="550f1-2652">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="550f1-2653">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="550f1-2653">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="550f1-2654">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="550f1-2654">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="550f1-2655">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="550f1-2655">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="550f1-2656">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2656">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="550f1-2657">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="550f1-2657">Lab</span></span>

* <span data-ttu-id="550f1-2658">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="550f1-2658">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="550f1-2659">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="550f1-2659">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="550f1-2660">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="550f1-2660">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="550f1-2661">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="550f1-2661">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="550f1-2662">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="550f1-2662">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="550f1-2663">Мониторинг</span><span class="sxs-lookup"><span data-stu-id="550f1-2663">Monitor</span></span>

* <span data-ttu-id="550f1-2664">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2664">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="550f1-2665">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2665">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="550f1-2666">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-2666">Network</span></span>

* <span data-ttu-id="550f1-2667">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2667">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="550f1-2668">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2668">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="550f1-2669">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="550f1-2669">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="550f1-2670">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="550f1-2670">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="550f1-2671">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="550f1-2671">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="550f1-2672">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="550f1-2672">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="550f1-2673">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="550f1-2673">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="550f1-2674">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="550f1-2674">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="550f1-2675">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2675">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="550f1-2676">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="550f1-2676">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="550f1-2677">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2677">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="550f1-2678">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2678">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="550f1-2679">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="550f1-2679">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="550f1-2680">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="550f1-2680">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="550f1-2681">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="550f1-2681">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="550f1-2682">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="550f1-2682">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="550f1-2683">Профиль</span><span class="sxs-lookup"><span data-stu-id="550f1-2683">Profile</span></span>

* <span data-ttu-id="550f1-2684">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2684">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="550f1-2685">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2685">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="550f1-2686">Redis</span><span class="sxs-lookup"><span data-stu-id="550f1-2686">Redis</span></span>

* <span data-ttu-id="550f1-2687">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="550f1-2687">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="550f1-2688">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="550f1-2688">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="550f1-2689">Ресурс</span><span class="sxs-lookup"><span data-stu-id="550f1-2689">Resource</span></span>

* <span data-ttu-id="550f1-2690">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2690">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="550f1-2691">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2691">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="550f1-2692">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2692">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="550f1-2693">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="550f1-2693">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="550f1-2694">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="550f1-2694">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="550f1-2695">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="550f1-2695">Add docs for az lock update.</span></span> <span data-ttu-id="550f1-2696">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="550f1-2696">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="550f1-2697">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="550f1-2697">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="550f1-2698">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="550f1-2698">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="550f1-2699">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="550f1-2699">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="550f1-2700">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="550f1-2700">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="550f1-2701">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2701">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="550f1-2702">Роль</span><span class="sxs-lookup"><span data-stu-id="550f1-2702">Role</span></span>

* <span data-ttu-id="550f1-2703">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2703">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="550f1-2704">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2704">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="550f1-2705">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2705">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="550f1-2706">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="550f1-2706">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="550f1-2707">SQL</span><span class="sxs-lookup"><span data-stu-id="550f1-2707">SQL</span></span>

* <span data-ttu-id="550f1-2708">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="550f1-2708">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="550f1-2709">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2709">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="550f1-2710">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-2710">Storage</span></span>

* <span data-ttu-id="550f1-2711">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2711">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="550f1-2712">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2712">Add support for incremental blob copy</span></span>
* <span data-ttu-id="550f1-2713">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="550f1-2713">Add support for large block blob upload</span></span>
* <span data-ttu-id="550f1-2714">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="550f1-2714">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2715">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2715">VM</span></span>

* <span data-ttu-id="550f1-2716">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="550f1-2716">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="550f1-2717">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="550f1-2717">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="550f1-2718">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="550f1-2718">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="550f1-2719">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="550f1-2719">az vm/vmss disk</span></span>
  3. <span data-ttu-id="550f1-2720">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="550f1-2720">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="550f1-2721">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="550f1-2721">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="550f1-2722">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2722">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="550f1-2723">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2723">April 3, 2017</span></span>

<span data-ttu-id="550f1-2724">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="550f1-2724">Version 2.0.2</span></span>

<span data-ttu-id="550f1-2725">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="550f1-2725">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="550f1-2726">Core</span><span class="sxs-lookup"><span data-stu-id="550f1-2726">Core</span></span>

* <span data-ttu-id="550f1-2727">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-2727">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="550f1-2728">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2728">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="550f1-2729">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2729">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="550f1-2730">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2730">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="550f1-2731">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2731">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="550f1-2732">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="550f1-2732">Add prompting for missing template parameters.</span></span> <span data-ttu-id="550f1-2733">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2733">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="550f1-2734">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="550f1-2734">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="550f1-2735">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="550f1-2735">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="550f1-2736">ACS</span><span class="sxs-lookup"><span data-stu-id="550f1-2736">ACS</span></span>

* <span data-ttu-id="550f1-2737">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2737">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="550f1-2738">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="550f1-2738">Add support for ssh key password prompting.</span></span> <span data-ttu-id="550f1-2739">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2739">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="550f1-2740">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="550f1-2740">Add support for windows clusters.</span></span> <span data-ttu-id="550f1-2741">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2741">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="550f1-2742">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="550f1-2742">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="550f1-2743">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2743">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="550f1-2744">AppService</span><span class="sxs-lookup"><span data-stu-id="550f1-2744">AppService</span></span>

* <span data-ttu-id="550f1-2745">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2745">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="550f1-2746">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2746">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="550f1-2747">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2747">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="550f1-2748">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2748">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="550f1-2749">Data Lake</span><span class="sxs-lookup"><span data-stu-id="550f1-2749">DataLake</span></span>

* <span data-ttu-id="550f1-2750">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="550f1-2750">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="550f1-2751">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="550f1-2751">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="550f1-2752">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="550f1-2752">DocuemntDB</span></span>

* <span data-ttu-id="550f1-2753">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2753">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="550f1-2754">ВМ</span><span class="sxs-lookup"><span data-stu-id="550f1-2754">VM</span></span>

* <span data-ttu-id="550f1-2755">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2755">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="550f1-2756">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2756">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="550f1-2757">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2757">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="550f1-2758">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2758">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="550f1-2759">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2759">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="550f1-2760">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2760">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="550f1-2761">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="550f1-2761">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="550f1-2762">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="550f1-2762">February 27, 2017</span></span>

<span data-ttu-id="550f1-2763">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="550f1-2763">Version 2.0.0</span></span>

<span data-ttu-id="550f1-2764">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="550f1-2764">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="550f1-2765">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="550f1-2765">Container Service (acs)</span></span>
- <span data-ttu-id="550f1-2766">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="550f1-2766">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="550f1-2767">Сеть</span><span class="sxs-lookup"><span data-stu-id="550f1-2767">Networking</span></span>
- <span data-ttu-id="550f1-2768">Хранилище</span><span class="sxs-lookup"><span data-stu-id="550f1-2768">Storage</span></span>

<span data-ttu-id="550f1-2769">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2769">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="550f1-2770">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="550f1-2770">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="550f1-2771">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="550f1-2771">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="550f1-2772">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="550f1-2772">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="550f1-2773">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="550f1-2773">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="550f1-2774">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="550f1-2774">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="550f1-2775">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="550f1-2775">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="550f1-2776">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="550f1-2776">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="550f1-2777">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="550f1-2777">Provide feedback from the command line with the `az feedback` command</span></span>

