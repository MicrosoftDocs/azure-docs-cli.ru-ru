---
title: Заметки о выпуске Azure CLI
description: Узнайте о последних обновлениях в Azure CLI
author: dbradish-microsoft
ms.author: dbradish
manager: barbkess
ms.date: 02/04/2020
ms.topic: article
ms.prod: azure
ms.technology: azure-cli
ms.devlang: azurecli
ms.openlocfilehash: eafd18344ac4c1c0124ff53864a45510070b6fe7
ms.sourcegitcommit: d0b2763cc856eef44a6ecb78f6b8c64291625750
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/04/2020
ms.locfileid: "77013290"
---
# <a name="azure-cli-release-notes"></a><span data-ttu-id="8b368-103">Заметки о выпуске Azure CLI</span><span class="sxs-lookup"><span data-stu-id="8b368-103">Azure CLI release notes</span></span>

## <a name="february-04-2020"></a><span data-ttu-id="8b368-104">4 февраля 2020 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-104">February 04, 2020</span></span>

<span data-ttu-id="8b368-105">Версия 2.0.81</span><span class="sxs-lookup"><span data-stu-id="8b368-105">Version 2.0.81</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-106">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-106">ACS</span></span>

* <span data-ttu-id="8b368-107">Добавлена возможность задания выделенных исходящих портов и времени ожидания подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="8b368-107">Add support to set outbound allocated ports and idle timeouts on standard load balancer</span></span>
* <span data-ttu-id="8b368-108">Выполнено обновление до API версии 2019-11-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-108">Update to API Version 2019-11-01</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-109">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-109">ACR</span></span>

* <span data-ttu-id="8b368-110">[Критическое изменение] `az acr delete` будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="8b368-110">[BREAKING CHANGE] `az acr delete` will prompt</span></span>
* <span data-ttu-id="8b368-111">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда az acr task delete будет выводить запрос.</span><span class="sxs-lookup"><span data-stu-id="8b368-111">[BREAKING CHANGE] 'az acr task delete' will prompt</span></span>
* <span data-ttu-id="8b368-112">Добавлена новая группа команд az acr taskrun show/list/delete для управления выполнением задач.</span><span class="sxs-lookup"><span data-stu-id="8b368-112">Add a new command group 'az acr taskrun show/list/delete' for taskrun management</span></span>

### <a name="aks"></a><span data-ttu-id="8b368-113">AKS</span><span class="sxs-lookup"><span data-stu-id="8b368-113">AKS</span></span>

* <span data-ttu-id="8b368-114">Каждый кластер получает отдельный субъект-службу для улучшения изоляции.</span><span class="sxs-lookup"><span data-stu-id="8b368-114">Each cluster gets a separate service principal to improve isolation</span></span>

### <a name="appconfig"></a><span data-ttu-id="8b368-115">AppConfig</span><span class="sxs-lookup"><span data-stu-id="8b368-115">AppConfig</span></span>

* <span data-ttu-id="8b368-116">Поддержка импорта ссылок на хранилище ключей из службы приложений и их экспорта в нее.</span><span class="sxs-lookup"><span data-stu-id="8b368-116">Support import/export of keyvault references from/to appservice</span></span>
* <span data-ttu-id="8b368-117">Поддержка импорта и экспорта всех меток между файлами appconfig.</span><span class="sxs-lookup"><span data-stu-id="8b368-117">Support import/export of all labels from appconfig to appconfig</span></span>
* <span data-ttu-id="8b368-118">Проверка имен ключей и функций перед настройкой и импортом.</span><span class="sxs-lookup"><span data-stu-id="8b368-118">Validate key and feature names before setting and importing</span></span>
* <span data-ttu-id="8b368-119">Предоставление изменений номера SKU в хранилище конфигураций.</span><span class="sxs-lookup"><span data-stu-id="8b368-119">Expose sku modification for configuration store.</span></span>
* <span data-ttu-id="8b368-120">Новая группа команд для управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="8b368-120">Add command group for managed identity.</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-121">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-121">AppService</span></span>

* <span data-ttu-id="8b368-122">Azure Stack: команды поверхности в профиле 2019-03-01-hybrid</span><span class="sxs-lookup"><span data-stu-id="8b368-122">Azure Stack: surface commands under the profile of 2019-03-01-hybrid</span></span>
* <span data-ttu-id="8b368-123">functionapp: добавлена возможность создавать приложения-функции Java в Linux.</span><span class="sxs-lookup"><span data-stu-id="8b368-123">functionapp: Add ability to create Java function apps in Linux</span></span>

### <a name="arm"></a><span data-ttu-id="8b368-124">ARM</span><span class="sxs-lookup"><span data-stu-id="8b368-124">ARM</span></span>

* <span data-ttu-id="8b368-125">Исправление ошибки 10246: аварийное завершение `az resource tag` в случае, если переданный параметр `--ids` являлся идентификатором группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-125">Fix issue #10246: `az resource tag` crashes when the parameter `--ids` passed in is resource group ID</span></span>
* <span data-ttu-id="8b368-126">Исправление ошибки 11658: команда `az group export` не поддерживала параметры `--query` и `--output`.</span><span class="sxs-lookup"><span data-stu-id="8b368-126">Fix issue #11658: `az group export` command does not support `--query` and `--output` parameters</span></span>
* <span data-ttu-id="8b368-127">Исправление ошибки 10279: код выхода `az group deployment validate` был равен 0, если проверка не пройдена.</span><span class="sxs-lookup"><span data-stu-id="8b368-127">Fix issue #10279: The exit code of `az group deployment validate` is 0 when the verification fails</span></span>
* <span data-ttu-id="8b368-128">Исправление ошибки 9916: улучшено сообщение об ошибке из-за конфликта между тегом и другими условиями фильтра для команды `az resource list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-128">Fix issue #9916: Improve the error message of the conflict between tag and other filter conditions for `az resource list` command</span></span>
* <span data-ttu-id="8b368-129">Добавлен новый параметр `--managed-by` для добавления данных managedBy для команды `az group create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-129">Add new parameter `--managed-by` to support adding managedBy information for command `az group create`</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="8b368-130">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="8b368-130">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="8b368-131">Добавлена подгруппа `monitor` для управления мониторингом Log Analytics в кластере Azure Red Hat OpensShift.</span><span class="sxs-lookup"><span data-stu-id="8b368-131">Add `monitor` subgroup to manage Log Analytics monitoring in Azure Red Hat OpensShift cluster</span></span>

### <a name="botservice"></a><span data-ttu-id="8b368-132">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-132">BotService</span></span>

* <span data-ttu-id="8b368-133">Исправление ошибки 11697: команда `az bot create` не являлась идемпотентной.</span><span class="sxs-lookup"><span data-stu-id="8b368-133">Fix issue #11697: `az bot create` is not idempotent</span></span>
* <span data-ttu-id="8b368-134">Проверки исправления имен изменены для выполнения только в режиме реального времени.</span><span class="sxs-lookup"><span data-stu-id="8b368-134">Change name-correcting tests to run in Live-mode only</span></span>

### <a name="cdn"></a><span data-ttu-id="8b368-135">CDN</span><span class="sxs-lookup"><span data-stu-id="8b368-135">CDN</span></span>

* <span data-ttu-id="8b368-136">Добавлена поддержка функции rulesEngine.</span><span class="sxs-lookup"><span data-stu-id="8b368-136">Add support for rulesEngine feature</span></span>
* <span data-ttu-id="8b368-137">Добавлена новая группа команд cdn endpoint rule для управления правилами.</span><span class="sxs-lookup"><span data-stu-id="8b368-137">Add new commands group 'cdn endpoint rule' to manage rules</span></span>
* <span data-ttu-id="8b368-138">Пакет azure-mgmt-cdn обновлен до версии 4.0.0 для использования API версии 2019-04-15.</span><span class="sxs-lookup"><span data-stu-id="8b368-138">Update azure-mgmt-cdn version to 4.0.0 to use api version 2019-04-15</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="8b368-139">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="8b368-139">Deployment Manager</span></span>

* <span data-ttu-id="8b368-140">Добавлена операция вывода списка всех ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-140">Add list operation for all resources.</span></span>
* <span data-ttu-id="8b368-141">Улучшен ресурс шага для нового типа шага.</span><span class="sxs-lookup"><span data-stu-id="8b368-141">Enhance step resource for new step type.</span></span>
* <span data-ttu-id="8b368-142">Пакет azure-mgmt-deploymentmanager обновлен для использования версии 0.2.0.</span><span class="sxs-lookup"><span data-stu-id="8b368-142">Update azure-mgmt-deploymentmanager package to use version 0.2.0.</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-143">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-143">IoT</span></span>

* <span data-ttu-id="8b368-144">Команды IoT hub Job объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="8b368-144">Deprecate 'IoT hub Job' commands.</span></span>

### <a name="iot-central"></a><span data-ttu-id="8b368-145">IoT Central</span><span class="sxs-lookup"><span data-stu-id="8b368-145">IoT Central</span></span>

* <span data-ttu-id="8b368-146">Добавлена поддержка создания и обновления приложений с новыми SKU: ST0, ST1, ST2.</span><span class="sxs-lookup"><span data-stu-id="8b368-146">Support app creation/update with the new sku name ST0, ST1, ST2.</span></span>

### <a name="key-vault"></a><span data-ttu-id="8b368-147">Key Vault</span><span class="sxs-lookup"><span data-stu-id="8b368-147">Key Vault</span></span>

* <span data-ttu-id="8b368-148">Добавлена новая команда `az keyvault key download` для скачивания ключей.</span><span class="sxs-lookup"><span data-stu-id="8b368-148">Add a new command `az keyvault key download` for downloading keys.</span></span>

### <a name="misc"></a><span data-ttu-id="8b368-149">Разное</span><span class="sxs-lookup"><span data-stu-id="8b368-149">Misc</span></span>

* <span data-ttu-id="8b368-150">Исправление ошибки 6371: поддержка завершения имен файлов и переменных среды в Bash.</span><span class="sxs-lookup"><span data-stu-id="8b368-150">Fix #6371: Support filename and environment variable completion in Bash</span></span>

### <a name="network"></a><span data-ttu-id="8b368-151">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-151">Network</span></span>

* <span data-ttu-id="8b368-152">Исправление ошибки 2092: для команды az network dns record-set add/remove добавлено предупреждение, отображаемое, если набор записей не найден.</span><span class="sxs-lookup"><span data-stu-id="8b368-152">Fix #2092: az network dns record-set add/remove: add warning when record-set is not found.</span></span> <span data-ttu-id="8b368-153">В будущем для подтверждения этого автоматического создания будет добавлен дополнительный аргумент.</span><span class="sxs-lookup"><span data-stu-id="8b368-153">In the future, an extra argument will be supported to confirm this auto creation.</span></span>

### <a name="policy"></a><span data-ttu-id="8b368-154">Политика</span><span class="sxs-lookup"><span data-stu-id="8b368-154">Policy</span></span>

* <span data-ttu-id="8b368-155">Добавлена новая команда `az policy metadata` для получения ресурсов метаданных расширенной политики.</span><span class="sxs-lookup"><span data-stu-id="8b368-155">Add new command `az policy metadata` to retrieve rich policy metadata resources</span></span>
* <span data-ttu-id="8b368-156">`az policy remediation create`: С помощью параметра `--resource-discovery-mode` можно указать, следует ли повторно оценить соответствие перед исправлением.</span><span class="sxs-lookup"><span data-stu-id="8b368-156">`az policy remediation create`: Specify whether compliance should be re-evaluated prior to remediation with the `--resource-discovery-mode` parameter</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-157">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-157">Profile</span></span>

* <span data-ttu-id="8b368-158">`az account get-access-token`: Добавлен параметр `--tenant` для получения маркера для арендатора напрямую, без необходимости указывать подписку.</span><span class="sxs-lookup"><span data-stu-id="8b368-158">`az account get-access-token`: Add `--tenant` parameter to acquire token for the tenant directly, needless to specify a subscription</span></span>

### <a name="rbac"></a><span data-ttu-id="8b368-159">RBAC</span><span class="sxs-lookup"><span data-stu-id="8b368-159">RBAC</span></span>

* <span data-ttu-id="8b368-160">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправление ошибки 11883: `az role assignment create`: пустая область приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="8b368-160">[BREAKING CHANGE] Fix #11883: `az role assignment create`: empty scope will prompt error</span></span>

### <a name="security"></a><span data-ttu-id="8b368-161">безопасность</span><span class="sxs-lookup"><span data-stu-id="8b368-161">Security</span></span>

* <span data-ttu-id="8b368-162">Добавлены новые команды `az atp show` и `az atp update` для просмотра и настройки дополнительных параметров защиты от угроз для учетных записей хранения.</span><span class="sxs-lookup"><span data-stu-id="8b368-162">Add new commands `az atp show` and `az atp update` to view and manage advanced threat protection settings for storage accounts.</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-163">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-163">SQL</span></span>

* <span data-ttu-id="8b368-164">`sql dw create`: параметры `--zone-redundant` и `--read-replica-count` объявлены нерекомендуемыми.</span><span class="sxs-lookup"><span data-stu-id="8b368-164">`sql dw create`: deprecate `--zone-redundant` and `--read-replica-count` parameters.</span></span> <span data-ttu-id="8b368-165">Эти параметры не применяются к хранилищу данных.</span><span class="sxs-lookup"><span data-stu-id="8b368-165">These parameters do not apply to DataWarehouse.</span></span>
* <span data-ttu-id="8b368-166">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql db create`: Значения WideWorldImportersStd и WideWorldImportersFull больше не являются задокументированным допустимыми значениями для команды az sql db create --sample-name.</span><span class="sxs-lookup"><span data-stu-id="8b368-166">[BREAKING CHANGE] `az sql db create`: Remove "WideWorldImportersStd" and "WideWorldImportersFull" as documented allowed values for "az sql db create --sample-name".</span></span> <span data-ttu-id="8b368-167">Эти примеры базы данных всегда будут приводить к сбою создания.</span><span class="sxs-lookup"><span data-stu-id="8b368-167">These sample databases would always cause creation to fail.</span></span>
* <span data-ttu-id="8b368-168">Добавлены новые команды `sql db classification show/list/update/delete` и `sql db classification recommendation list/enable/disable` для управления классификациями конфиденциальности баз данных SQL.</span><span class="sxs-lookup"><span data-stu-id="8b368-168">Add New commands `sql db classification show/list/update/delete` and `sql db classification recommendation list/enable/disable` to manage sensitivity classifications for SQL databases.</span></span>
* <span data-ttu-id="8b368-169">`az sql db audit-policy`: устранены пустые действия аудита и группы.</span><span class="sxs-lookup"><span data-stu-id="8b368-169">`az sql db audit-policy`: Fix for empty audit actions and groups</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-170">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-170">Storage</span></span>

* <span data-ttu-id="8b368-171">Добавлена новая группа команд `az storage share-rm` для использования поставщика ресурсов Microsoft.Storage в операциях управления файловыми ресурсами Azure.</span><span class="sxs-lookup"><span data-stu-id="8b368-171">Add a new command group `az storage share-rm` to use the Microsoft.Storage resource provider for Azure file share management operations.</span></span>
* <span data-ttu-id="8b368-172">Исправление ошибки 11415: ошибка разрешения для `az storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-172">Fix issue #11415: permission error for `az storage blob update`</span></span>
* <span data-ttu-id="8b368-173">Добавлены интеграция AzCopy 10.3.3 и поддержка Win32.</span><span class="sxs-lookup"><span data-stu-id="8b368-173">Integrate Azcopy 10.3.3 and support Win32.</span></span>
* <span data-ttu-id="8b368-174">`az storage copy`: добавлены параметры `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="8b368-174">`az storage copy`: Add `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="8b368-175">`az storage remove`: параметры `--inlcude` и `--exclude` заменены параметрами `--include-path`, `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="8b368-175">`az storage remove`: Change `--inlcude` and `--exclude` parameters to `--include-path`, `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>
* <span data-ttu-id="8b368-176">`az storage sync`: добавлены параметры `--include-pattern`, `--exclude-path` и `--exclude-pattern`.</span><span class="sxs-lookup"><span data-stu-id="8b368-176">`az storage sync`: Add `--include-pattern`, `--exclude-path` and`--exclude-pattern` parameters</span></span>

### <a name="servicefabric"></a><span data-ttu-id="8b368-177">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8b368-177">ServiceFabric</span></span>

* <span data-ttu-id="8b368-178">Добавлены новые команды для управления приложениями и службами.</span><span class="sxs-lookup"><span data-stu-id="8b368-178">Add new commands to manage appliaction and services.</span></span>

## <a name="january-13-2020"></a><span data-ttu-id="8b368-179">13 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-179">January 13, 2020</span></span>

<span data-ttu-id="8b368-180">Версия 2.0.80</span><span class="sxs-lookup"><span data-stu-id="8b368-180">Version 2.0.80</span></span>

### <a name="compute"></a><span data-ttu-id="8b368-181">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="8b368-181">Compute</span></span>

* <span data-ttu-id="8b368-182">Обновление диска: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="8b368-182">disk update: Add --disk-encryption-set and --encryption-type</span></span>
* <span data-ttu-id="8b368-183">Создание и обновление моментального снимка: добавлены параметры --disk-encryption-set и --encryption-type.</span><span class="sxs-lookup"><span data-stu-id="8b368-183">snapshot create/update: Add --disk-encryption-set and --encryption-type</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-184">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-184">Storage</span></span>

* <span data-ttu-id="8b368-185">Обновление azure-mgmt-storage до версии 7.1.0</span><span class="sxs-lookup"><span data-stu-id="8b368-185">Upgrade azure-mgmt-storage version to 7.1.0</span></span>
* <span data-ttu-id="8b368-186">`az storage account create`: добавлены параметры `--encryption-key-type-for-table` и `--encryption-key-type-for-queue` для включения поддержки службы шифрования таблиц и очередей.</span><span class="sxs-lookup"><span data-stu-id="8b368-186">`az storage account create`: Add `--encryption-key-type-for-table` and `--encryption-key-type-for-queue` to support Table and Queue Encryption Service</span></span>

## <a name="january-07-2020"></a><span data-ttu-id="8b368-187">7 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-187">January 07, 2020</span></span>

<span data-ttu-id="8b368-188">Версия 2.0.79</span><span class="sxs-lookup"><span data-stu-id="8b368-188">Version 2.0.79</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-189">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-189">ACR</span></span>

* <span data-ttu-id="8b368-190">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --os для команд acr build, acr task create/update, acr run и acr pack.</span><span class="sxs-lookup"><span data-stu-id="8b368-190">[BREAKING CHANGE] Remove '--os' parameter for 'acr build', 'acr task create/update', 'acr run', and 'acr pack'.</span></span> <span data-ttu-id="8b368-191">Вместо этого используется параметр --platform.</span><span class="sxs-lookup"><span data-stu-id="8b368-191">Use '--platform' instead.</span></span>

### <a name="appconfig"></a><span data-ttu-id="8b368-192">AppConfig</span><span class="sxs-lookup"><span data-stu-id="8b368-192">AppConfig</span></span>

* <span data-ttu-id="8b368-193">Добавлена поддержка импорта и экспорта флагов функций.</span><span class="sxs-lookup"><span data-stu-id="8b368-193">Add support for importing/exporting feature flags</span></span>
* <span data-ttu-id="8b368-194">Добавлена новая команда az appconfig kv set-keyvault для создания ссылки на хранилище ключей.</span><span class="sxs-lookup"><span data-stu-id="8b368-194">Add new command 'az appconfig kv set-keyvault' for creating keyvault reference</span></span>
* <span data-ttu-id="8b368-195">Добавлена поддержка различных соглашений об именовании при экспорте флагов функций в файл.</span><span class="sxs-lookup"><span data-stu-id="8b368-195">Support various naming conventions when exporting feature flags to file</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-196">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-196">AppService</span></span>

* <span data-ttu-id="8b368-197">Устранена проблема № 7154: обновлена документация по команде <> — теперь в ней используются обратные, а не одинарные кавычки.</span><span class="sxs-lookup"><span data-stu-id="8b368-197">Fix issue #7154: Updating documentation for command <> to use back ticks instead of single quotes</span></span>
* <span data-ttu-id="8b368-198">Устранена проблема № 11287 (webapp up): по умолчанию для приложения, созданного с использованием этого флага, должен быть включен SSL.</span><span class="sxs-lookup"><span data-stu-id="8b368-198">Fix issue #11287: webapp up: By default make the app created using up 'should be 'SSL enabled'</span></span>
* <span data-ttu-id="8b368-199">Устранена проблема № 11592: добавлен флаг az webapp up для статических сайтов HTML.</span><span class="sxs-lookup"><span data-stu-id="8b368-199">Fix issue #11592: Add az webapp up flag for html static sites</span></span>

### <a name="arm"></a><span data-ttu-id="8b368-200">ARM</span><span class="sxs-lookup"><span data-stu-id="8b368-200">ARM</span></span>

* <span data-ttu-id="8b368-201">Исправлена ошибка с командой `az resource tag`: невозможно было обновить теги хранилища Служб восстановления.</span><span class="sxs-lookup"><span data-stu-id="8b368-201">Fix `az resource tag`: Recovery Services Vault tags cannot be updated</span></span>

### <a name="backup"></a><span data-ttu-id="8b368-202">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="8b368-202">Backup</span></span>

* <span data-ttu-id="8b368-203">Добавлена новая команда backup protection undelete для включения функции обратимого удаления рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="8b368-203">Added new command 'backup protection undelete' to enable soft-delete feature for IaasVM workload</span></span>
* <span data-ttu-id="8b368-204">Добавлен новый параметр --soft-delete-feature-state для команды set backup-properties.</span><span class="sxs-lookup"><span data-stu-id="8b368-204">Added new parameter '--soft-delete-feature-state' to set backup-properties command</span></span>
* <span data-ttu-id="8b368-205">Добавлена поддержка исключения диска для рабочей нагрузки IaasVM.</span><span class="sxs-lookup"><span data-stu-id="8b368-205">Added disk exclusion support for IaasVM workload</span></span>

### <a name="compute"></a><span data-ttu-id="8b368-206">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="8b368-206">Compute</span></span>

* <span data-ttu-id="8b368-207">Исправлен сбой `vm create` в профиле Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8b368-207">Fix `vm create` failure in Azure Stack profile.</span></span>
* <span data-ttu-id="8b368-208">Добавлена поддержка определений списков и метрик запросов для виртуальной машины (vm monitor metrics tail/list-definitions).</span><span class="sxs-lookup"><span data-stu-id="8b368-208">vm monitor metrics tail/list-definitions: support query metric and list definitions for a vm.</span></span>
* <span data-ttu-id="8b368-209">Добавлено новое действия повторного применения команды az vm</span><span class="sxs-lookup"><span data-stu-id="8b368-209">Add new reapply command action for az vm</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8b368-210">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b368-210">HDInsight</span></span>

* <span data-ttu-id="8b368-211">Включена поддержка создания кластера Kafka с помощью прокси-сервера Kafka RESTful.</span><span class="sxs-lookup"><span data-stu-id="8b368-211">Support for creating a Kafka cluster with Kafka Rest Proxy</span></span>
* <span data-ttu-id="8b368-212">Обновление azure-mgmt-hdinsight до версии 1.3.0</span><span class="sxs-lookup"><span data-stu-id="8b368-212">Upgrade azure-mgmt-hdinsight to 1.3.0</span></span>

### <a name="misc"></a><span data-ttu-id="8b368-213">Прочее</span><span class="sxs-lookup"><span data-stu-id="8b368-213">Misc.</span></span>

* <span data-ttu-id="8b368-214">Добавлена команда `az version show` предварительного просмотра для отображения версий модулей и расширений Azure CLI в формате JSON по умолчанию или в формате, настроенном с помощью параметра --output</span><span class="sxs-lookup"><span data-stu-id="8b368-214">Add preview command `az version show` to show the versions of Azure CLI modules and extensions in JSON format by default or format configured by --output</span></span>

### <a name="event-hubs"></a><span data-ttu-id="8b368-215">Центры событий</span><span class="sxs-lookup"><span data-stu-id="8b368-215">Event Hubs</span></span>

* <span data-ttu-id="8b368-216">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az eventhubs eventhub update и az eventhubs eventhub create.</span><span class="sxs-lookup"><span data-stu-id="8b368-216">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az eventhubs eventhub update' and 'az eventhubs eventhub create'.</span></span> <span data-ttu-id="8b368-217">Данный параметр недопустим для сущностей концентратора событий.</span><span class="sxs-lookup"><span data-stu-id="8b368-217">This option is not valid for Event Hub entities.</span></span>

### <a name="service-bus"></a><span data-ttu-id="8b368-218">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="8b368-218">Service Bus</span></span>

* <span data-ttu-id="8b368-219">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр состояния ReceiveDisabled из команд az servicebus topic create, az servicebus topic update, az servicebus queue create и az servicebus queue update.</span><span class="sxs-lookup"><span data-stu-id="8b368-219">[BREAKING CHANGE] Remove 'ReceiveDisabled' status option from command 'az servicebus topic create', 'az servicebus topic update', 'az servicebus queue create', and 'az servicebus queue update'.</span></span> <span data-ttu-id="8b368-220">Этот параметр является недопустимым для разделов и очередей служебной шины.</span><span class="sxs-lookup"><span data-stu-id="8b368-220">This option is not valid for Service Bus topics and queues.</span></span>

### <a name="rbac"></a><span data-ttu-id="8b368-221">RBAC</span><span class="sxs-lookup"><span data-stu-id="8b368-221">RBAC</span></span>

* <span data-ttu-id="8b368-222">Устранена проблема № 11712: команда `az ad app/sp show` не возвращала код выхода 3, если приложение или субъект-служба не существует.</span><span class="sxs-lookup"><span data-stu-id="8b368-222">Fix #11712: `az ad app/sp show` does not return exit code 3 when the application or service principal does not exist</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-223">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-223">Storage</span></span>

* <span data-ttu-id="8b368-224">`az storage account create`: удален флаг предварительного просмотра для параметра --enable-hierarchical-namespace.</span><span class="sxs-lookup"><span data-stu-id="8b368-224">`az storage account create`: Remove preview flag for --enable-hierarchical-namespace parameter</span></span>
* <span data-ttu-id="8b368-225">Хранилище azure-mgmt-storage обновлено до версии 7.0.0 для использования API версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-225">Update azure-mgmt-storage version to 7.0.0 to use api version 2019-06-01</span></span>
* <span data-ttu-id="8b368-226">Добавлены новые параметры (`--enable-delete-retention` и `--delete-retention-days`) для поддержки управления политикой хранения удаленных свойств службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="8b368-226">Add new parameters `--enable-delete-retention` and `--delete-retention-days` to support managing delete retention policy for storage account blob-service-properties.</span></span>

## <a name="december-17-2019"></a><span data-ttu-id="8b368-227">17 декабря 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-227">December 17, 2019</span></span>

<span data-ttu-id="8b368-228">2.0.78</span><span class="sxs-lookup"><span data-stu-id="8b368-228">2.0.78</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-229">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-229">ACR</span></span>

* <span data-ttu-id="8b368-230">Добавлена поддержка локального контекста во время выполнения задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="8b368-230">Added support Local context in acr task run</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-231">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-231">ACS</span></span>

* <span data-ttu-id="8b368-232">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде az openshift create параметр `--workspace-resource-id` переименован на `--workspace-id`.</span><span class="sxs-lookup"><span data-stu-id="8b368-232">[BREAKING CHANGE]az openshift create: rename `--workspace-resource-id` to `--workspace-id`.</span></span>

### <a name="ams"></a><span data-ttu-id="8b368-233">AMS</span><span class="sxs-lookup"><span data-stu-id="8b368-233">AMS</span></span>

* <span data-ttu-id="8b368-234">Команды show обновлены для возвращения ответа 3, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="8b368-234">Updated show commands to return 3 when resource not found</span></span>

### <a name="appconfig"></a><span data-ttu-id="8b368-235">AppConfig</span><span class="sxs-lookup"><span data-stu-id="8b368-235">AppConfig</span></span>

* <span data-ttu-id="8b368-236">Исправлена ошибка, возникающая при добавлении api-version в URL-адрес запроса.</span><span class="sxs-lookup"><span data-stu-id="8b368-236">Fixed bug when appending api-version to request url.</span></span> <span data-ttu-id="8b368-237">Имеющееся решение не работает с разбивкой на страницы.</span><span class="sxs-lookup"><span data-stu-id="8b368-237">The existing solution doesn't work with pagination.</span></span>
* <span data-ttu-id="8b368-238">Добавлена поддержка отображения языков, кроме английского, так как наша внутренняя служба поддерживает Юникод для глобализации.</span><span class="sxs-lookup"><span data-stu-id="8b368-238">Added support for showing languages besides English as our backend service support unicode for globalization.</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-239">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-239">AppService</span></span>

* <span data-ttu-id="8b368-240">Устранена проблема № 11217 (webapp): теперь команда az webapp config ssl upload поддерживает параметр слота.</span><span class="sxs-lookup"><span data-stu-id="8b368-240">Fixed issue #11217: webapp: az webapp config ssl upload should support slot parameter</span></span>
* <span data-ttu-id="8b368-241">Устранена проблема № 10965. Ошибка: Имя не может быть пустым.</span><span class="sxs-lookup"><span data-stu-id="8b368-241">Fixed issue #10965: Error: Name cannot be empty.</span></span> <span data-ttu-id="8b368-242">Разрешено удаление по IP-адресу и подсети.</span><span class="sxs-lookup"><span data-stu-id="8b368-242">Allow remove by ip_address and subnet</span></span>
* <span data-ttu-id="8b368-243">Добавлена поддержка импорта сертификатов из хранилища ключей: `az webapp config ssl import`</span><span class="sxs-lookup"><span data-stu-id="8b368-243">Added support for importing certificates from Key Vault `az webapp config ssl import`</span></span>

### <a name="arm"></a><span data-ttu-id="8b368-244">ARM</span><span class="sxs-lookup"><span data-stu-id="8b368-244">ARM</span></span>

* <span data-ttu-id="8b368-245">Обновлен пакет ресурсов azure-mgmt-resource для использования версии 6.0.0</span><span class="sxs-lookup"><span data-stu-id="8b368-245">Updated azure-mgmt-resource package to use 6.0.0</span></span>
* <span data-ttu-id="8b368-246">Добавлена межклиентская поддержка команды `az group deployment create` путем добавления нового параметра `--aux-subs`</span><span class="sxs-lookup"><span data-stu-id="8b368-246">Cross Tenant Support for `az group deployment create` command by adding new parameter `--aux-subs`</span></span>
* <span data-ttu-id="8b368-247">Добавлен новый параметр `--metadata` для поддержки добавления метаданных определений наборов политик.</span><span class="sxs-lookup"><span data-stu-id="8b368-247">Added new parameter `--metadata` to support adding metadata information for policy set definitions.</span></span>

### <a name="backup"></a><span data-ttu-id="8b368-248">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="8b368-248">Backup</span></span>

* <span data-ttu-id="8b368-249">Добавлена поддержка резервного копирования для рабочей нагрузки SQL и SAP HANA.</span><span class="sxs-lookup"><span data-stu-id="8b368-249">Added Backup support for SQL and SAP Hana workload.</span></span>

### <a name="botservice"></a><span data-ttu-id="8b368-250">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-250">BotService</span></span>

* <span data-ttu-id="8b368-251">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг --version из предварительной версии команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="8b368-251">[Breaking change] Remove '--version' flag from preview command 'az bot create'.</span></span> <span data-ttu-id="8b368-252">Поддерживаются только боты пакетов SDK версии 4.</span><span class="sxs-lookup"><span data-stu-id="8b368-252">Only v4 SDK bots are supported.</span></span>
* <span data-ttu-id="8b368-253">Добавлена проверка доступности имени для команды az bot create.</span><span class="sxs-lookup"><span data-stu-id="8b368-253">Added name availability check for 'az bot create'.</span></span>
* <span data-ttu-id="8b368-254">Добавлена поддержка обновления URL-адреса значка для бота с помощью команды az bot update.</span><span class="sxs-lookup"><span data-stu-id="8b368-254">Added support for updating the icon URL for a bot via 'az bot update'.</span></span>
* <span data-ttu-id="8b368-255">Добавлена поддержка обновления канала Direct Line с помощью команды az bot directline update.</span><span class="sxs-lookup"><span data-stu-id="8b368-255">Added support for updating a Direct Line channel via 'az bot directline update'.</span></span>
* <span data-ttu-id="8b368-256">Добавлена поддержка флага --enable-enhanced-auth в команде az bot directline create.</span><span class="sxs-lookup"><span data-stu-id="8b368-256">Added '--enable-enhanced-auth' flag support to 'az bot directline create'.</span></span>
* <span data-ttu-id="8b368-257">Следующие группы команд предоставляются в общедоступной, а не в предварительной версии: az bot authsetting.</span><span class="sxs-lookup"><span data-stu-id="8b368-257">The following command groups are GA and not in preview: 'az bot authsetting'.</span></span>
* <span data-ttu-id="8b368-258">Следующие команды в az bot предоставляются в общедоступной, а не в предварительной версии: create, prepare-deploy, show, delete и update.</span><span class="sxs-lookup"><span data-stu-id="8b368-258">The following commands in 'az bot' are GA and not in preview: 'create', 'prepare-deploy', 'show', 'delete', 'update'.</span></span>
* <span data-ttu-id="8b368-259">Устранена проблема с командой az bot prepare-deploy, которая изменяла значение параметра --proj-file-path на нижний регистр (например, с Test.csproj на test.csproj).</span><span class="sxs-lookup"><span data-stu-id="8b368-259">Fixed 'az bot prepare-deploy' changing '--proj-file-path' value to lower case (e.g. "Test.csproj" to "test.csproj").</span></span>

### <a name="compute"></a><span data-ttu-id="8b368-260">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="8b368-260">Compute</span></span>

* <span data-ttu-id="8b368-261">vmss create/update: добавлен параметр --scale-on-policy, который определяет, какие виртуальные машины выбираются для удаления при масштабировании VMSS.</span><span class="sxs-lookup"><span data-stu-id="8b368-261">vmss create/update: Added --scale-in-policy, which decides which virtual machines are chosen for removal when a VMSS is scaled-in.</span></span>
* <span data-ttu-id="8b368-262">vm/vmss update: добавлен параметр --priority.</span><span class="sxs-lookup"><span data-stu-id="8b368-262">vm/vmss update: Added --priority.</span></span>
* <span data-ttu-id="8b368-263">vm/vmss update: добавлен параметр --max-price.</span><span class="sxs-lookup"><span data-stu-id="8b368-263">vm/vmss update: Added --max-price.</span></span>
* <span data-ttu-id="8b368-264">Добавлена группа команд для шифрования дисков (create, show, update, delete, list).</span><span class="sxs-lookup"><span data-stu-id="8b368-264">Added disk-encryption-set command group (create, show, update, delete, list).</span></span>
* <span data-ttu-id="8b368-265">disk create: добавлены параметры --encryption-type и --disk-encryption-set.</span><span class="sxs-lookup"><span data-stu-id="8b368-265">disk create: Added --encryption-type and --disk-encryption-set.</span></span>
* <span data-ttu-id="8b368-266">vm/vmss create. Добавлены параметры --os-disk-encryption-set и --data-disk-encryption-sets.</span><span class="sxs-lookup"><span data-stu-id="8b368-266">vm/vmss create: Added --os-disk-encryption-set and --data-disk-encryption-sets.</span></span>

### <a name="core"></a><span data-ttu-id="8b368-267">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-267">Core</span></span>

* <span data-ttu-id="8b368-268">Удалена поддержка Python версии 3.4.</span><span class="sxs-lookup"><span data-stu-id="8b368-268">Removed support for Python 3.4</span></span>
* <span data-ttu-id="8b368-269">Подключение к опросу HaTS в нескольких командах.</span><span class="sxs-lookup"><span data-stu-id="8b368-269">Plug in HaTS survey in multiple commands</span></span>

### <a name="dls"></a><span data-ttu-id="8b368-270">DLS</span><span class="sxs-lookup"><span data-stu-id="8b368-270">DLS</span></span>

* <span data-ttu-id="8b368-271">Обновлена версия пакета SDK для ADLS (0.0.48).</span><span class="sxs-lookup"><span data-stu-id="8b368-271">Updated ADLS sdk version (0.0.48).</span></span>

### <a name="install"></a><span data-ttu-id="8b368-272">Установка</span><span class="sxs-lookup"><span data-stu-id="8b368-272">Install</span></span>

* <span data-ttu-id="8b368-273">Добавлена поддержка установки скриптов Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="8b368-273">Install script support python 3.8</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-274">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-274">IOT</span></span>

* <span data-ttu-id="8b368-275">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр --failover-region из команды manual-failover.</span><span class="sxs-lookup"><span data-stu-id="8b368-275">[BREAKING CHANGE] Removed --failover-region parameter from manual-failover.</span></span> <span data-ttu-id="8b368-276">Теперь она будет выполнять отработку отказа в назначенный геопарный дополнительный регион.</span><span class="sxs-lookup"><span data-stu-id="8b368-276">Now it will failover to assigned geo-paired secondary region.</span></span>

### <a name="key-vault"></a><span data-ttu-id="8b368-277">Key Vault</span><span class="sxs-lookup"><span data-stu-id="8b368-277">Key Vault</span></span>

* <span data-ttu-id="8b368-278">Устранена проблема № 8095: (`az keyvault storage remove`): улучшено справочное сообщение.</span><span class="sxs-lookup"><span data-stu-id="8b368-278">Fixed #8095: `az keyvault storage remove`: improve the help message</span></span>
* <span data-ttu-id="8b368-279">Устранена проблема № 8921 (`az keyvault key/secret/certificate list/list-deleted/list-versions`): исправлена ошибка проверки в параметре `--maxresults`.</span><span class="sxs-lookup"><span data-stu-id="8b368-279">Fixed #8921: `az keyvault key/secret/certificate list/list-deleted/list-versions`: fix the validation bug on parameter `--maxresults`</span></span>
* <span data-ttu-id="8b368-280">Устранена проблема № 10512 (`az keyvault set-policy`): улучшено сообщение об ошибке, возвращаемое, если не указан ни один из параметров `--object-id`, `--spn` или `--upn`.</span><span class="sxs-lookup"><span data-stu-id="8b368-280">Fixed #10512: `az keyvault set-policy`: improve the error message when none of `--object-id`, `--spn` or `--upn` is specified</span></span>
* <span data-ttu-id="8b368-281">Устранена проблема № 10846 (`az keyvault secret show-deleted`): при указании значения `--id` значение `--name/-n` не требовалось.</span><span class="sxs-lookup"><span data-stu-id="8b368-281">Fixed #10846: `az keyvault secret show-deleted`: when `--id` is specified, `--name/-n` is not required</span></span>
* <span data-ttu-id="8b368-282">Устранена проблема № 11084: (`az keyvault secret download`): улучшено справочное сообщение параметра `--encoding`.</span><span class="sxs-lookup"><span data-stu-id="8b368-282">Fixed #11084: `az keyvault secret download`: improve the help message of parameter `--encoding`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-283">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-283">Network</span></span>

* <span data-ttu-id="8b368-284">az network application-gateway probe: добавлена поддержка параметра --port, позволяющего указать порт, который используется для проверки внутренних серверов при создании и обновлении.</span><span class="sxs-lookup"><span data-stu-id="8b368-284">az network application-gateway probe: Added support --port option to specify a port for probing backend servers when create and update</span></span>
* <span data-ttu-id="8b368-285">az network application-gateway url-path-map create/update: исправлена ошибка с `--waf-policy`.</span><span class="sxs-lookup"><span data-stu-id="8b368-285">az network application-gateway url-path-map create/update: bug fix for `--waf-policy`</span></span>
* <span data-ttu-id="8b368-286">az network application-gateway: добавлена поддержка параметра `--rewrite-rule-set`.</span><span class="sxs-lookup"><span data-stu-id="8b368-286">az network application-gateway: Added support `--rewrite-rule-set`</span></span>
* <span data-ttu-id="8b368-287">az network list-service-aliases: добавлена поддержка перечисления псевдонимов служб, которые можно использовать для политик конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-287">az network list-service-aliases: Added support list service aliases which can be used for Service Endpoint Policies</span></span>
* <span data-ttu-id="8b368-288">az network dns zone import: добавлена поддержка символа .@ в имени записи.</span><span class="sxs-lookup"><span data-stu-id="8b368-288">az network dns zone import: Added support .@ in record name</span></span>

### <a name="packaging"></a><span data-ttu-id="8b368-289">Упаковка</span><span class="sxs-lookup"><span data-stu-id="8b368-289">Packaging</span></span>

* <span data-ttu-id="8b368-290">Снова добавлены сборки Edge для установки PIP.</span><span class="sxs-lookup"><span data-stu-id="8b368-290">Added back edge builds for pip install</span></span>
* <span data-ttu-id="8b368-291">Добавлен пакет Ubuntu eoan.</span><span class="sxs-lookup"><span data-stu-id="8b368-291">Added Ubuntu eoan package</span></span>

### <a name="policy"></a><span data-ttu-id="8b368-292">Политика</span><span class="sxs-lookup"><span data-stu-id="8b368-292">Policy</span></span>

* <span data-ttu-id="8b368-293">Добавлена поддержка API Политики версии 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-293">Added support for Policy API version 2019-09-01.</span></span>
* <span data-ttu-id="8b368-294">az policy set-definition: добавлена поддержка группирования в определениях наборов политик с помощью параметра `--definition-groups`.</span><span class="sxs-lookup"><span data-stu-id="8b368-294">az policy set-definition: Added support grouping within policy set definitions with `--definition-groups` parameter</span></span>

### <a name="redis"></a><span data-ttu-id="8b368-295">Redis</span><span class="sxs-lookup"><span data-stu-id="8b368-295">Redis</span></span>

* <span data-ttu-id="8b368-296">В команду `az redis create` добавлена предварительная версия параметра `--replicas-per-master`.</span><span class="sxs-lookup"><span data-stu-id="8b368-296">Added preview param `--replicas-per-master` to `az redis create` command</span></span>
* <span data-ttu-id="8b368-297">Обновлена версия azure-mgmt-redis с 6.0.0 на 7.0.0 RC1.</span><span class="sxs-lookup"><span data-stu-id="8b368-297">Updated azure-mgmt-redis from 6.0.0 to 7.0.0rc1</span></span>

### <a name="servicefabric"></a><span data-ttu-id="8b368-298">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8b368-298">ServiceFabric</span></span>

* <span data-ttu-id="8b368-299">Исправлена логика добавления типа узла, а также устранена проблема № 10963: при добавлении нового типа узла с уровнем устойчивости Gold возникала ошибка CLI.</span><span class="sxs-lookup"><span data-stu-id="8b368-299">Fixed in node-type add logic including #10963: Adding new node type with durability level Gold will always throw CLI error</span></span>
* <span data-ttu-id="8b368-300">Обновлена версия параметра ServiceFabricNodeVmExt до 1.1 в шаблоне создания.</span><span class="sxs-lookup"><span data-stu-id="8b368-300">Updated ServiceFabricNodeVmExt version to 1.1 in creation template</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-301">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-301">SQL</span></span>

* <span data-ttu-id="8b368-302">В команды create и update базы данных SQL добавлены параметры --read-scale и --read-replicas для поддержки управления масштабированием операций чтения.</span><span class="sxs-lookup"><span data-stu-id="8b368-302">Added "--read-scale" and "--read-replicas" parameters to sql db create and update commands, to support read scale management.</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-303">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-303">Storage</span></span>

* <span data-ttu-id="8b368-304">Выпущена общедоступная версия больших файловых ресурсов для команды создания и обновления учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="8b368-304">GA Release Large File Shares property for storage account create and update command</span></span>
* <span data-ttu-id="8b368-305">Выпущена общедоступная версия поддержки маркера SAS для делегирования пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b368-305">GA Release User Delegation SAS token Support</span></span>
* <span data-ttu-id="8b368-306">Добавлены новые команды (`az storage account blob-service-properties show` и `az storage account blob-service-properties update --enable-change-feed`) для управления свойствами службы BLOB-объектов учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="8b368-306">Added new commands `az storage account blob-service-properties show` and `az storage account blob-service-properties update --enable-change-feed` to manage blob service properties for storage account.</span></span>
* <span data-ttu-id="8b368-307">[ОЖИДАЕТСЯ КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] `az storage copy`: символ `*` больше не поддерживается в качестве подстановочного знака в URL-адресе. Тем не менее новые параметры--include-pattern и--exclude-pattern будут добавлены с поддержкой подстановочных знаков `*`.</span><span class="sxs-lookup"><span data-stu-id="8b368-307">[COMING BREAKING CHANGE] `az storage copy`: `*` character is no longer supported as a wildcard in URL, but new parameters --include-pattern and --exclude-pattern will be added with `*` wildcard support.</span></span>
* <span data-ttu-id="8b368-308">Устранена проблема № 11043: добавлена поддержка удаления всего контейнера или общего ресурса в команде `az storage remove`.</span><span class="sxs-lookup"><span data-stu-id="8b368-308">Fixed issue #11043: Added support to remove whole container/share in `az storage remove` command</span></span>

## <a name="november-26-2019"></a><span data-ttu-id="8b368-309">26 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-309">November 26, 2019</span></span>

<span data-ttu-id="8b368-310">Версия 2.0.77</span><span class="sxs-lookup"><span data-stu-id="8b368-310">Version 2.0.77</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-311">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-311">ACR</span></span>

* <span data-ttu-id="8b368-312">Параметр `--branch`, используемый при обновлении или создании задачи ACR, объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="8b368-312">Deprecated parameter `--branch` from acr task create/update</span></span>

### <a name="azure-red-hat-openshift"></a><span data-ttu-id="8b368-313">Azure Red Hat OpenShift</span><span class="sxs-lookup"><span data-stu-id="8b368-313">Azure Red Hat OpenShift</span></span>

* <span data-ttu-id="8b368-314">Добавлен флаг `--workspace-resource-id` для создания кластера Azure Red Hat Openshift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="8b368-314">Added `--workspace-resource-id` flag to allow creation of Azure Red Hat Openshift cluster with monitoring</span></span>
* <span data-ttu-id="8b368-315">Добавлен флаг `monitor_profile` для создания кластера Azure Red Hat OpenShift с мониторингом.</span><span class="sxs-lookup"><span data-stu-id="8b368-315">Added `monitor_profile` to create Azure Red Hat OpenShift cluster with monitoring</span></span>

### <a name="aks"></a><span data-ttu-id="8b368-316">AKS</span><span class="sxs-lookup"><span data-stu-id="8b368-316">AKS</span></span>

* <span data-ttu-id="8b368-317">Включена поддержка операции смены сертификата кластера с использованием команды az aks rotate-certs.</span><span class="sxs-lookup"><span data-stu-id="8b368-317">Added support cluster certificate rotation operation using "az aks rotate-certs".</span></span>

### <a name="appconfig"></a><span data-ttu-id="8b368-318">AppConfig</span><span class="sxs-lookup"><span data-stu-id="8b368-318">AppConfig</span></span>

* <span data-ttu-id="8b368-319">Включена поддержка использования символа ":" для разделителя `as az appconfig kv import`.</span><span class="sxs-lookup"><span data-stu-id="8b368-319">Added support for using ":" for `as az appconfig kv import` separator</span></span>
* <span data-ttu-id="8b368-320">Исправлена проблема с перечислением значений ключей с несколькими метками, включая метку NULL.</span><span class="sxs-lookup"><span data-stu-id="8b368-320">Fixed issue for listing key values with multiple labels including null label.</span></span> 
* <span data-ttu-id="8b368-321">Обновлен пакет SDK для плоскости управления, azure-mgmt-appconfiguration, до версии 0.3.0.</span><span class="sxs-lookup"><span data-stu-id="8b368-321">Updated management plane sdk, azure-mgmt-appconfiguration, to version 0.3.0.</span></span> 

### <a name="appservice"></a><span data-ttu-id="8b368-322">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-322">AppService</span></span>

* <span data-ttu-id="8b368-323">Исправлена ошибка № 11100. Использование AttributeError для az webapp up при создании плана службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-323">Fixed issue #11100: AttributeError for az webapp up when create service plan</span></span>
* <span data-ttu-id="8b368-324">az webapp up. При принудительном создании или развертывании сайта для поддерживаемых языков значения по умолчанию не используются.</span><span class="sxs-lookup"><span data-stu-id="8b368-324">az webapp up: Forcing the creation or deployment to a site for supported languages, no defaults used.</span></span>
* <span data-ttu-id="8b368-325">Включена поддержка Среды службы приложений: az appservice ase show | list | list-addresses | list-plans | create | update | delete.</span><span class="sxs-lookup"><span data-stu-id="8b368-325">Added support for App Service Environment: az appservice ase show | list | list-addresses | list-plans | create | update | delete</span></span>

### <a name="backup"></a><span data-ttu-id="8b368-326">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="8b368-326">Backup</span></span>

* <span data-ttu-id="8b368-327">Исправлена проблема в команде az backup policy list-associated-items.</span><span class="sxs-lookup"><span data-stu-id="8b368-327">Fixed issue in az backup policy list-associated-items.</span></span> <span data-ttu-id="8b368-328">Добавлен необязательный параметр BackupManagementType.</span><span class="sxs-lookup"><span data-stu-id="8b368-328">Added optional BackupManagementType parameter.</span></span>

### <a name="compute"></a><span data-ttu-id="8b368-329">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="8b368-329">Compute</span></span>

* <span data-ttu-id="8b368-330">Обновлена версия API вычислений, дисков, моментальных снимков до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-330">Upgraded API version of compute, disks, snapshots to 2019-07-01</span></span>
* <span data-ttu-id="8b368-331">vmss create. Улучшение для --orchestration-mode.</span><span class="sxs-lookup"><span data-stu-id="8b368-331">vmss create: Improvement for --orchestration-mode</span></span>
* <span data-ttu-id="8b368-332">sig image-definition create. Добавлен параметр --os-state для указания того, являются ли виртуальные машины, созданные в этом образе, универсальными или специализированными.</span><span class="sxs-lookup"><span data-stu-id="8b368-332">sig image-definition create: Added --os-state to allow specifying whether the virtual machines created under this image are 'Generalized' or 'Specialized'</span></span>
* <span data-ttu-id="8b368-333">sig image-definition create. Добавлен параметр --hyper-v-generation для указания создания гипервизора.</span><span class="sxs-lookup"><span data-stu-id="8b368-333">sig image-definition create: Added --hyper-v-generation to allow specifying the hypervisor generation</span></span>
* <span data-ttu-id="8b368-334">sig image-version create. Включена поддержка параметров --os-snapshot и --data-snapshots.</span><span class="sxs-lookup"><span data-stu-id="8b368-334">sig image-version create: Added support --os-snapshot and --data-snapshots</span></span>
* <span data-ttu-id="8b368-335">image create. Включена поддержка параметра --data-disk-caching для указания параметра кэширования для дисков данных.</span><span class="sxs-lookup"><span data-stu-id="8b368-335">image create: Added --data-disk-caching to allow specifying caching setting of data disks</span></span>
* <span data-ttu-id="8b368-336">Обновлена версия пакета SDK для вычислений Python до 10.0.0.</span><span class="sxs-lookup"><span data-stu-id="8b368-336">Upgraded Python Compute SDK to 10.0.0</span></span>
* <span data-ttu-id="8b368-337">vm/vmss create. Добавлен фрагмент Spot в свойство перечисления Priority.</span><span class="sxs-lookup"><span data-stu-id="8b368-337">vm/vmss create: Added 'Spot' to 'Priority' enum property</span></span>
* <span data-ttu-id="8b368-338">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименование параметра --max-billing в --max-price для виртуальных машин и Масштабируемых наборов виртуальных машин в соответствии с командлетами Swagger и PowerShell.</span><span class="sxs-lookup"><span data-stu-id="8b368-338">[Breaking change] Renamed '--max-billing' parameter to '--max-price', for both VM and VMSS, to be consistent with Swagger and Powershell cmdlets</span></span>
* <span data-ttu-id="8b368-339">vm monitor log show. Включена поддержка запроса журналов в связанной рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="8b368-339">vm monitor log show: Added support for querying log over linked log analytics workspace.</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-340">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-340">IOT</span></span>

* <span data-ttu-id="8b368-341">Исправление № 2531. Добавлены вспомогательные аргументы для обновления концентратора.</span><span class="sxs-lookup"><span data-stu-id="8b368-341">Fix #2531: Added convenience arguments for hub update.</span></span>
* <span data-ttu-id="8b368-342">Исправление № 8323. Добавлены недостающие параметры для создания пользовательской конечной точки хранилища.</span><span class="sxs-lookup"><span data-stu-id="8b368-342">Fix #8323: Added missing parameters to create storage custom endpoint.</span></span>
* <span data-ttu-id="8b368-343">Исправлена ошибка регрессии. Отменены изменения, переопределяющие конечную точку хранилища по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-343">Fix regression bug: Reverted the changes which overrides the default storage endpoint.</span></span>

### <a name="key-vault"></a><span data-ttu-id="8b368-344">Key Vault</span><span class="sxs-lookup"><span data-stu-id="8b368-344">Key Vault</span></span>

* <span data-ttu-id="8b368-345">Исправление № 11121. При использовании `az keyvault certificate list` для передачи `--include-pending` теперь не требуется значение `true` или `false`.</span><span class="sxs-lookup"><span data-stu-id="8b368-345">Fixed #11121: When using `az keyvault certificate list`, passing `--include-pending` now doesn't require a value of `true` or `false`</span></span>

### <a name="netappfiles"></a><span data-ttu-id="8b368-346">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="8b368-346">NetAppFiles</span></span>

* <span data-ttu-id="8b368-347">Обновлена версия azure-mgmt-netapp до 0.7.0, которая включает некоторые дополнительные свойства тома, связанные с предстоящими операциями репликации.</span><span class="sxs-lookup"><span data-stu-id="8b368-347">Upgraded azure-mgmt-netapp to 0.7.0 which includes some additional volume properties associated with upcoming replication operations</span></span>

### <a name="network"></a><span data-ttu-id="8b368-348">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-348">Network</span></span>

* <span data-ttu-id="8b368-349">application-gateway waf-config. Не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="8b368-349">application-gateway waf-config: deprecated</span></span>
* <span data-ttu-id="8b368-350">application-gateway waf-policy. Добавлены управляемые правила подгрупп для контроля управляемых наборов правил и правил исключения.</span><span class="sxs-lookup"><span data-stu-id="8b368-350">application-gateway waf-policy: Added subgroup managed-rules to manage managed rule sets and exclusion rules</span></span>
* <span data-ttu-id="8b368-351">application-gateway waf-policy. Добавлен параметр политики подгруппы для управления глобальной конфигурацией политики WAF.</span><span class="sxs-lookup"><span data-stu-id="8b368-351">application-gateway waf-policy: Added subgroup policy-setting to manage global configuration of a waf-policy</span></span>
* <span data-ttu-id="8b368-352">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] application-gateway waf-policy. Переименовано правило подгруппы в пользовательское правило.</span><span class="sxs-lookup"><span data-stu-id="8b368-352">[BREAKING CHANGE] application-gateway waf-policy: Renamed subgroup rule to custom-rule</span></span>
* <span data-ttu-id="8b368-353">application-gateway http-listener. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="8b368-353">application-gateway http-listener: Added --firewall-policy when create</span></span>
* <span data-ttu-id="8b368-354">application-gateway url-path-map rule. Добавлен параметр --firewall-policy при создании.</span><span class="sxs-lookup"><span data-stu-id="8b368-354">application-gateway url-path-map rule: Added --firewall-policy when create</span></span>

### <a name="packaging"></a><span data-ttu-id="8b368-355">Упаковка</span><span class="sxs-lookup"><span data-stu-id="8b368-355">Packaging</span></span>

* <span data-ttu-id="8b368-356">Удалена команда az wrapper в Python.</span><span class="sxs-lookup"><span data-stu-id="8b368-356">Rewrote the az wrapper in Python</span></span>
* <span data-ttu-id="8b368-357">Включена поддержка Python 3.8.</span><span class="sxs-lookup"><span data-stu-id="8b368-357">Added support for Python 3.8</span></span>
* <span data-ttu-id="8b368-358">Изменена версия на Python 3 для пакета RPM.</span><span class="sxs-lookup"><span data-stu-id="8b368-358">Changed to Python 3 for RPM package</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-359">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-359">Profile</span></span>

* <span data-ttu-id="8b368-360">Исправлена ошибка при выполнении `az login -u {} -p {}` с учетной записью Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="8b368-360">Polished error when running `az login -u {} -p {}` with Microsoft account</span></span>
* <span data-ttu-id="8b368-361">Исправлена ошибка с `SSLError` при выполнении `az login` за прокси-сервером с самозаверяющим корневым сертификатом.</span><span class="sxs-lookup"><span data-stu-id="8b368-361">Polished `SSLError` when running `az login` behind a proxy with self-signed root certificate</span></span>
* <span data-ttu-id="8b368-362">Исправлена ошибка № 10578. `az login` зависает при одновременном запуске нескольких экземпляров в Windows или WSL.</span><span class="sxs-lookup"><span data-stu-id="8b368-362">Fixed #10578: `az login` hangs when more than one instances are launched at the same time on Windows or WSL</span></span>
* <span data-ttu-id="8b368-363">Исправлена ошибка № 11059. Сбой выполнения `az login --allow-no-subscriptions`, если в клиенте есть подписки.</span><span class="sxs-lookup"><span data-stu-id="8b368-363">Fixed #11059: `az login --allow-no-subscriptions` fails if there are subscriptions in the tenant</span></span>
* <span data-ttu-id="8b368-364">Исправлена ошибка № 11238. После переименования подписки вход с помощью MSI приведет к тому, что одна и та же подписка появится дважды.</span><span class="sxs-lookup"><span data-stu-id="8b368-364">Fixed #11238: After renaming a subscription, logging in with MSI will result in the same subscription appearing twice</span></span>

### <a name="rbac"></a><span data-ttu-id="8b368-365">RBAC</span><span class="sxs-lookup"><span data-stu-id="8b368-365">RBAC</span></span>

* <span data-ttu-id="8b368-366">Исправлена ошибка № 10996. Исправлена ошибка с `--force-change-password-next-login` в `az ad user update`, если `--password` не указывается.</span><span class="sxs-lookup"><span data-stu-id="8b368-366">Fixed #10996: Polish error for `--force-change-password-next-login` in `az ad user update` when `--password` is not specified</span></span>

### <a name="redis"></a><span data-ttu-id="8b368-367">Redis</span><span class="sxs-lookup"><span data-stu-id="8b368-367">Redis</span></span>

* <span data-ttu-id="8b368-368">Исправлена ошибка № 2902. Предотвращена настройка конфигураций памяти при обновлении кэша с номером SKU "Базовый".</span><span class="sxs-lookup"><span data-stu-id="8b368-368">Fixed #2902: Avoid setting memory configs while updating Basic SKU cache</span></span>

### <a name="reservations"></a><span data-ttu-id="8b368-369">Резервирование</span><span class="sxs-lookup"><span data-stu-id="8b368-369">Reservations</span></span>

* <span data-ttu-id="8b368-370">Обновлена версия пакета SDK до 0.6.0</span><span class="sxs-lookup"><span data-stu-id="8b368-370">Upgraded SDK Version to 0.6.0</span></span>
* <span data-ttu-id="8b368-371">Добавлены сведения о плане выставления счетов после вызова Get-Catalogs.</span><span class="sxs-lookup"><span data-stu-id="8b368-371">Added billingplan details info after calling Get-Gatalogs</span></span>
* <span data-ttu-id="8b368-372">Добавлена новая команда `az reservations reservation-order calculate` для вычисления стоимости резервирования.</span><span class="sxs-lookup"><span data-stu-id="8b368-372">Added new command `az reservations reservation-order calculate` to calculate the price for a reservation</span></span>
* <span data-ttu-id="8b368-373">Добавлена новая команда `az reservations reservation-order purchase` для приобретения нового резервирования.</span><span class="sxs-lookup"><span data-stu-id="8b368-373">Added new command `az reservations reservation-order purchase` to purchase a new reservation</span></span>

### <a name="rest"></a><span data-ttu-id="8b368-374">Rest</span><span class="sxs-lookup"><span data-stu-id="8b368-374">Rest</span></span>
* <span data-ttu-id="8b368-375">Изменена версия `az rest` на общедоступную.</span><span class="sxs-lookup"><span data-stu-id="8b368-375">Changed `az rest` to GA</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-376">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-376">SQL</span></span>

* <span data-ttu-id="8b368-377">Обновлена версия azure-mgmt-sql до 0.15.0.</span><span class="sxs-lookup"><span data-stu-id="8b368-377">Updated azure-mgmt-sql to version 0.15.0.</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-378">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-378">Storage</span></span>

* <span data-ttu-id="8b368-379">storage account create. Добавлен параметр --enable-hierarchical-namespace для включения поддержки семантики файловой системы в службе больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="8b368-379">storage account create: Added --enable-hierarchical-namespace to support filesystem semantics in blob service.</span></span>
* <span data-ttu-id="8b368-380">Удалено несвязанное исключение из сообщения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="8b368-380">Removed unrelated exception from error message</span></span>
* <span data-ttu-id="8b368-381">Исправлены проблемы, из-за которых появлялось неверное сообщение об отсутствии нужных разрешений на выполнение требуемой операции</span><span class="sxs-lookup"><span data-stu-id="8b368-381">Fixed issues with incorrect error message "You do not have the required permissions needed to perform this operation."</span></span> <span data-ttu-id="8b368-382">при блокировке правилами сети (AuthenticationFailed).</span><span class="sxs-lookup"><span data-stu-id="8b368-382">when blocked by network rules or AuthenticationFailed.</span></span>

## <a name="november-4-2019"></a><span data-ttu-id="8b368-383">4 ноября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-383">November 4, 2019</span></span>

<span data-ttu-id="8b368-384">Версия 2.0.76</span><span class="sxs-lookup"><span data-stu-id="8b368-384">Version 2.0.76</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-385">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-385">ACR</span></span>

* <span data-ttu-id="8b368-386">В команду `az acr pack build` добавлен параметр предварительной версии `--pack-image-tag`.</span><span class="sxs-lookup"><span data-stu-id="8b368-386">Added a preview parameter `--pack-image-tag` to command `az acr pack build`.</span></span>
* <span data-ttu-id="8b368-387">Добавлена поддержка включения аудита при создании реестра.</span><span class="sxs-lookup"><span data-stu-id="8b368-387">Added support for enabling auditing on creating a registry</span></span>
* <span data-ttu-id="8b368-388">Включена поддержка функции RBAC, распространяющаяся на репозиторий.</span><span class="sxs-lookup"><span data-stu-id="8b368-388">Added support for Repository-scoped RBAC</span></span>

### <a name="aks"></a><span data-ttu-id="8b368-389">AKS</span><span class="sxs-lookup"><span data-stu-id="8b368-389">AKS</span></span>

* <span data-ttu-id="8b368-390">В команду `az aks create` добавлены `--enable-cluster-autoscaler`, `--min-count` и `--max-count`, что позволяет автоматически масштабировать кластер для пула узлов.</span><span class="sxs-lookup"><span data-stu-id="8b368-390">Added `--enable-cluster-autoscaler`, `--min-count` and `--max-count` to the `az aks create` command, which enables cluster autoscaler for the node pool.</span></span>
* <span data-ttu-id="8b368-391">Добавлены указанные выше флаги, а также `--update-cluster-autoscaler` и `--disable-cluster-autoscaler` в команду `az aks update`, что позволяет обновлять средство автоматического масштабирования кластера.</span><span class="sxs-lookup"><span data-stu-id="8b368-391">Added the above flags as well as `--update-cluster-autoscaler` and `--disable-cluster-autoscaler` to the `az aks update` command, allowing updates to cluster autoscaler.</span></span>

### <a name="appconfig"></a><span data-ttu-id="8b368-392">AppConfig</span><span class="sxs-lookup"><span data-stu-id="8b368-392">AppConfig</span></span>

* <span data-ttu-id="8b368-393">Добавлена группа команд функции appconfig для управления флагами функций, хранимыми в Конфигурации приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-393">Added appconfig feature command group to manage feature flags stored in an App Configuration.</span></span>
* <span data-ttu-id="8b368-394">Исправлена незначительная ошибка команды экспорта в файл appconfig kv.</span><span class="sxs-lookup"><span data-stu-id="8b368-394">Fixed minor bug for appconfig kv export to file command.</span></span> <span data-ttu-id="8b368-395">Прерывание чтения содержимого конечного файла во время экспорта.</span><span class="sxs-lookup"><span data-stu-id="8b368-395">Stop reading dest file contents during export.</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-396">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-396">AppService</span></span>

* <span data-ttu-id="8b368-397">`az appservice plan create`: Добавлена поддержка определения persitescaling при создании плана appservice.</span><span class="sxs-lookup"><span data-stu-id="8b368-397">`az appservice plan create`: Added support to set 'persitescaling' on appservice plan create.</span></span>
* <span data-ttu-id="8b368-398">Исправлена проблема, из-за которой операция webapp config ssl bind удаляла существующие теги из ресурса.</span><span class="sxs-lookup"><span data-stu-id="8b368-398">Fixed an issue where webapp config ssl bind operation was removing existing tags from the resource</span></span>
* <span data-ttu-id="8b368-399">Добавлен флаг `--build-remote` для `az functionapp deployment source config-zip` для включения поддержки действия удаленной сборки во время развертывания приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="8b368-399">Added `--build-remote` flag for `az functionapp deployment source config-zip` to support remote build action during function app deployment.</span></span>
* <span data-ttu-id="8b368-400">Изменена версия узла по умолчанию для приложений-функций на ~10 для Windows</span><span class="sxs-lookup"><span data-stu-id="8b368-400">Changed default node version on function apps to ~10 for Windows</span></span>
* <span data-ttu-id="8b368-401">В `az functionapp create` добавлено свойство `--runtime-version`.</span><span class="sxs-lookup"><span data-stu-id="8b368-401">Added `--runtime-version` property to `az functionapp create`</span></span>

### <a name="arm"></a><span data-ttu-id="8b368-402">ARM</span><span class="sxs-lookup"><span data-stu-id="8b368-402">ARM</span></span>

* <span data-ttu-id="8b368-403">`az deployment/group deployment validate`: В `--handle-extended-json-format` добавлен параметр для включения поддержки многострочности и комментариев в шаблоне JSON при развертывании.</span><span class="sxs-lookup"><span data-stu-id="8b368-403">`az deployment/group deployment validate`: Added `--handle-extended-json-format` parameter to support multiline and comments in json template when deployment.</span></span>
* <span data-ttu-id="8b368-404">Версия azure-mgmt-resource обновлена до 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-404">Bumped azure-mgmt-resource to 2019-07-01</span></span>

### <a name="backup"></a><span data-ttu-id="8b368-405">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="8b368-405">Backup</span></span>

* <span data-ttu-id="8b368-406">Добавлена поддержка резервного копирования AzureFiles.</span><span class="sxs-lookup"><span data-stu-id="8b368-406">Added AzureFiles backup support</span></span>

### <a name="compute"></a><span data-ttu-id="8b368-407">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="8b368-407">Compute</span></span>

* <span data-ttu-id="8b368-408">`az vm create`: Добавлено предупреждение при одновременном определении ускоренной сети и существующей сетевой карты.</span><span class="sxs-lookup"><span data-stu-id="8b368-408">`az vm create`: Added warning when specifying accelerated networking and an existing NIC together.</span></span>
* <span data-ttu-id="8b368-409">`az vm create`: Добавлен параметр `--vmss` для определения существующего масштабируемого набора виртуальных машин, которому должна быть назначена виртуальная машина.</span><span class="sxs-lookup"><span data-stu-id="8b368-409">`az vm create`: Added `--vmss` to specify an existing virtual machine scale set that the virtual machine should be assigned to.</span></span>
* <span data-ttu-id="8b368-410">`az vm/vmss create`: Добавлена локальная копия файла псевдонима изображения, к которой можно получить доступ в ограниченной сетевой среде.</span><span class="sxs-lookup"><span data-stu-id="8b368-410">`az vm/vmss create`: Added a local copy of image alias file so that it can be accessed in a restricted network environment.</span></span>
* <span data-ttu-id="8b368-411">`az vmss create`: Добавлен параметр `--orchestration-mode` для определения того, как виртуальные машины управляются масштабируемым набором.</span><span class="sxs-lookup"><span data-stu-id="8b368-411">`az vmss create`: Added `--orchestration-mode` to specify how virtual machines are managed by the scale set.</span></span>
* <span data-ttu-id="8b368-412">`az vm/vmss update`: Добавлен параметр `--ultra-ssd-enabled`, чтобы разрешить обновление параметра Ultra SSD.</span><span class="sxs-lookup"><span data-stu-id="8b368-412">`az vm/vmss update`: Added `--ultra-ssd-enabled` to allow updating ultra SSD setting.</span></span>
* <span data-ttu-id="8b368-413">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az vm extension set`: Исправлена ошибка, из-за которой пользователям не удавалось определять расширение на виртуальной машине с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="8b368-413">[BREAKING CHANGE] `az vm extension set`: Fixed bug where users could not set an extension on a VM with `--ids`.</span></span>
* <span data-ttu-id="8b368-414">Добавлены новые команды `az vm image terms accept/cancel/show` для управления условиями использования образов Azure Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8b368-414">Added new commands `az vm image terms accept/cancel/show` to manage Azure Marketplace image terms.</span></span>
* <span data-ttu-id="8b368-415">Расширение VMAccessForLinux обновлено до версии 1.5.</span><span class="sxs-lookup"><span data-stu-id="8b368-415">Updated VMAccessForLinux to version 1.5</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8b368-416">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-416">CosmosDB</span></span>

* <span data-ttu-id="8b368-417">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az sql container create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="8b368-417">[BREAKING CHANGE] `az sql container create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="8b368-418">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az gremlin graph create`: `--partition-key-path` изменен на обязательный параметр.</span><span class="sxs-lookup"><span data-stu-id="8b368-418">[BREAKING CHANGE] `az gremlin graph create`: Changed `--partition-key-path` to required parameter</span></span>
* <span data-ttu-id="8b368-419">`az sql container create`: Добавлены команды `--unique-key-policy` и `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="8b368-419">`az sql container create`: Added `--unique-key-policy` and `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="8b368-420">`az sql container create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-420">`az sql container create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="8b368-421">`gremlin graph create`: Добавлена команда `--conflict-resolution-policy`.</span><span class="sxs-lookup"><span data-stu-id="8b368-421">`gremlin graph create`: Added `--conflict-resolution-policy`</span></span>
* <span data-ttu-id="8b368-422">`gremlin graph create/update`: Обновлена схема `--idx` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-422">`gremlin graph create/update`: Updated the `--idx` default schema</span></span>
* <span data-ttu-id="8b368-423">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="8b368-423">Fixed typo in help message</span></span>
* <span data-ttu-id="8b368-424">База данных: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="8b368-424">database: Added deprecation infomation</span></span>
* <span data-ttu-id="8b368-425">Коллекция: добавлены сведения об устаревании.</span><span class="sxs-lookup"><span data-stu-id="8b368-425">collection: Added deprecation infomation</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-426">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-426">IoT</span></span>

* <span data-ttu-id="8b368-427">Добавлен новый тип источника маршрутизации: DigitalTwinChangeEvents.</span><span class="sxs-lookup"><span data-stu-id="8b368-427">Added new routing source type: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="8b368-428">Добавлены отсутствующие компоненты в `az iot hub create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-428">Fixed missing features in `az iot hub create`</span></span>

### <a name="key-vault"></a><span data-ttu-id="8b368-429">Key Vault</span><span class="sxs-lookup"><span data-stu-id="8b368-429">Key Vault</span></span>

* <span data-ttu-id="8b368-430">Исправлена непредвиденная ошибка с отсутствием файла сертификата.</span><span class="sxs-lookup"><span data-stu-id="8b368-430">Fixed an unexpected error when certificate file does not exist</span></span>
* <span data-ttu-id="8b368-431">Исправлена ошибка с неработающей командой `az keyvault recover/purge`.</span><span class="sxs-lookup"><span data-stu-id="8b368-431">Fixed `az keyvault recover/purge` not working</span></span>

### <a name="netappfiles"></a><span data-ttu-id="8b368-432">NetAppFiles</span><span class="sxs-lookup"><span data-stu-id="8b368-432">NetAppFiles</span></span>

* <span data-ttu-id="8b368-433">Пакет azure-mgmt-netapp обновлен до версии 0.6.0 для включения поддержки API версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-433">Upgraded azure-mgmt-netapp to 0.6.0 to use API version 2019-07-01.</span></span> <span data-ttu-id="8b368-434">Эта новая версия API включает:</span><span class="sxs-lookup"><span data-stu-id="8b368-434">This new API version includes:</span></span>

    - <span data-ttu-id="8b368-435">При создании тома с использованием `--protocol-types` допускается NFSv4.1 вместо NFSv4.</span><span class="sxs-lookup"><span data-stu-id="8b368-435">Volume creation `--protocol-types` accepts now "NFSv4.1" not "NFSv4"</span></span>
    - <span data-ttu-id="8b368-436">Свойство политики экспорта томов теперь называется nfsv41, а не nfsv4.</span><span class="sxs-lookup"><span data-stu-id="8b368-436">Volume export policy property now named 'nfsv41' not 'nfsv4'</span></span>
    - <span data-ttu-id="8b368-437">Параметр `--creation-token` для тома переименован в `--file-path`.</span><span class="sxs-lookup"><span data-stu-id="8b368-437">Volume `--creation-token` renamed to `--file-path`</span></span>
    - <span data-ttu-id="8b368-438">Дата создания моментального снимка теперь имеет значение Created.</span><span class="sxs-lookup"><span data-stu-id="8b368-438">Snapshot creation date now named just 'created'</span></span>

### <a name="network"></a><span data-ttu-id="8b368-439">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-439">Network</span></span>

* <span data-ttu-id="8b368-440">`az network private-dns link vnet create/update`: Добавлена поддержка связывания виртуальных сетей между клиентами.</span><span class="sxs-lookup"><span data-stu-id="8b368-440">`az network private-dns link vnet create/update`: Support cross-tenant virtual network linking.</span></span>
* <span data-ttu-id="8b368-441">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ.] `az network vnet subnet list`: Параметры `--resource-group` и `--vnet-name` теперь являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="8b368-441">[BREAKING CHANGE] `az network vnet subnet list`: Changed `--resource-group` and `--vnet-name` to be required now.</span></span>
* <span data-ttu-id="8b368-442">`az network public-ip prefix create`: Включена поддержка определения версии IP-адреса (IPv4, IPv6) при создании.</span><span class="sxs-lookup"><span data-stu-id="8b368-442">`az network public-ip prefix create`: Added support to specify IP address version (IPv4, IPv6) when creation</span></span>
* <span data-ttu-id="8b368-443">Версия azure-mgmt-network обновлена до 7.0.0 и версия api-version до 2019-09-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-443">Bumped azure-mgmt-network to 7.0.0 and api-version to 2019-09-01</span></span>
* <span data-ttu-id="8b368-444">`az network vrouter`: Включена поддержка нового виртуального маршрутизатора службы и пиринга виртуальных маршрутизаторов.</span><span class="sxs-lookup"><span data-stu-id="8b368-444">`az network vrouter`: Added support for new service virtual router and virtual router peering</span></span>
* <span data-ttu-id="8b368-445">`az network express-route gateway connection`: Добавлена поддержка параметра `--internet-security`.</span><span class="sxs-lookup"><span data-stu-id="8b368-445">`az network express-route gateway connection`: Added support for `--internet-security`</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-446">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-446">Profile</span></span>

* <span data-ttu-id="8b368-447">Исправлена ошибка с неработающей командой `az account get-access-token --resource-type ms-graph`.</span><span class="sxs-lookup"><span data-stu-id="8b368-447">Fixed `az account get-access-token --resource-type ms-graph` not working</span></span>
* <span data-ttu-id="8b368-448">Удалено предупреждение из `az login`.</span><span class="sxs-lookup"><span data-stu-id="8b368-448">Removed warning from `az login`</span></span>

### <a name="rbac"></a><span data-ttu-id="8b368-449">RBAC</span><span class="sxs-lookup"><span data-stu-id="8b368-449">RBAC</span></span>

* <span data-ttu-id="8b368-450">Исправление `az ad app update --id {} --display-name {}` не работает.</span><span class="sxs-lookup"><span data-stu-id="8b368-450">Fixed `az ad app update --id {} --display-name {}` doesn't work</span></span>

### <a name="servicefabric"></a><span data-ttu-id="8b368-451">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8b368-451">ServiceFabric</span></span>

* <span data-ttu-id="8b368-452">`az sf cluster create`: Исправлена проблема путем изменения VMSS для вычислений с использованием файла template.json для Service Fabric Linux и Windows со стандартных дисков на управляемые.</span><span class="sxs-lookup"><span data-stu-id="8b368-452">`az sf cluster create`: Fixed an issue by modifying service fabric linux and windows template.json compute vmss from standard to managed disks</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-453">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-453">SQL</span></span>

* <span data-ttu-id="8b368-454">Добавлены параметры `--compute-model`, `--auto-pause-delay` и `--min-capacity` для включения поддержки операций CRUD для нового предложения Базы данных SQL: Модель бессерверных вычислений.</span><span class="sxs-lookup"><span data-stu-id="8b368-454">Added `--compute-model`, `--auto-pause-delay`, and `--min-capacity` parameters to support CRUD operations for new SQL Database offering: Serverless compute model.</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-455">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-455">Storage</span></span>

* <span data-ttu-id="8b368-456">`az storage account create/update`: Добавлен параметр --enable-files-adds и группа аргументов свойств Azure Active Directory для включения поддержки аутентификации доменных служб Azure Active Directory для Файлов Azure.</span><span class="sxs-lookup"><span data-stu-id="8b368-456">`az storage account create/update`: Added --enable-files-adds parameter and Azure Active Directory Properties Argument group to support Azure Files Active Directory Domain Service Authentication</span></span>
* <span data-ttu-id="8b368-457">Расширена команда `az storage account keys list/renew` для включения поддержки перечисления или повторного создания ключей Kerberos для учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="8b368-457">Expanded `az storage account keys list/renew` to support listing or regenerating Kerberos keys of storage account.</span></span>

## <a name="october-15-2019"></a><span data-ttu-id="8b368-458">15 октября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-458">October 15, 2019</span></span>

<span data-ttu-id="8b368-459">Версия 2.0.75</span><span class="sxs-lookup"><span data-stu-id="8b368-459">Version 2.0.75</span></span>

### <a name="aks"></a><span data-ttu-id="8b368-460">AKS</span><span class="sxs-lookup"><span data-stu-id="8b368-460">AKS</span></span>

* <span data-ttu-id="8b368-461">Для параметра `--load-balancer-sku` изменено значение по умолчанию на `standard`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="8b368-461">Changed `--load-balancer-sku` default value to `standard` if supported by the kubernetes version</span></span>
* <span data-ttu-id="8b368-462">Для параметра `--vm-set-type` изменено значение по умолчанию на `virtualmachinescalesets`, если поддерживается версией AKS.</span><span class="sxs-lookup"><span data-stu-id="8b368-462">Changed `--vm-set-type` default value to `virtualmachinescalesets` if supported by the kubernetes version</span></span>

### <a name="ams"></a><span data-ttu-id="8b368-463">AMS</span><span class="sxs-lookup"><span data-stu-id="8b368-463">AMS</span></span>

* <span data-ttu-id="8b368-464">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя `job start` изменено на `job create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-464">[BREAKING CHANGE] Changed the name of `job start` to `job create`</span></span>
* <span data-ttu-id="8b368-465">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В параметре `--ask` команды `content-key-policy create` вместо кодировки UTF8 теперь используется шестнадцатеричная строка из 32 символов.</span><span class="sxs-lookup"><span data-stu-id="8b368-465">[BREAKING CHANGE] Changed the `--ask` parameter of `content-key-policy create` to use a 32-character hex string instead of UTF8</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-466">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-466">AppService</span></span>

* <span data-ttu-id="8b368-467">Добавлены команды `webapp config access-restriction show|set|add|remove`.</span><span class="sxs-lookup"><span data-stu-id="8b368-467">Added commands `webapp config access-restriction show|set|add|remove`</span></span>
* <span data-ttu-id="8b368-468">Улучшена обработка ошибок в `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="8b368-468">Added better error handling to `webapp up`</span></span>
* <span data-ttu-id="8b368-469">Для `appservice plan update` добавлена поддержка номера SKU `Isolated`.</span><span class="sxs-lookup"><span data-stu-id="8b368-469">Added support for `Isolated` SKU to `appservice plan update`</span></span>

### <a name="arm"></a><span data-ttu-id="8b368-470">ARM</span><span class="sxs-lookup"><span data-stu-id="8b368-470">ARM</span></span>

* <span data-ttu-id="8b368-471">В `deployment create` добавлен параметр `--handle-extended-json-format` для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="8b368-471">Added `--handle-extended-json-format` parameter `deployment create` to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="8b368-472">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="8b368-472">Compute</span></span>

* <span data-ttu-id="8b368-473">Добавлен параметр `--enable-agent` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-473">Added `--enable-agent` parameter to `vm create`</span></span>
* <span data-ttu-id="8b368-474">Внесены изменения в `vm create`, позволяющие автоматически использовать номер SKU "Стандартный" для общедоступных IP-адресов при использовании зон.</span><span class="sxs-lookup"><span data-stu-id="8b368-474">Changed `vm create` to use standard public IP SKU automatically when using zones</span></span>
* <span data-ttu-id="8b368-475">Внесены изменения в `vm create`, позволяющие автоматически создавать допустимое имя для виртуальной машины, если оно не задано.</span><span class="sxs-lookup"><span data-stu-id="8b368-475">Changed `vm create` to automatically create a valid computer name for a VM if none is provided</span></span>
* <span data-ttu-id="8b368-476">В `vmss create` добавлен параметр `--computer-name-prefix` для поддержки пользовательского префикса имени для виртуальных машин в VMSS.</span><span class="sxs-lookup"><span data-stu-id="8b368-476">Added `--computer-name-prefix` parameter to `vmss create` to support custom computer name prefix of virtual machines in the VMSS</span></span>
* <span data-ttu-id="8b368-477">В `vm create` добавлен параметр `--workspace` для автоматического включения рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="8b368-477">Add `--workspace` parameter to `vm create` to enable log analytics workspace automatically</span></span>
* <span data-ttu-id="8b368-478">API коллекций обновлен до версии 2019-07-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-478">Updated galleries API version to 2019-07-01</span></span>

### <a name="core"></a><span data-ttu-id="8b368-479">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-479">Core</span></span>

* <span data-ttu-id="8b368-480">Добавлена проверка синтаксиса для параметра `--set` в универсальной команде обновления.</span><span class="sxs-lookup"><span data-stu-id="8b368-480">Added syntax check for `--set` parameter in generic update command</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-481">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-481">IoT</span></span>

* <span data-ttu-id="8b368-482">Исправлена проблема, при которой `iot hub show` неправильно выдавал ошибку "Ресурс не найден".</span><span class="sxs-lookup"><span data-stu-id="8b368-482">Fixed an issue where `iot hub show` would incorrectly error with "resource not found"</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-483">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-483">Monitor</span></span>

* <span data-ttu-id="8b368-484">В `monitor log-analytics workspace` добавлена поддержка CRUD.</span><span class="sxs-lookup"><span data-stu-id="8b368-484">Added support for CRUD to `monitor log-analytics workspace`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-485">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-485">Network</span></span>

* <span data-ttu-id="8b368-486">В `network private-dns link vnet [create|update]` добавлена поддержка виртуального канала для клиентов.</span><span class="sxs-lookup"><span data-stu-id="8b368-486">Added support for cross-tenant virtual linking to `network private-dns link vnet [create|update]`</span></span>
* <span data-ttu-id="8b368-487">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для `network vnet subnet list` теперь требуются параметры `--resource-group` и `--vnet-name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-487">[BREAKING CHANGE] Changed `network vnet subnet list` to require `--resource-group` and `--vnet-name` parameters</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-488">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-488">SQL</span></span>

* <span data-ttu-id="8b368-489">В `sql mi ad-admin` добавлены команды, которые поддерживают назначение администратора AAD в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="8b368-489">Added commands to `sql mi ad-admin` that support setting an AAD administrator on managed instances</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-490">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-490">Storage</span></span>

* <span data-ttu-id="8b368-491">В `storage copy` добавлен параметр `--preserve-s2s-access-tier`, позволяющий сохранить уровень доступа во время копирования между службами.</span><span class="sxs-lookup"><span data-stu-id="8b368-491">Added `--preserve-s2s-access-tier` parameter `storage copy` to preserve access tier during service to service copy</span></span>
* <span data-ttu-id="8b368-492">В `storage account [create|update]` добавлен параметр `--enable-large-file-share` для поддержки общих папок большого размера в учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="8b368-492">Added `--enable-large-file-share` parameter to `storage account [create|update]` to support large file shares for storage account</span></span>

## <a name="september-24-2019"></a><span data-ttu-id="8b368-493">24 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-493">September 24, 2019</span></span>

<span data-ttu-id="8b368-494">Версия 2.0.74</span><span class="sxs-lookup"><span data-stu-id="8b368-494">Version 2.0.74</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-495">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-495">ACR</span></span>

* <span data-ttu-id="8b368-496">В `acr config retention update` добавлен обязательный параметр `--type`.</span><span class="sxs-lookup"><span data-stu-id="8b368-496">Added a required `--type` parameter to `acr config retention update`</span></span>
* <span data-ttu-id="8b368-497">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименованный параметр `--name -n` изменен на `--registry -r ` для группы команд `acr config`.</span><span class="sxs-lookup"><span data-stu-id="8b368-497">[BREAKING CHNAGE] Renamed parameter `--name -n` changed to `--registry -r ` for `acr config` command group</span></span>

### <a name="aks"></a><span data-ttu-id="8b368-498">AKS</span><span class="sxs-lookup"><span data-stu-id="8b368-498">AKS</span></span>

* <span data-ttu-id="8b368-499">В команду `aks create` добавлен параметр `--load-balancer-sku`, позволяющий создать кластер AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="8b368-499">Added `--load-balancer-sku` parameter to `aks create` command, which allows for creating AKS cluster with SLB</span></span>
* <span data-ttu-id="8b368-500">В команды `aks [create|update]` добавлены параметры `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` и `--load-balancer-outbound-ip-prefixes`, позволяющие обновлять профиль подсистемы балансировки нагрузки у кластера AKS с SLB.</span><span class="sxs-lookup"><span data-stu-id="8b368-500">Added `--load-balancer-managed-outbound-ip-count`, `--load-balancer-outbound-ips` and `--load-balancer-outbound-ip-prefixes` parameters to `aks [create|update]` commands, which allow for updating load balancer profile of an AKS cluster with SLB</span></span>
* <span data-ttu-id="8b368-501">В команду `aks create` добавлен параметр `--vm-set-type`, позволяющий указывать типы виртуальных машин в кластере AKS.</span><span class="sxs-lookup"><span data-stu-id="8b368-501">Added `--vm-set-type` parameter to `aks create` command, which allows to specify vm types of an AKS Cluster (vmas or vmss)</span></span>

### <a name="arm"></a><span data-ttu-id="8b368-502">ARM</span><span class="sxs-lookup"><span data-stu-id="8b368-502">ARM</span></span>

* <span data-ttu-id="8b368-503">В команду `group deployment create` добавлен параметр `--handle-extended-json-format`, для поддержки многострочности и комментариев в шаблоне JSON.</span><span class="sxs-lookup"><span data-stu-id="8b368-503">Added `--handle-extended-json-format` parameter to `group deployment create` command to support multiline and comments in json template</span></span>

### <a name="compute"></a><span data-ttu-id="8b368-504">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="8b368-504">Compute</span></span>

* <span data-ttu-id="8b368-505">В команды `vmss [create|update]` добавлен параметр `--terminate-notification-time`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="8b368-505">Added `--terminate-notification-time` parameter to `vmss [create|update]` commands to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="8b368-506">В команду `vmss update` добавлен параметр `--enable-terminate-notification`, поддерживающий завершение настройки запланированных событий.</span><span class="sxs-lookup"><span data-stu-id="8b368-506">Added `--enable-terminate-notification` parameter to `vmss update` command to support terminate scheduled event configurability</span></span>
* <span data-ttu-id="8b368-507">В команды `[vm|vmss] create` добавлены параметры `--priority,`, `--eviction-policy,` и `--max-billing`.</span><span class="sxs-lookup"><span data-stu-id="8b368-507">Added `--priority,` `--eviction-policy,` `--max-billing` parameters to `[vm|vmss] create` commands</span></span>
* <span data-ttu-id="8b368-508">Изменена команда `disk create`, которая теперь позволяет указать точный размер отправки на диск.</span><span class="sxs-lookup"><span data-stu-id="8b368-508">Changed `disk create` to allow specifying the exact size of the disk upload</span></span>
* <span data-ttu-id="8b368-509">В `snapshot create` добавлена поддержка добавочных моментальных снимков для управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="8b368-509">Added support for incremental snapshots for managed disks to `snapshot create`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="8b368-510">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-510">Cosmos DB</span></span>

* <span data-ttu-id="8b368-511">В команду `cosmosdb keys list` добавлен параметр `--type <key-type>` для отображения ключей, ключей только для чтения или строк подключения.</span><span class="sxs-lookup"><span data-stu-id="8b368-511">Added `--type <key-type>` parameter to `cosmosdb keys list` command to show key, read only keys or connection strings</span></span>
* <span data-ttu-id="8b368-512">Добавлена команда `cosmosdb keys regenerate`.</span><span class="sxs-lookup"><span data-stu-id="8b368-512">Added `cosmosdb keys regenerate` command</span></span>
* <span data-ttu-id="8b368-513">[УСТАРЕЛО] Команды `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` и `cosmosdb list-read-only-keys` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8b368-513">[DEPRECATED] Deprecated `cosmosdb list-connection-strings`, `cosmosdb regenerate-key` and `cosmosdb list-read-only-keys` commands</span></span>

### <a name="eventgrid"></a><span data-ttu-id="8b368-514">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="8b368-514">EventGrid</span></span>

* <span data-ttu-id="8b368-515">Исправлен текст справки по конечной точке — дана ссылка на правильный параметр.</span><span class="sxs-lookup"><span data-stu-id="8b368-515">Fixed the endpoint help text to refer to the right parameter</span></span>

### <a name="key-vault"></a><span data-ttu-id="8b368-516">Key Vault</span><span class="sxs-lookup"><span data-stu-id="8b368-516">Key Vault</span></span>

* <span data-ttu-id="8b368-517">Исправлена проблема, из-за которой вход с помощью клиента (`login -t`) мог приводить к сбою `keyvault create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-517">Fixed issue where logging in with a tenant (`login -t`) could cause `keyvault create` to fail</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-518">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-518">Monitor</span></span>

* <span data-ttu-id="8b368-519">Исправлена проблема с тем, что символ `:` являлся недопустимым в аргументе `--condition` для `monitor metrics alert create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-519">Fixed issue where `:` character was not allowed in `--condition` argument to `monitor metrics alert create`</span></span>

### <a name="policy"></a><span data-ttu-id="8b368-520">Политика</span><span class="sxs-lookup"><span data-stu-id="8b368-520">Policy</span></span>

* <span data-ttu-id="8b368-521">Добавлена поддержка API Политики версии 2019-06-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-521">Added support for Policy API version 2019-06-01</span></span>
* <span data-ttu-id="8b368-522">В команду `policy assignment create` добавлен параметр `--enforcement-mode`.</span><span class="sxs-lookup"><span data-stu-id="8b368-522">Added `--enforcement-mode` parameter to `policy assignment create` command</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-523">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-523">Storage</span></span>

* <span data-ttu-id="8b368-524">В команду `az storage copy` добавлен параметр `--blob-type`.</span><span class="sxs-lookup"><span data-stu-id="8b368-524">Added `--blob-type` parameter to `az storage copy` command</span></span>

## <a name="september-10-2019"></a><span data-ttu-id="8b368-525">10 сентября 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-525">September 10, 2019</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-526">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-526">ACR</span></span>

* <span data-ttu-id="8b368-527">Добавлена группа команд `acr config retention` для настройки политики хранения.</span><span class="sxs-lookup"><span data-stu-id="8b368-527">Added command group `acr config retention` to configure retention policy</span></span>

### <a name="aks"></a><span data-ttu-id="8b368-528">AKS</span><span class="sxs-lookup"><span data-stu-id="8b368-528">AKS</span></span>

* <span data-ttu-id="8b368-529">Добавлена возможность интеграции ACR с помощью следующих команд:</span><span class="sxs-lookup"><span data-stu-id="8b368-529">Added support for ACR integration with the following commands:</span></span>
  * <span data-ttu-id="8b368-530">В `aks [create|update]` добавлен параметр `--attach-acr` для подключения ACR к кластеру AKS.</span><span class="sxs-lookup"><span data-stu-id="8b368-530">Added `--attach-acr` parameter to `aks [create|update]` to attach an ACR to an AKS cluster</span></span>
  * <span data-ttu-id="8b368-531">В `aks update` добавлен параметр `--detach-acr` для отключения ACR от кластера AKS.</span><span class="sxs-lookup"><span data-stu-id="8b368-531">Added `--detach-acr` parameter to `aks update` to detach the ACR from an AKS cluster</span></span>

### <a name="arm"></a><span data-ttu-id="8b368-532">ARM</span><span class="sxs-lookup"><span data-stu-id="8b368-532">ARM</span></span>

* <span data-ttu-id="8b368-533">Добавлена возможность использования API версии 2019-05-10.</span><span class="sxs-lookup"><span data-stu-id="8b368-533">Updated to use API version 2019-05-10</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-534">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-534">Batch</span></span>

* <span data-ttu-id="8b368-535">Добавлены новые параметры конфигурации JSON в `--json-file` для `batch pool create`:</span><span class="sxs-lookup"><span data-stu-id="8b368-535">Added new JSON configuration settings to `--json-file` for `batch pool create`:</span></span>
  * <span data-ttu-id="8b368-536">Добавлен параметр `MountConfigurations` для подключений файловой системы (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="8b368-536">Added `MountConfigurations` for file system mounts (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
  * <span data-ttu-id="8b368-537">Добавлено необязательное свойство `publicIPs` в `NetworkConfiguration` для общедоступных IP-адресов в пулах (дополнительные сведения см. в разделе https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body ).</span><span class="sxs-lookup"><span data-stu-id="8b368-537">Added optional property `publicIPs` on `NetworkConfiguration` for public IPs on pools (see https://docs.microsoft.com/rest/api/batchservice/pool/add#request-body for details)</span></span>
* <span data-ttu-id="8b368-538">В `--image` добавлена поддержка коллекций общих образов.</span><span class="sxs-lookup"><span data-stu-id="8b368-538">Added support for shared image galleries to `--image`</span></span>
* <span data-ttu-id="8b368-539">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `--start-task-wait-for-success` в `batch pool create` изменено на `true`.</span><span class="sxs-lookup"><span data-stu-id="8b368-539">[BREAKING CHANGE] Changed default value of `--start-task-wait-for-success` on `batch pool create` to be `true`</span></span>
* <span data-ttu-id="8b368-540">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию для `Scope` в `AutoUserSpecification` задано как Pool (ранее `Task` на узлах Windows и `Pool` на узлах Linux).</span><span class="sxs-lookup"><span data-stu-id="8b368-540">[BREAKING CHANGE] Changed default value for `Scope` on `AutoUserSpecification` to always be Pool (was `Task` on Windows nodes, `Pool` on Linux nodes)</span></span>
  * <span data-ttu-id="8b368-541">Этот аргумент можно задать только в конфигурации JSON с помощью `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="8b368-541">This argument can only be set from a JSON configuration with `--json-file`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8b368-542">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b368-542">HDInsight</span></span>

* <span data-ttu-id="8b368-543">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="8b368-543">GA release</span></span>
* <span data-ttu-id="8b368-544">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--workernode-count/-c` в `az hdinsight resize` теперь является обязательным.</span><span class="sxs-lookup"><span data-stu-id="8b368-544">[BREAKING CHANGE] Changed parameter `--workernode-count/-c` of `az hdinsight resize` to be required.</span></span>

### <a name="key-vault"></a><span data-ttu-id="8b368-545">Key Vault</span><span class="sxs-lookup"><span data-stu-id="8b368-545">Key Vault</span></span>

* <span data-ttu-id="8b368-546">Исправлена проблема, когда подсети не удавалось удалить из сетевых правил.</span><span class="sxs-lookup"><span data-stu-id="8b368-546">Fixed issue where subnets couldn't be deleted from network rules</span></span>
* <span data-ttu-id="8b368-547">Исправлена проблема, когда дублированные подсети и IP-адреса могли быть добавлены к сетевым правилам.</span><span class="sxs-lookup"><span data-stu-id="8b368-547">Fixed issue where duplicated subnets and IP addresses could be added to network rules</span></span>

### <a name="network"></a><span data-ttu-id="8b368-548">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-548">Network</span></span>

* <span data-ttu-id="8b368-549">Добавлен параметр `--interval` в `network watcher flow-log` для выбора значения интервала анализа трафика.</span><span class="sxs-lookup"><span data-stu-id="8b368-549">Added `--interval` parameter to `network watcher flow-log` to set traffic analysis interval value</span></span>
* <span data-ttu-id="8b368-550">Добавлена команда `network application-gateway identity` для управления удостоверением шлюза.</span><span class="sxs-lookup"><span data-stu-id="8b368-550">Added `network application-gateway identity` to manage gateway identity</span></span>
* <span data-ttu-id="8b368-551">Добавлена возможность указать идентификатор Key Vault в команде `network application-gateway ssl-cert`.</span><span class="sxs-lookup"><span data-stu-id="8b368-551">Added support for setting Key Vault ID to `network application-gateway ssl-cert`</span></span>
* <span data-ttu-id="8b368-552">Добавлена команда `network express-route peering peer-connection [show|list]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-552">Added `network express-route peering peer-connection [show|list]`</span></span>

### <a name="policy"></a><span data-ttu-id="8b368-553">Политика</span><span class="sxs-lookup"><span data-stu-id="8b368-553">Policy</span></span>

* <span data-ttu-id="8b368-554">Добавлена возможность использования API версии 2019-01-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-554">Updated to use API version 2019-01-01</span></span>

## <a name="august-27-2019"></a><span data-ttu-id="8b368-555">27 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-555">August 27, 2019</span></span>

<span data-ttu-id="8b368-556">Версия 2.0.72</span><span class="sxs-lookup"><span data-stu-id="8b368-556">Version 2.0.72</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-557">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-557">ACR</span></span>

* <span data-ttu-id="8b368-558">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка SKU `classic`.</span><span class="sxs-lookup"><span data-stu-id="8b368-558">[BREAKING CHANGE] Removed support for the `classic` SKU</span></span>

### <a name="api-management"></a><span data-ttu-id="8b368-559">Управление API</span><span class="sxs-lookup"><span data-stu-id="8b368-559">API Management</span></span>

* <span data-ttu-id="8b368-560">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена группа команд `apim`.</span><span class="sxs-lookup"><span data-stu-id="8b368-560">[PREVIEW] Added `apim` command group</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-561">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-561">AppService</span></span>

* <span data-ttu-id="8b368-562">Исправлена проблема с командой `webapp webjob continuous start` при указании слота.</span><span class="sxs-lookup"><span data-stu-id="8b368-562">Fixed issue with `webapp webjob continuous start` command when specifying a slot</span></span>
* <span data-ttu-id="8b368-563">Изменена команда `webapp up` для обнаружения и удаления папки `env` из файла, используемого для развертывания.</span><span class="sxs-lookup"><span data-stu-id="8b368-563">Changed `webapp up` to detect `env` folder and remove it from the file used for deployment</span></span>

### <a name="keyvault"></a><span data-ttu-id="8b368-564">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8b368-564">Keyvault</span></span>

* <span data-ttu-id="8b368-565">Исправлена ошибка в команде `keyvault secret set`, которая игнорировала аргумент `--expires`.</span><span class="sxs-lookup"><span data-stu-id="8b368-565">Fixed a bug in `keyvault secret set` that igored the `--expires` argument</span></span>

### <a name="network"></a><span data-ttu-id="8b368-566">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-566">Network</span></span>

* <span data-ttu-id="8b368-567">Добавлена поддержка IPv6-адресов для аргументов `--private-ip-address-version`.</span><span class="sxs-lookup"><span data-stu-id="8b368-567">Added support for IPv6 addresses to `--private-ip-address-version` arguments</span></span>
* <span data-ttu-id="8b368-568">Добавлены новые команды `network private-endpoint [create|update|list-types]` для управления закрытыми конечными точками.</span><span class="sxs-lookup"><span data-stu-id="8b368-568">Added new commands `network private-endpoint [create|update|list-types]` for private endpoint management</span></span>
* <span data-ttu-id="8b368-569">Добавлена группа команд для `network private-link-service`.</span><span class="sxs-lookup"><span data-stu-id="8b368-569">Added command group `network private-link-service`</span></span>
* <span data-ttu-id="8b368-570">Добавлены аргументы `--private-endpoint-network-policies` и `--private-link-service-network-policies` для команды `network vnet subnet update`</span><span class="sxs-lookup"><span data-stu-id="8b368-570">Added `--private-endpoint-network-policies` and `--private-link-service-network-policies` arguments to `network vnet subnet update`</span></span>

### <a name="rbac"></a><span data-ttu-id="8b368-571">RBAC</span><span class="sxs-lookup"><span data-stu-id="8b368-571">RBAC</span></span>

* <span data-ttu-id="8b368-572">Исправлена проблема с `ad app update --homepage`, когда домашнюю страницу нельзя было обновить.</span><span class="sxs-lookup"><span data-stu-id="8b368-572">Fixed issue with `ad app update --homepage` where homepage would not be updated</span></span>

### <a name="servicefabric"></a><span data-ttu-id="8b368-573">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8b368-573">ServiceFabric</span></span>

* <span data-ttu-id="8b368-574">Добавлена поддержка имен Key Vault в смешанном регистре.</span><span class="sxs-lookup"><span data-stu-id="8b368-574">Added support for mixed-case Key Vault names</span></span>
* <span data-ttu-id="8b368-575">Исправлена проблема с использованием сертификатов в Key Vault.</span><span class="sxs-lookup"><span data-stu-id="8b368-575">Fixed issue when using certificates in Key Vault</span></span>
* <span data-ttu-id="8b368-576">Исправлена проблема с использованием файлов сертификатов PFX.</span><span class="sxs-lookup"><span data-stu-id="8b368-576">Fixed issue with using PFX certificate files</span></span>
* <span data-ttu-id="8b368-577">Исправлена проблема с `sf cluster certificate add`, когда группа ресурсов Key Vault не была указана.</span><span class="sxs-lookup"><span data-stu-id="8b368-577">Fixed issue with `sf cluster certificate add` when Key Vault resource group wasn't specified</span></span>
* <span data-ttu-id="8b368-578">Исправлена проблема с неработающей командой `sf cluster set`.</span><span class="sxs-lookup"><span data-stu-id="8b368-578">Fixed issue with `sf cluster set` not working</span></span>

### <a name="signalr"></a><span data-ttu-id="8b368-579">SignalR</span><span class="sxs-lookup"><span data-stu-id="8b368-579">SignalR</span></span>

* <span data-ttu-id="8b368-580">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="8b368-580">Added new commands:</span></span>
  * <span data-ttu-id="8b368-581">`signalr cors`: Управление CORS SignalR</span><span class="sxs-lookup"><span data-stu-id="8b368-581">`signalr cors`: Manage SignalR CORS</span></span>
  * <span data-ttu-id="8b368-582">`signalr restart`: Перезапуск службы SignalR</span><span class="sxs-lookup"><span data-stu-id="8b368-582">`signalr restart`: Restart a SignalR service</span></span>
  * <span data-ttu-id="8b368-583">`signalr update`: Обновление службы SignalR</span><span class="sxs-lookup"><span data-stu-id="8b368-583">`signalr update`: Update a SignalR service</span></span>
* <span data-ttu-id="8b368-584">Добавлен аргумент `--service-mode` для команды `signalr create`</span><span class="sxs-lookup"><span data-stu-id="8b368-584">Added `--service-mode` argument to `signalr create`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-585">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-585">Storage</span></span>

* <span data-ttu-id="8b368-586">Добавлена команда `storage account revoke-delegation-keys`.</span><span class="sxs-lookup"><span data-stu-id="8b368-586">Added `storage account revoke-delegation-keys` command</span></span>

## <a name="august-13-2019"></a><span data-ttu-id="8b368-587">13 августа 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-587">August 13, 2019</span></span>

<span data-ttu-id="8b368-588">Версия 2.0.71</span><span class="sxs-lookup"><span data-stu-id="8b368-588">Version 2.0.71</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-589">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-589">AppService</span></span>

* <span data-ttu-id="8b368-590">Исправлена проблема, из-за которой выполнение команд `webapp webjob continuous` для слотов завершалось сбоем.</span><span class="sxs-lookup"><span data-stu-id="8b368-590">Fixed issue where `webapp webjob continuous` commands were failing for slots</span></span>

### <a name="botservice"></a><span data-ttu-id="8b368-591">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-591">BotService</span></span>

* <span data-ttu-id="8b368-592">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Прекращена поддержка создания ботов на основе пакета SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="8b368-592">[BREAKING CHANGE] Removed support for creating v3 SDK bots</span></span>

### <a name="cognitiveservices"></a><span data-ttu-id="8b368-593">Cognitive Services:</span><span class="sxs-lookup"><span data-stu-id="8b368-593">CognitiveServices</span></span>

* <span data-ttu-id="8b368-594">Добавлены команды `cognitiveservices account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="8b368-594">Added `cognitiveservices account network-rule` commands</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="8b368-595">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-595">Cosmos DB</span></span>

* <span data-ttu-id="8b368-596">Удалено предупреждение при обновлении нескольких расположений для записи.</span><span class="sxs-lookup"><span data-stu-id="8b368-596">Removed warning when updating multiple write locations</span></span>
* <span data-ttu-id="8b368-597">Добавлены команды CRUD для ресурсов CosmosDB SQL, MongoDB, Cassandra, Gremlin и ресурсов таблиц, а также пропускной способности ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-597">Added CRUD commands for CosmosDB SQL, MongoDB, Cassandra, Gremlin and Table resources and resource's throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8b368-598">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b368-598">HDInsight</span></span>

<span data-ttu-id="8b368-599">Этот выпуск содержит большое число критических изменений.</span><span class="sxs-lookup"><span data-stu-id="8b368-599">This release contains a large number of breaking changes.</span></span>

* <span data-ttu-id="8b368-600">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `hdinsight create`:</span><span class="sxs-lookup"><span data-stu-id="8b368-600">[BREAKING CHANGE] Renamed parameters for `hdinsight create`:</span></span>
  * <span data-ttu-id="8b368-601">Переименование `--storage-default-container` в `--storage-container`</span><span class="sxs-lookup"><span data-stu-id="8b368-601">Renamed `--storage-default-container` to `--storage-container`</span></span>
  * <span data-ttu-id="8b368-602">Переименование `--storage-default-filesystem` в `--storage-filesystem`</span><span class="sxs-lookup"><span data-stu-id="8b368-602">Renamed `--storage-default-filesystem` to `--storage-filesystem`</span></span>
* <span data-ttu-id="8b368-603">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--name` для `application create`, чтобы представлять имя приложения вместо имени кластера.</span><span class="sxs-lookup"><span data-stu-id="8b368-603">[BREAKING CHANGE] Changed the `--name` argument of `application create` to represent the application name instead of the cluster name</span></span>
* <span data-ttu-id="8b368-604">Добавлен аргумент `--cluster-name` для `application create`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-604">Added `--cluster-name` argument to `application create` to replace old `--name` functionality</span></span>
* <span data-ttu-id="8b368-605">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименованы параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="8b368-605">[BREAKING CHANGE] Renamed parameters for `application create`:</span></span>
  * <span data-ttu-id="8b368-606">Переименование `--application-type` в `--type`</span><span class="sxs-lookup"><span data-stu-id="8b368-606">Renamed `--application-type` to `--type`</span></span>
  * <span data-ttu-id="8b368-607">Переименование `--marketplace-identifier` в `--marketplace-id`</span><span class="sxs-lookup"><span data-stu-id="8b368-607">Renamed `--marketplace-identifier` to `--marketplace-id`</span></span>
  * <span data-ttu-id="8b368-608">Переименование `--https-endpoint-access-mode` в `--access-mode`</span><span class="sxs-lookup"><span data-stu-id="8b368-608">Renamed `--https-endpoint-access-mode` to `--access-mode`</span></span>
  * <span data-ttu-id="8b368-609">Переименован аргумент `--https-endpoint-destination-port` на `--destination-port`.</span><span class="sxs-lookup"><span data-stu-id="8b368-609">Renamed  `--https-endpoint-destination-port` to `--destination-port`</span></span>
* <span data-ttu-id="8b368-610">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены параметры для `application create`:</span><span class="sxs-lookup"><span data-stu-id="8b368-610">[BREAKING CHANGE] Removed parameters for `application create`:</span></span>
  * `--https-endpoint-location`
  * `--https-endpoint-public-port`
  * `--ssh-endpoint-destination-port`
  * `--ssh-endpoint-location`
  * `--ssh-endpoint-public-port`
* <span data-ttu-id="8b368-611">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Переименован аргумент `--target-instance-count` на `--workernode-count` для `hdinsight resize`.</span><span class="sxs-lookup"><span data-stu-id="8b368-611">[BREAKING CHNAGE] Renamed `--target-instance-count` to `--workernode-count` for `hdinsight resize`</span></span>
* <span data-ttu-id="8b368-612">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены все команды в группе `hdinsight script-action`, чтобы использовать параметр `--name` в качестве имени действия скрипта.</span><span class="sxs-lookup"><span data-stu-id="8b368-612">[BREAKING CHANGE] Changed all commands in the `hdinsight script-action` group to use the `--name` parameter as the name of the script action.</span></span>
* <span data-ttu-id="8b368-613">Добавлен аргумент `--cluster-name` для всех команд `hdinsight script-action`, чтобы заменить старый аргумент `--name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-613">Added `--cluster-name` argument to all `hdinsight script-action` commands to replace old `--name` functionality</span></span>
* <span data-ttu-id="8b368-614">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименован аргумент `--script-execution-id` на `--execution-id`для всех команд `hdinsight script-action`.</span><span class="sxs-lookup"><span data-stu-id="8b368-614">[BREAKING CHANGE] Renamed `--script-execution-id` to `--execution-id` for all `hdinsight script-action` commands</span></span>
* <span data-ttu-id="8b368-615">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `hdinsight script-action show` переименована в `hdinsight script-action show-execution-details`.</span><span class="sxs-lookup"><span data-stu-id="8b368-615">[BREAKING CHANGE] Renamed `hdinsight script-action show` to `hdinsight script-action show-execution-details`</span></span>
* <span data-ttu-id="8b368-616">[КРИТИЧЕСКОЕ ИЗМЕНЕНИЕ] Изменены параметры для `hdinsight script-action execute --roles`, чтобы они разделялись пробелами, а не запятыми.</span><span class="sxs-lookup"><span data-stu-id="8b368-616">[BREAKING CHNAGE] Changed parameters to `hdinsight script-action execute --roles` to be space-separated instead of comma-separated</span></span>
* <span data-ttu-id="8b368-617">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--persisted` для `hdinsight script-action list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-617">[BREAKING CHANGE] Removed the `--persisted` parameter of `hdinsight script-action list`</span></span>
* <span data-ttu-id="8b368-618">Изменен параметр `hdinsight create --cluster-configurations`, чтобы принимать путь к локальному файлу JSON или строке JSON.</span><span class="sxs-lookup"><span data-stu-id="8b368-618">Changed the `hdinsight create --cluster-configurations` parameter to accept a path to a local JSON file or a JSON string</span></span>
* <span data-ttu-id="8b368-619">Добавлена команда `hdinsight script-action list-execution-history`.</span><span class="sxs-lookup"><span data-stu-id="8b368-619">Added command `hdinsight script-action list-execution-history`</span></span>
* <span data-ttu-id="8b368-620">Изменен параметр `hdinsight monitor enable --workspace`, чтобы принимать идентификатор или имя рабочей области Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="8b368-620">Changed `hdinsight monitor enable --workspace` to accept a Log Analytics workspace ID or workspace name</span></span>
* <span data-ttu-id="8b368-621">Добавлен аргумент `hdinsight monitor enable --primary-key`, который требуется, если в качестве параметра указан идентификатор рабочей области.</span><span class="sxs-lookup"><span data-stu-id="8b368-621">Added the `hdinsight monitor enable --primary-key` argument, which is needed if a workspace ID is provided as the parameter</span></span>
* <span data-ttu-id="8b368-622">Добавлены дополнительные примеры и обновленные описания для справочных сообщений.</span><span class="sxs-lookup"><span data-stu-id="8b368-622">Added more examples and updated descriptions for help messages</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-623">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-623">Interactive</span></span>

* <span data-ttu-id="8b368-624">Исправлена ошибка загрузки.</span><span class="sxs-lookup"><span data-stu-id="8b368-624">Fixed a loading error</span></span>

### <a name="kubernetes"></a><span data-ttu-id="8b368-625">Kubernetes</span><span class="sxs-lookup"><span data-stu-id="8b368-625">Kubernetes</span></span>

* <span data-ttu-id="8b368-626">Теперь используется `https`, если порт контейнера панели мониторинга использует `https`.</span><span class="sxs-lookup"><span data-stu-id="8b368-626">Changed to use `https` if dashboard container port is using `https`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-627">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-627">Network</span></span>

* <span data-ttu-id="8b368-628">Добавлен аргумент `--yes` для `network dns record-set cname delete`.</span><span class="sxs-lookup"><span data-stu-id="8b368-628">Added `--yes` argument `network dns record-set cname delete`</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-629">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-629">Profile</span></span>

* <span data-ttu-id="8b368-630">Добавлен аргумент `--resource-type` для `account get-access-token`, чтобы получать маркеры доступа к ресурсам.</span><span class="sxs-lookup"><span data-stu-id="8b368-630">Added `--resource-type` argument to `account get-access-token` to get resource access tokens</span></span>

### <a name="servicefabric"></a><span data-ttu-id="8b368-631">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8b368-631">ServiceFabric</span></span>

* <span data-ttu-id="8b368-632">Добавлены все поддерживаемые версии ОС для команды sf cluster create.</span><span class="sxs-lookup"><span data-stu-id="8b368-632">Added all supported os version for sf cluster create</span></span>
* <span data-ttu-id="8b368-633">Исправлена ошибка проверки основного сертификата.</span><span class="sxs-lookup"><span data-stu-id="8b368-633">Fixed primary certificate validation bug</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-634">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-634">Storage</span></span>

* <span data-ttu-id="8b368-635">Добавлена команда `storage copy`.</span><span class="sxs-lookup"><span data-stu-id="8b368-635">Added command `storage copy`</span></span>

## <a name="july-30-2019"></a><span data-ttu-id="8b368-636">30 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-636">July 30, 2019</span></span>

<span data-ttu-id="8b368-637">Версия 2.0.70</span><span class="sxs-lookup"><span data-stu-id="8b368-637">Version 2.0.70</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-638">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-638">ACR</span></span>

* <span data-ttu-id="8b368-639">Исправлена проблема № 9952 (регрессия в команде `acr pack build`).</span><span class="sxs-lookup"><span data-stu-id="8b368-639">Fixed issue #9952 (a regression in the `acr pack build` command)</span></span>
* <span data-ttu-id="8b368-640">Удалено имя образа построителя по умолчанию в `acr pack build`.</span><span class="sxs-lookup"><span data-stu-id="8b368-640">Removed the default builder image name in `acr pack build`</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-641">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-641">Appservice</span></span>

* <span data-ttu-id="8b368-642">Команда `webapp config ssl` изменена для отображения сообщения, если ресурс не найден.</span><span class="sxs-lookup"><span data-stu-id="8b368-642">Changed `webapp config ssl` to show a message if a resource is not found</span></span>
* <span data-ttu-id="8b368-643">Исправлена проблема, когда команда `functionapp create` не принимала тип учетной записи хранения `Standard_RAGRS`.</span><span class="sxs-lookup"><span data-stu-id="8b368-643">Fixed issue where `functionapp create` does not accept `Standard_RAGRS` storage account type</span></span>
* <span data-ttu-id="8b368-644">Исправлена проблема, когда команда `webapp up` завершала работу со сбоем в случае выполнения со старой версией Python.</span><span class="sxs-lookup"><span data-stu-id="8b368-644">Fixed an issue where `webapp up` would fail if run using older versions of python</span></span>

### <a name="network"></a><span data-ttu-id="8b368-645">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-645">Network</span></span>

* <span data-ttu-id="8b368-646">Удален недопустимый параметр `--ids` из `network nic ip-config add` (исправление проблемы № 9861).</span><span class="sxs-lookup"><span data-stu-id="8b368-646">Removed invalid parameter `--ids` from `network nic ip-config add` (fixes #9861)</span></span>
* <span data-ttu-id="8b368-647">Исправлена проблема № 9604.</span><span class="sxs-lookup"><span data-stu-id="8b368-647">Fixes #9604.</span></span> <span data-ttu-id="8b368-648">Добавлен параметр `--root-certs` в `network application-gateway http-settings [create|update]` для поддержки связанных с пользователем доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="8b368-648">Added `--root-certs` parameter to `network application-gateway http-settings [create|update]` to support user associate trusted root certificates.</span></span>
* <span data-ttu-id="8b368-649">Исправлен аргумент `--subscription` для `network dns record-set ns create` (проблема № 9965).</span><span class="sxs-lookup"><span data-stu-id="8b368-649">Fixed arguent `--subscription` for `network dns record-set ns create` (#9965)</span></span>

### <a name="rbac"></a><span data-ttu-id="8b368-650">RBAC</span><span class="sxs-lookup"><span data-stu-id="8b368-650">RBAC</span></span>

* <span data-ttu-id="8b368-651">Добавлена команда `user update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-651">Added `user update` command</span></span>
* <span data-ttu-id="8b368-652">[УСТАРЕЛО]`--upn-or-object-id` не рекомендуется использовать в связанных с пользователями командах.</span><span class="sxs-lookup"><span data-stu-id="8b368-652">[DEPRECATED] Deprecated `--upn-or-object-id` from user-related commands</span></span>
    * <span data-ttu-id="8b368-653">Вместо этого применяйте аргумент `--id`.</span><span class="sxs-lookup"><span data-stu-id="8b368-653">Use replacement argument `--id`</span></span>
* <span data-ttu-id="8b368-654">Добавлен аргумент `--id` в связанные с пользователями команды.</span><span class="sxs-lookup"><span data-stu-id="8b368-654">Added `--id` argument to user-related commands</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-655">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-655">SQL</span></span>

* <span data-ttu-id="8b368-656">Добавлены команды управления для ключей и предохранителя TDE управляемого экземпляра.</span><span class="sxs-lookup"><span data-stu-id="8b368-656">Added management commands for managed instance keys and TDE protector</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-657">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-657">Storage</span></span>

* <span data-ttu-id="8b368-658">Добавлена команда `storage remove`.</span><span class="sxs-lookup"><span data-stu-id="8b368-658">Added `storage remove` command</span></span>
* <span data-ttu-id="8b368-659">Исправлена проблема с `storage blob update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-659">Fixed an issue with `storage blob update`</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-660">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-660">VM</span></span>

* <span data-ttu-id="8b368-661">Изменена команда `list-skus` для использования новой версии API для вывода сведений о зонах.</span><span class="sxs-lookup"><span data-stu-id="8b368-661">Changed `list-skus` to use newer api-version to output zone details</span></span>
* <span data-ttu-id="8b368-662">Изменено значение по умолчанию параметра `--single-placement-group` на `false` для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-662">Changed default of `--single-placement-group` to `false` for `vmss create`</span></span>
* <span data-ttu-id="8b368-663">Добавлена возможность выбирать номера SKU хранилища ZRS для `[snapshot|disk] create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-663">Added ability to select ZRS storage SKUs for `[snapshot|disk] create`</span></span>
* <span data-ttu-id="8b368-664">Добавлена новая группа команд `vm host` для поддержки выделенных узлов.</span><span class="sxs-lookup"><span data-stu-id="8b368-664">Added new command group `vm host` to support dedicated hosts</span></span>
* <span data-ttu-id="8b368-665">Добавлены параметры `--host` и `--host-group` в команде `vm create` для указания выделенного узла виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="8b368-665">Added parameters `--host` and `--host-group` on `vm create` to set VM dedicated host</span></span>

## <a name="july-16-2019"></a><span data-ttu-id="8b368-666">16 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-666">July 16, 2019</span></span>

<span data-ttu-id="8b368-667">Версия 2.0.69</span><span class="sxs-lookup"><span data-stu-id="8b368-667">Version 2.0.69</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-668">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-668">Appservice</span></span>

* <span data-ttu-id="8b368-669">Изменены команды `webapp identity`. Теперь они возвращают правильное сообщение об ошибке, если параметр ResourceGroupName или имя приложения недопустимы.</span><span class="sxs-lookup"><span data-stu-id="8b368-669">Changed `webapp identity` commands to return a proper error message if ResourceGroupName or App name are invalid</span></span>
* <span data-ttu-id="8b368-670">Исправлена команда `webapp list`. Теперь она возвращает правильное значение для параметра numberOfSites, если не указан параметр ResourceGroup.</span><span class="sxs-lookup"><span data-stu-id="8b368-670">Fixed `webapp list` to return the correct value for numberOfSites if no ResourceGroup was provided</span></span>
* <span data-ttu-id="8b368-671">Исправлены побочные эффекты для команд `appservice plan create` и `webapp create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-671">Fixed side-effects of `appservice plan create` and `webapp create`</span></span>

### <a name="core"></a><span data-ttu-id="8b368-672">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-672">Core</span></span>

* <span data-ttu-id="8b368-673">Исправлена ошибка, при которой отображался параметр `--subscription`, хотя он был неприменим.</span><span class="sxs-lookup"><span data-stu-id="8b368-673">Fixed issue where `--subscription` would appear despite being not applicable</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-674">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-674">Batch</span></span>

* <span data-ttu-id="8b368-675">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `batch pool node-agent-skus list` заменена на `batch pool supported-images list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-675">[BREAKING CHANGE] Replaced `batch pool node-agent-skus list` with `batch pool supported-images list`</span></span>
* <span data-ttu-id="8b368-676">Добавлена поддержка правил безопасности, которые блокируют сетевой доступ к пулу на основе исходного порта трафика при использовании параметра `--json-file` команды `batch pool create network`.</span><span class="sxs-lookup"><span data-stu-id="8b368-676">Added support for security rules blocking network access to a pool based on the source port of the traffic when using the `--json-file` option of `batch pool create network`</span></span>
* <span data-ttu-id="8b368-677">Добавлена поддержка выполнения задачи в рабочей папке контейнера или рабочей папке задачи пакета при использовании параметра `--json-file` команды `batch task create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-677">Added support for executing the task in the container working directory or in the Batch task working directory when using the `--json-file` option of `batch task create`</span></span>
* <span data-ttu-id="8b368-678">Исправлена ошибка в параметре `--application-package-references` команды `batch pool create`, которая позволяла работать только со значениями по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-678">Fixed error in `--application-package-references` option of `batch pool create` where it would only work with defaults</span></span>

### <a name="eventhubs"></a><span data-ttu-id="8b368-679">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="8b368-679">Eventhubs</span></span>

* <span data-ttu-id="8b368-680">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="8b368-680">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-681">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="8b368-681">RDBMS</span></span>

* <span data-ttu-id="8b368-682">Добавлен необязательный параметр для указания номера SKU реплики в команде создания реплики.</span><span class="sxs-lookup"><span data-stu-id="8b368-682">Added optional parameter to specify replica SKU for create replica command</span></span>
* <span data-ttu-id="8b368-683">Исправлена ошибка теста CI при создании реплики MySQL.</span><span class="sxs-lookup"><span data-stu-id="8b368-683">Fixed the issue with CI test failure with creating MySQL replica</span></span>

### <a name="relay"></a><span data-ttu-id="8b368-684">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="8b368-684">Relay</span></span>

* <span data-ttu-id="8b368-685">Исправлена проблема с гибридным подключением при выключенной авторизации клиента ([8775](https://github.com/azure/azure-cli/issues/8775)).</span><span class="sxs-lookup"><span data-stu-id="8b368-685">Fixed issue with hybrid connection when client authroization disabled [#8775](https://github.com/azure/azure-cli/issues/8775)</span></span>
* <span data-ttu-id="8b368-686">Добавлен параметр `--requires-transport-security` для команды `relay wcfrelay create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-686">Added parameter `--requires-transport-security` to `relay wcfrelay create`</span></span>

### <a name="servicebus"></a><span data-ttu-id="8b368-687">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="8b368-687">Servicebus</span></span>

* <span data-ttu-id="8b368-688">Добавлена проверка параметра `--rights` команд `authorizationrule`.</span><span class="sxs-lookup"><span data-stu-id="8b368-688">Added validation for parameter `--rights` of `authorizationrule` commands</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-689">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-689">Storage</span></span>

* <span data-ttu-id="8b368-690">Добавлена возможность обновления учетной записи хранения для AADDS в службе "Файлы".</span><span class="sxs-lookup"><span data-stu-id="8b368-690">Enable Files AADDS for storage account update</span></span>
* <span data-ttu-id="8b368-691">Устранена проблема, описанная здесь: `storage blob service-properties update --set`.</span><span class="sxs-lookup"><span data-stu-id="8b368-691">Fixed issue `storage blob service-properties update --set`</span></span>

## <a name="july-2-2019"></a><span data-ttu-id="8b368-692">2 июля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-692">July 2, 2019</span></span>

<span data-ttu-id="8b368-693">Версия 2.0.68</span><span class="sxs-lookup"><span data-stu-id="8b368-693">Version 2.0.68</span></span>

### <a name="core"></a><span data-ttu-id="8b368-694">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-694">Core</span></span>

* <span data-ttu-id="8b368-695">Командные модули теперь объединены в один распространяемый пакет Python.</span><span class="sxs-lookup"><span data-stu-id="8b368-695">Command modules are now consolidated into a single Python distributable.</span></span> <span data-ttu-id="8b368-696">В результате этого прекращается непосредственное использование множества пакетов `azure-cli-` в PyPI.</span><span class="sxs-lookup"><span data-stu-id="8b368-696">This deprecates direct use of many `azure-cli-` packages on PyPI.</span></span>
  <span data-ttu-id="8b368-697">Это также должно уменьшить размер установки и повлияет только на пользователей, которые выполняли установку непосредственно через `pip`.</span><span class="sxs-lookup"><span data-stu-id="8b368-697">This should reduce install size and only affect users who have directly installed via `pip`.</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-698">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-698">ACR</span></span>

* <span data-ttu-id="8b368-699">В заданиях добавлена поддержка триггеров таймера.</span><span class="sxs-lookup"><span data-stu-id="8b368-699">Added support for Timer Triggers to Task</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-700">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-700">Appservice</span></span>

* <span data-ttu-id="8b368-701">Внесены изменения в `functionapp create` для включения Application Insights по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-701">Changed `functionapp create` to enable application insights by default</span></span>
* <span data-ttu-id="8b368-702">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена устаревшая команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="8b368-702">[BREAKING CHANGE] Removed deprecated `functionapp devops-build` command.</span></span>
  *  <span data-ttu-id="8b368-703">Вместо нее используйте новую команду `az functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="8b368-703">Use the new command `az functionapp devops-pipeline` instead</span></span>
* <span data-ttu-id="8b368-704">В `functionapp deployment config-zip` добавлена поддержка плана потребления приложения-функции Linux.</span><span class="sxs-lookup"><span data-stu-id="8b368-704">Added Linux Consumption function app plan support to `functionapp deployment config-zip`</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="8b368-705">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-705">Cosmos DB</span></span>

* <span data-ttu-id="8b368-706">Добавлена возможность отключения TTL.</span><span class="sxs-lookup"><span data-stu-id="8b368-706">Added support for disabling TTL</span></span>

### <a name="dls"></a><span data-ttu-id="8b368-707">DLS</span><span class="sxs-lookup"><span data-stu-id="8b368-707">DLS</span></span>

* <span data-ttu-id="8b368-708">Обновленная версия ADLS (0.0.45)</span><span class="sxs-lookup"><span data-stu-id="8b368-708">Updated ADLS version (0.0.45)</span></span>

### <a name="feedback"></a><span data-ttu-id="8b368-709">Отзывы</span><span class="sxs-lookup"><span data-stu-id="8b368-709">Feedback</span></span>

* <span data-ttu-id="8b368-710">При сообщении о сбое при выполнении команды расширения `az feedback` теперь пытается открыть браузер по URL-адресу репозитория или проекта расширения из индекса.</span><span class="sxs-lookup"><span data-stu-id="8b368-710">When reporting a failed extension command, `az feedback` now attempts to open the browser to the project/repo url of the extension from the index</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8b368-711">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b368-711">HDInsight</span></span>

* <span data-ttu-id="8b368-712">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Имя группы команд `oms` изменилось на `monitor`.</span><span class="sxs-lookup"><span data-stu-id="8b368-712">[BREAKING CHANGE] Changed `oms` command group name to `monitor`</span></span>
* <span data-ttu-id="8b368-713">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--http-password/-p` стал обязательным.</span><span class="sxs-lookup"><span data-stu-id="8b368-713">[BREAKING CHANGE] Made `--http-password/-p` a required parameter</span></span> 
* <span data-ttu-id="8b368-714">Добавлены средства заполнения для `--cluster-admin-account` и средство заполнения для параметров `cluster-users-group-dns`.</span><span class="sxs-lookup"><span data-stu-id="8b368-714">Added completers for `--cluster-admin-account` and `cluster-users-group-dns` parameters completer</span></span> 
* <span data-ttu-id="8b368-715">Параметр `cluster-users-group-dns` стал обязательным, если присутствует `—esp`.</span><span class="sxs-lookup"><span data-stu-id="8b368-715">Changed `cluster-users-group-dns` parameter to be required when `—esp` is present</span></span>
* <span data-ttu-id="8b368-716">Добавлено время ожидания для всех существующих средств автоматического заполнения аргументов.</span><span class="sxs-lookup"><span data-stu-id="8b368-716">Added a timeout for all existing argument auto-completers</span></span>
* <span data-ttu-id="8b368-717">Добавлено время ожидания для преобразования имени ресурса в идентификатор ресурса.</span><span class="sxs-lookup"><span data-stu-id="8b368-717">Added a timeout for transforming resource name to resource id</span></span>
* <span data-ttu-id="8b368-718">Внесены изменения в средства автоматического заполнения для выбора ресурсов из любой группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-718">Changed Auto-completers to select resources from any resource group.</span></span> <span data-ttu-id="8b368-719">Это может быть группа ресурсов, отличная от той, которая указана с помощью `-g`.</span><span class="sxs-lookup"><span data-stu-id="8b368-719">It can be a different resource group than the one specified with `-g`</span></span>
* <span data-ttu-id="8b368-720">Добавлена поддержка параметров `--sub-domain-suffix` и `--disable_gateway_auth` в команде `hdinsight application create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-720">Added support for `--sub-domain-suffix` and `--disable_gateway_auth` parameters in the `hdinsight application create` command</span></span>

### <a name="managed-services"></a><span data-ttu-id="8b368-721">Управляемые службы</span><span class="sxs-lookup"><span data-stu-id="8b368-721">Managed Services</span></span>

* <span data-ttu-id="8b368-722">Командный модуль управляемых служб выпущен в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="8b368-722">Introducing managed service command module in preview</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-723">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-723">Profile</span></span>
* <span data-ttu-id="8b368-724">Аргумент `--subscription` подавляется для команды выхода.</span><span class="sxs-lookup"><span data-stu-id="8b368-724">Suppress `--subscription` argument for logout command</span></span>

### <a name="rbac"></a><span data-ttu-id="8b368-725">RBAC</span><span class="sxs-lookup"><span data-stu-id="8b368-725">RBAC</span></span>

* <span data-ttu-id="8b368-726">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален аргумент `--password` для `create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="8b368-726">[BREAKING CHANGE] Removed `--password` argument for `create-for-rbac`</span></span>
* <span data-ttu-id="8b368-727">В команду `create` добавлен параметр `--assignee-principal-type` для устранения периодических сбоев из-за задержки репликации сервера AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="8b368-727">Added `--assignee-principal-type` parameter to `create` command to avoid intermittent failures caused by AAD graph server replication latency</span></span>
* <span data-ttu-id="8b368-728">Исправлен сбой в `ad signed-in-user` при перечислении собственных объектов.</span><span class="sxs-lookup"><span data-stu-id="8b368-728">Fixed a crash in `ad signed-in-user` when listing owned objects</span></span>
* <span data-ttu-id="8b368-729">Исправлена проблема, при которой `ad sp` не удавалось найти нужное приложение в субъекте-службе.</span><span class="sxs-lookup"><span data-stu-id="8b368-729">Fixed issue where `ad sp` would not find the right application from a service principal</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-730">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="8b368-730">RDBMS</span></span>

* <span data-ttu-id="8b368-731">Добавлена поддержка репликации MariaDB.</span><span class="sxs-lookup"><span data-stu-id="8b368-731">Added support for replication for MariaDB</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-732">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-732">SQL</span></span>

* <span data-ttu-id="8b368-733">Описаны допустимые значения для `sql db create --sample-name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-733">Documented allowed values for `sql db create --sample-name`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-734">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-734">Storage</span></span>

* <span data-ttu-id="8b368-735">В `storage blob generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="8b368-735">Added user delegation SAS token support with `--as-user` to `storage blob generate-sas`</span></span> 
* <span data-ttu-id="8b368-736">В `storage container generate-sas` добавлена поддержка маркера SAS для делегирования пользователя с помощью `--as-user`.</span><span class="sxs-lookup"><span data-stu-id="8b368-736">Added user delegation SAS token support with `--as-user` to `storage container generate-sas`</span></span> 

### <a name="vm"></a><span data-ttu-id="8b368-737">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-737">VM</span></span>

* <span data-ttu-id="8b368-738">Исправлена ошибка, при которой команда `vmss create` возвращала сообщение об ошибке при выполнении с `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-738">Fixed bug where `vmss create` returns an error message when run with `--no-wait`</span></span>
* <span data-ttu-id="8b368-739">Прекращена проверка `vmss create --single-placement-group` на стороне клиента.</span><span class="sxs-lookup"><span data-stu-id="8b368-739">Removed client-side validation for `vmss create --single-placement-group`.</span></span> <span data-ttu-id="8b368-740">Команда не завершается сбоем, если для `--single-placement-group` задано значение `true`, а значение `--instance-count` больше 100 или указаны зоны доступности. Сама проверка теперь выполняется службой вычислений.</span><span class="sxs-lookup"><span data-stu-id="8b368-740">Does not fail if `--single-placement-group` is set to `true` and`--instance-count` is greater than 100 or availability zones are specified, but leaves this validation to the compute service</span></span>
* <span data-ttu-id="8b368-741">Исправлена ошибка, при которой команда `[vm|vmss] extension image list` завершалась сбоем при указании `--latest`.</span><span class="sxs-lookup"><span data-stu-id="8b368-741">Fixed bug where `[vm|vmss] extension image list` fails when used with `--latest`</span></span>


## <a name="june-18-2019"></a><span data-ttu-id="8b368-742">18 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-742">June 18, 2019</span></span>

<span data-ttu-id="8b368-743">Версия 2.0.67</span><span class="sxs-lookup"><span data-stu-id="8b368-743">Version 2.0.67</span></span>

### <a name="core"></a><span data-ttu-id="8b368-744">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-744">Core</span></span>

<span data-ttu-id="8b368-745">В этом выпуске добавлен новый тег [Предварительная версия], который яснее дает понять, что группа команд, команда или аргумент находятся в состоянии предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="8b368-745">This release introduces a new [Preview] tag to more clearly communicate to customers when a command group, command or argument is in preview status.</span></span> <span data-ttu-id="8b368-746">Ранее это указывалось в тексте справки или подразумевалось в номере версии командного модуля.</span><span class="sxs-lookup"><span data-stu-id="8b368-746">This was previously called out in help text or communicated implicitly by the command module version number.</span></span>
<span data-ttu-id="8b368-747">В будущем в интерфейсе командной строки номера версий отдельных пакетов не будут указываться.</span><span class="sxs-lookup"><span data-stu-id="8b368-747">The CLI will be removing version numbers for individual packages in the future.</span></span> <span data-ttu-id="8b368-748">Если команда доступна в предварительной версии, это также касается и всех ее аргументов.</span><span class="sxs-lookup"><span data-stu-id="8b368-748">If a command is in preview, all of its arguments are as well.</span></span> <span data-ttu-id="8b368-749">Если группа команд помечается как находящаяся в предварительной версии, значит все команды и аргументы также считаются доступными в предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="8b368-749">If a command group is labeled as being in preview, then all commands and arguments are considered to be in preview as well.</span></span>

<span data-ttu-id="8b368-750">В результате этого изменения несколько групп команд могут "внезапно" оказаться в состоянии предварительной версии в этом выпуске.</span><span class="sxs-lookup"><span data-stu-id="8b368-750">As a result of this change, several command groups may seem to "suddenly" appear to be in a preview status with this release.</span></span> <span data-ttu-id="8b368-751">В действительности большинство пакетов, которые находились в состоянии предварительной версии, в этом выпуске будут считаться общедоступными.</span><span class="sxs-lookup"><span data-stu-id="8b368-751">What actually happened is that most packages were in a preview status, but are being deemed GA with this release</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-752">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-752">ACR</span></span>
* <span data-ttu-id="8b368-753">Добавлена команда acr check-health.</span><span class="sxs-lookup"><span data-stu-id="8b368-753">Added 'acr check-health' command</span></span>
* <span data-ttu-id="8b368-754">Улучшена обработка ошибок с маркерами безопасности AAD и ошибок при получении внешних команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-754">Improved error handling for AAD tokens and for retrieving external commands</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-755">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-755">ACS</span></span>
* <span data-ttu-id="8b368-756">Устаревшие команды ACS теперь скрыты в тексте справки.</span><span class="sxs-lookup"><span data-stu-id="8b368-756">Deprecated ACS commands are now hidden from help view</span></span>

### <a name="ams"></a><span data-ttu-id="8b368-757">AMS</span><span class="sxs-lookup"><span data-stu-id="8b368-757">AMS</span></span>
* <span data-ttu-id="8b368-758">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в возврате строк времени ISO 8601 для archive-window-length и key-frame-interval-duration.</span><span class="sxs-lookup"><span data-stu-id="8b368-758">[BREAKING CHANGE] Changed to return ISO 8601 time strings for archive-window-length and key-frame-interval-duration</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-759">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-759">AppService</span></span>
* <span data-ttu-id="8b368-760">Добавлена маршрутизация на основе расположение для `webapp deleted list` и `webapp deleted restore`.</span><span class="sxs-lookup"><span data-stu-id="8b368-760">Added location based routing for `webapp deleted list` and `webapp deleted restore`</span></span>
* <span data-ttu-id="8b368-761">Исправлена проблема, при которой целевой URL-адрес веб-приложения ("Вы можете запустить приложение в...") не был активным в Azure Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="8b368-761">Fixed issue where webapp up logged target URL ("You can launch the app at...") was not clickable in Azure Cloud Shell</span></span>
* <span data-ttu-id="8b368-762">Устранена проблема, при которой создание приложений в некоторых SKU завершалось сбоем с ошибкой AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="8b368-762">Fixed an issue where creating apps with the some SKUs was failing with an AlwaysOn error</span></span>
* <span data-ttu-id="8b368-763">Добавлена предварительная проверка в `[appservice|webapp] create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-763">Added pre-validation to `[appservice|webapp] create`</span></span>
* <span data-ttu-id="8b368-764">Исправлено `[webapp|functionapp] traffic-routing` для использования правильного actionHostName.</span><span class="sxs-lookup"><span data-stu-id="8b368-764">Fixed `[webapp|functionapp] traffic-routing` to use the correct actionHostName</span></span>
* <span data-ttu-id="8b368-765">Добавлена поддержка слотов для команд `functionapp`.</span><span class="sxs-lookup"><span data-stu-id="8b368-765">Added slot support to `functionapp` commands</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-766">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-766">Batch</span></span>
* <span data-ttu-id="8b368-767">Исправлена регрессия проверки подлинности AAD, которую вызывал чрезмерный поток уведомлений об авторизации с помощью общего ключа.</span><span class="sxs-lookup"><span data-stu-id="8b368-767">Fixed AAD auth regression caused by over-aggressive error reporting for Shared Key Auth</span></span>

### <a name="batchai"></a><span data-ttu-id="8b368-768">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8b368-768">BatchAI</span></span>
* <span data-ttu-id="8b368-769">Команды BatchAI теперь признаны устаревшими и скрыты.</span><span class="sxs-lookup"><span data-stu-id="8b368-769">BatchAI commands are now deprecated and hidden</span></span>

### <a name="botservice"></a><span data-ttu-id="8b368-770">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-770">BotService</span></span>
* <span data-ttu-id="8b368-771">Добавлены предупреждающие сообщения о прекращении поддержки и режиме обслуживания для команд, которые поддерживают пакет SDK версии 3.</span><span class="sxs-lookup"><span data-stu-id="8b368-771">Added "discontinued support"/"maintenance mode" warning messages for commands that support the v3 SDK</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8b368-772">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-772">CosmosDB</span></span>
* <span data-ttu-id="8b368-773">[УСТАРЕЛО] использовать команду `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="8b368-773">[DEPRECATED] Deprecated the `cosmosdb list-keys` command</span></span>
* <span data-ttu-id="8b368-774">Добавлена команда `cosmosdb keys list`, заменяющая `cosmosdb list-keys`.</span><span class="sxs-lookup"><span data-stu-id="8b368-774">Added the `cosmosdb keys list` command - replaces `cosmosdb list-keys`</span></span>
* <span data-ttu-id="8b368-775">`cosmsodb create/update`: Добавлен новый формат для --location, который позволяет задавать свойство isZoneRedundant.</span><span class="sxs-lookup"><span data-stu-id="8b368-775">`cosmsodb create/update`: Added new format for --location to allow setting "isZoneRedundant" property.</span></span> <span data-ttu-id="8b368-776">Нерекомендуемый старый формат.</span><span class="sxs-lookup"><span data-stu-id="8b368-776">Deprecated old format</span></span>

### <a name="eventgrid"></a><span data-ttu-id="8b368-777">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="8b368-777">EventGrid</span></span>
* <span data-ttu-id="8b368-778">Добавлены команды `eventgrid domain` для операций CRUD домена.</span><span class="sxs-lookup"><span data-stu-id="8b368-778">Added `eventgrid domain` commands for domain CRUD operations</span></span>
* <span data-ttu-id="8b368-779">Добавлены команды `eventgrid domain topic` для операций CRUD разделов домена.</span><span class="sxs-lookup"><span data-stu-id="8b368-779">Added `eventgrid domain topic` commands for domain topics CRUD operations</span></span>
* <span data-ttu-id="8b368-780">В `eventgrid [topic|event-subscription] list` добавлен аргумент `--odata-query` для фильтрации результатов с использованием синтаксиса OData.</span><span class="sxs-lookup"><span data-stu-id="8b368-780">Added `--odata-query` argument to `eventgrid [topic|event-subscription] list` for filtering results using OData syntax</span></span>
* <span data-ttu-id="8b368-781">`event-subscription create/update`: Добавлена ServiceBusQueue в качестве новых значений для параметра `--endpoint-type`.</span><span class="sxs-lookup"><span data-stu-id="8b368-781">`event-subscription create/update`: Added servicebusqueue as new values for the `--endpoint-type` parameter</span></span>
* <span data-ttu-id="8b368-782">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.], состоящее в прекращении поддержки `--included-event-types All` с `eventgrid event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-782">[BREAKING CHANGE] Removed support for `--included-event-types All` with `eventgrid event-subscription [create|update]`</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8b368-783">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b368-783">HDInsight</span></span>
* <span data-ttu-id="8b368-784">Добавлена поддержка параметра `--ssh-public-key` в команде `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-784">Added support for `--ssh-public-key` parameter in `hdinsight create` command</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-785">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-785">IoT</span></span>
* <span data-ttu-id="8b368-786">Добавлена поддержка для повторного создания ключей политики авторизации.</span><span class="sxs-lookup"><span data-stu-id="8b368-786">Added support to regenerate authorization policy keys</span></span>
* <span data-ttu-id="8b368-787">Добавлен пакет SDK и поддержка для службы подготовки репозитория DigitalTwin.</span><span class="sxs-lookup"><span data-stu-id="8b368-787">Added SDK and support for DigitalTwin Repository Provisioning Service</span></span>

### <a name="network"></a><span data-ttu-id="8b368-788">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-788">Network</span></span>
* <span data-ttu-id="8b368-789">Добавлена поддержка зон для Шлюза NAT.</span><span class="sxs-lookup"><span data-stu-id="8b368-789">Added Zone support for Nat Gateway</span></span>
* <span data-ttu-id="8b368-790">Добавлена команда `network list-service-tags`.</span><span class="sxs-lookup"><span data-stu-id="8b368-790">Added command `network list-service-tags`</span></span>
* <span data-ttu-id="8b368-791">Исправлена проблема с `dns zone import`, при которой пользователям не удавалось импортировать записи А с подстановочным знаком.</span><span class="sxs-lookup"><span data-stu-id="8b368-791">Fixed issue with `dns zone import` where users could not import wildcard A records</span></span>
* <span data-ttu-id="8b368-792">Исправлена проблема с `watcher flow-log configure`, при которой не удавалось включить ведение журнала потоков в определенных регионах.</span><span class="sxs-lookup"><span data-stu-id="8b368-792">Fixed issue with `watcher flow-log configure` where flow logging could not be enabled in certain regions</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-793">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-793">Resource</span></span>
* <span data-ttu-id="8b368-794">Добавлена команда `az rest` для вызовов REST.</span><span class="sxs-lookup"><span data-stu-id="8b368-794">Added `az rest` command for making REST calls</span></span>
* <span data-ttu-id="8b368-795">Исправлена ошибка, возникавшая при использовании `policy assignment list` с группой ресурсов или уровнем подписки `--scope`.</span><span class="sxs-lookup"><span data-stu-id="8b368-795">Fixed error when using `policy assignment list` with a resource group or subscription level `--scope`</span></span>

### <a name="servicebus"></a><span data-ttu-id="8b368-796">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="8b368-796">ServiceBus</span></span>
* <span data-ttu-id="8b368-797">Устранена проблема № [9319](https://github.com/azure/azure-cli/issues/9319) с `servicebus topic create --max-size`.</span><span class="sxs-lookup"><span data-stu-id="8b368-797">Fixed issue with `servicebus topic create --max-size` [#9319](https://github.com/azure/azure-cli/issues/9319)</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-798">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-798">SQL</span></span>
* <span data-ttu-id="8b368-799">Параметр `--location` стал необязательным для `sql [server|mi] create`. Если он не указан, используется расположение группы ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-799">Changed `--location` to be optional for `sql [server|mi] create` - uses resource group location if not specified</span></span>
* <span data-ttu-id="8b368-800">Исправлена ошибка "Объект NoneType не подлежит итерации" с `sql db list-editions --available`.</span><span class="sxs-lookup"><span data-stu-id="8b368-800">Fixed "'NoneType' object is not iterable" error for `sql db list-editions --available`</span></span>

### <a name="sqlvm"></a><span data-ttu-id="8b368-801">SQLVm</span><span class="sxs-lookup"><span data-stu-id="8b368-801">SQLVm</span></span>
* <span data-ttu-id="8b368-802">Критическое изменение. Для `sql vm create` теперь требуется параметр `--license-type`.</span><span class="sxs-lookup"><span data-stu-id="8b368-802">[BREAKING CHNAGE] Changed `sql vm create` to require `--license-type` parameter</span></span>
* <span data-ttu-id="8b368-803">Внесены изменения, позволяющие задавать SKU образа SQL при создании или обновлении виртуальной машины SQL.</span><span class="sxs-lookup"><span data-stu-id="8b368-803">Changed to allow setting SQL image SKU when creating or updating a sql vm</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-804">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-804">Storage</span></span>
* <span data-ttu-id="8b368-805">Исправлена проблема с отсутствующим ключом учетной записи для `storage container generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="8b368-805">Fixed issue with missing account key for `storage container generate-sas`</span></span>
* <span data-ttu-id="8b368-806">Исправлена проблема с `storage blob sync` на платформе Linux.</span><span class="sxs-lookup"><span data-stu-id="8b368-806">Fixed issue with `storage blob sync` on Linux</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-807">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-807">VM</span></span>
* <span data-ttu-id="8b368-808">[Предварительная версия] Добавлены команды `vm image template` для создания образов виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="8b368-808">[PREVIEW] Added `vm image template` commands to build VM images</span></span>

## <a name="june-4-2019"></a><span data-ttu-id="8b368-809">4 июня 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-809">June 4, 2019</span></span>

<span data-ttu-id="8b368-810">Версия 2.0.66</span><span class="sxs-lookup"><span data-stu-id="8b368-810">Version 2.0.66</span></span>

### <a name="core"></a><span data-ttu-id="8b368-811">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-811">Core</span></span>
* <span data-ttu-id="8b368-812">Исправлена ошибка, из-за которой выполнение команды завершалось со сбоем, если параметр `--output yaml` использовался с параметром `--query`</span><span class="sxs-lookup"><span data-stu-id="8b368-812">Fixed bug where commands fail if `--output yaml` is used with `--query`</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-813">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-813">ACR</span></span>
* <span data-ttu-id="8b368-814">Добавлена группа команд acr pack для создания заданий быстрой сборки с помощью пакетов сборок.</span><span class="sxs-lookup"><span data-stu-id="8b368-814">Added 'acr pack' command group for creating quick build Tasks using Buildpacks.</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-815">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-815">ACS</span></span>
* <span data-ttu-id="8b368-816">Разрешено включение и отключение надстройки панели мониторинга Kubernetes для AKS.</span><span class="sxs-lookup"><span data-stu-id="8b368-816">Allow enabling/disabling AKS kube-dashboard addon</span></span>
* <span data-ttu-id="8b368-817">Если подписку нельзя использовать с Azure Red Hat OpenShift, будет отображаться соответствующее сообщение.</span><span class="sxs-lookup"><span data-stu-id="8b368-817">Print a friendly message when the subscription is not whitelisted to use Azure Red Hat OpenShift</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-818">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-818">Batch</span></span>
* <span data-ttu-id="8b368-819">Улучшена обработка ошибок, если не выполнен вход в учетную запись \[[№ 9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[№ 8978](https://github.com/Azure/azure-cli/issues/8978)\].</span><span class="sxs-lookup"><span data-stu-id="8b368-819">Improved error handling when not logged in to an account \[[#9165](https://github.com/Azure/azure-cli/issues/9165)\]\[[#8978](https://github.com/Azure/azure-cli/issues/8978)\]</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-820">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-820">IoT</span></span>
* <span data-ttu-id="8b368-821">Добавлена поддержка для перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="8b368-821">Added support for manual failover</span></span>

### <a name="network"></a><span data-ttu-id="8b368-822">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-822">Network</span></span>
* <span data-ttu-id="8b368-823">Добавлены команды `network application-gateway waf-policy` для поддержки настраиваемых правил WAF.</span><span class="sxs-lookup"><span data-stu-id="8b368-823">Added `network application-gateway waf-policy` commands to support custom WAF rules.</span></span>
* <span data-ttu-id="8b368-824">Добавлены аргументы `--waf-policy` и `--max-capacity` для команды `network application-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8b368-824">Added `--waf-policy` and `--max-capacity` arguments to `network application-gateway [create|update]`</span></span> 

### <a name="resource"></a><span data-ttu-id="8b368-825">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-825">Resource</span></span>
* <span data-ttu-id="8b368-826">Улучшен вывод сообщения команды `deployment create` при отсутствии TTY.</span><span class="sxs-lookup"><span data-stu-id="8b368-826">Improved error message from `deployment create` when there is no TTY available</span></span>

### <a name="role"></a><span data-ttu-id="8b368-827">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-827">Role</span></span>
* <span data-ttu-id="8b368-828">Обновлен текст справки.</span><span class="sxs-lookup"><span data-stu-id="8b368-828">Updated help text.</span></span>

### <a name="compute"></a><span data-ttu-id="8b368-829">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="8b368-829">Compute</span></span>
* <span data-ttu-id="8b368-830">Добавлена поддержка команды `vm create` для создания виртуальных машин из управляемого образа с номерами LUN дисков данных, которые не начинаются с 0 или для которых пропущены номера.</span><span class="sxs-lookup"><span data-stu-id="8b368-830">Added support to `vm create` for VMs from a managed image with data-disk luns that do not start from 0 or that skip numbers</span></span>

## <a name="may-21-2019"></a><span data-ttu-id="8b368-831">21 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-831">May 21, 2019</span></span>

<span data-ttu-id="8b368-832">Версия 2.0.65</span><span class="sxs-lookup"><span data-stu-id="8b368-832">Version 2.0.65</span></span>

### <a name="core"></a><span data-ttu-id="8b368-833">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-833">Core</span></span>
* <span data-ttu-id="8b368-834">Улучшена функция обратной связи при ошибках аутентификации.</span><span class="sxs-lookup"><span data-stu-id="8b368-834">Added better feedback for authentication errors</span></span>
* <span data-ttu-id="8b368-835">Исправлена проблема, из-за которой интерфейс командной строки загружал расширения, которые не были совместимы с его базовой версией.</span><span class="sxs-lookup"><span data-stu-id="8b368-835">Fixed issue where the CLI would load extensions that were not compatible with its core version</span></span>
* <span data-ttu-id="8b368-836">Исправлена проблема с запуском и неисправностью `clouds.config`.</span><span class="sxs-lookup"><span data-stu-id="8b368-836">Fixed issue with launching when `clouds.config` is corrupted</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-837">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-837">ACR</span></span>
* <span data-ttu-id="8b368-838">Добавлена поддержка управляемых удостоверений в Задачи.</span><span class="sxs-lookup"><span data-stu-id="8b368-838">Added support for Managed Identities to Tasks</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-839">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-839">ACS</span></span>
* <span data-ttu-id="8b368-840">Исправлена команда `openshift create`, используемая с пользовательским клиентом AAD.</span><span class="sxs-lookup"><span data-stu-id="8b368-840">Fixed `openshift create` command when used with customer AAD client</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-841">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-841">AppService</span></span>
* <span data-ttu-id="8b368-842">[УСТАРЕЛО] Команда `functionapp devops-build` устарела и будет удалена в следующем выпуске.</span><span class="sxs-lookup"><span data-stu-id="8b368-842">[DEPRECATED] Deprecated `functionapp devops-build` command - will be removed in next release</span></span>
* <span data-ttu-id="8b368-843">Внесено изменение в `functionapp devops-pipeline` для получения журнала сборки из Azure DevOps в режиме подробного протоколирования.</span><span class="sxs-lookup"><span data-stu-id="8b368-843">Changed `functionapp devops-pipeline` to fetch build log from Azure DevOps in verbose mode</span></span>
* <span data-ttu-id="8b368-844">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален неподдерживаемый флаг `--use_local_settings` из команды `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="8b368-844">[BREAKING CHANGE] Removed `--use_local_settings` flag from `functionapp devops-pipeline` command - was a no-op</span></span>
* <span data-ttu-id="8b368-845">Внесено изменение в `webapp up` для возврата выходных данных JSON, если `--logs` не используется.</span><span class="sxs-lookup"><span data-stu-id="8b368-845">Changed `webapp up` to return JSON output if `--logs` is not used</span></span>
* <span data-ttu-id="8b368-846">Добавлена поддержка записи ресурсов по умолчанию в локальную конфигурацию для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="8b368-846">Added support for writing default resources to local config for `webapp up`</span></span>
* <span data-ttu-id="8b368-847">Добавлена поддержка `webapp up` для повторного развертывания приложения без использования аргумента `--location`.</span><span class="sxs-lookup"><span data-stu-id="8b368-847">Added support to `webapp up` for redeploying an app without using the `--location` argument</span></span>
* <span data-ttu-id="8b368-848">Устранена проблема, из-за которой нельзя было создать для Linux номер SKU с планом службы приложений "Бесплатный".</span><span class="sxs-lookup"><span data-stu-id="8b368-848">Fixed an issue where for Linux Free SKU ASP creation use Free as SKU value was not working</span></span>

### <a name="botservice"></a><span data-ttu-id="8b368-849">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-849">BotService</span></span>
* <span data-ttu-id="8b368-850">Внесено изменение для включения поддержки всех регистров в параметрах `--lang` для команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-850">Changed to allow all casing for `--lang` parameters for commands</span></span>
* <span data-ttu-id="8b368-851">Обновлено описание модуля команды.</span><span class="sxs-lookup"><span data-stu-id="8b368-851">Updated description for command module</span></span>

### <a name="consumption"></a><span data-ttu-id="8b368-852">Потребление</span><span class="sxs-lookup"><span data-stu-id="8b368-852">Consumption</span></span>
* <span data-ttu-id="8b368-853">Добавлен отсутствующий обязательный параметр при выполнении `consumption usage list --billing-period-name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-853">Added missing required parameter when running `consumption usage list --billing-period-name`</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-854">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-854">IoT</span></span>
* <span data-ttu-id="8b368-855">Добавлена поддержка перечисления всех ключей.</span><span class="sxs-lookup"><span data-stu-id="8b368-855">Added support to list all keys</span></span>

### <a name="network"></a><span data-ttu-id="8b368-856">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-856">Network</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `network interface-endpoints` command group - use `network private-endpoints`
[BREAKING CHANGE]: Removed `network interface-endpoints` command group - use `network private-endpoints` 
* <span data-ttu-id="8b368-858">Добавлен аргумент `--nat-gateway` для `network vnet subnet [create|update]` для подключения к шлюзу NAT.</span><span class="sxs-lookup"><span data-stu-id="8b368-858">Added `--nat-gateway` argument to `network vnet subnet [create|update]` for attaching to a NAT gateway</span></span>
* <span data-ttu-id="8b368-859">Исправлена проблема с `dns zone import`, из-за которой имена записей не сопоставлялись с типом записей.</span><span class="sxs-lookup"><span data-stu-id="8b368-859">Fixed issue with `dns zone import` where record names could not match a record type</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-860">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="8b368-860">RDBMS</span></span>
* <span data-ttu-id="8b368-861">Добавлена поддержка Postgres и MySQL для георепликации.</span><span class="sxs-lookup"><span data-stu-id="8b368-861">Added postgres and mysql support for geo replication</span></span>

### <a name="rbac"></a><span data-ttu-id="8b368-862">RBAC</span><span class="sxs-lookup"><span data-stu-id="8b368-862">RBAC</span></span>
* <span data-ttu-id="8b368-863">Добавлена поддержка области группы управления для `role assignment`.</span><span class="sxs-lookup"><span data-stu-id="8b368-863">Added support for management group scope to `role assignment`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-864">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-864">Storage</span></span>
* <span data-ttu-id="8b368-865">`storage blob sync`: добавьте команду синхронизации для хранилища BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="8b368-865">`storage blob sync`: add sync command for storage blob</span></span>

### <a name="compute"></a><span data-ttu-id="8b368-866">Службы вычислений</span><span class="sxs-lookup"><span data-stu-id="8b368-866">Compute</span></span>
* <span data-ttu-id="8b368-867">Добавлен параметр `--computer-name` для `vm create` для установки имени виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="8b368-867">Added `--computer-name` to `vm create` for setting a VM's computer name</span></span>
* <span data-ttu-id="8b368-868">Переименован параметр `--ssh-key-value` в `--ssh-key-values` для `[vm|vmss] create` для приема нескольких значений пути или открытого ключа SSH.</span><span class="sxs-lookup"><span data-stu-id="8b368-868">Renamed `--ssh-key-value` renamed to `--ssh-key-values` for `[vm|vmss] create` - can now accept multiple ssh public key values or paths</span></span>
  * <span data-ttu-id="8b368-869">__Примечание.__ Это **не** критическое изменение, благодаря которому `--ssh-key-value` будет правильно анализироваться, так как соответствует только `--ssh-key-values`.</span><span class="sxs-lookup"><span data-stu-id="8b368-869">__Note__: This is **not** a breaking change - `--ssh-key-value` will be parsed correctly as it matches only `--ssh-key-values`</span></span>
* <span data-ttu-id="8b368-870">Внесено изменение в аргумент `ppg create` для `--type` — теперь он необязательный.</span><span class="sxs-lookup"><span data-stu-id="8b368-870">Changed the `--type` argument of `ppg create` to be optional</span></span>

## <a name="may-6-2019"></a><span data-ttu-id="8b368-871">6 мая 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-871">May 6, 2019</span></span>

<span data-ttu-id="8b368-872">Версия 2.0.64</span><span class="sxs-lookup"><span data-stu-id="8b368-872">Version 2.0.64</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-873">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-873">ACS</span></span>
* <span data-ttu-id="8b368-874">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--fqdn` из команд `openshift`.</span><span class="sxs-lookup"><span data-stu-id="8b368-874">[BREAKING CHANGE] Removed `--fqdn` flag on `openshift` commands</span></span>
* <span data-ttu-id="8b368-875">Внесено изменение для использования общедоступной версии API для Azure Red Hat Openshift.</span><span class="sxs-lookup"><span data-stu-id="8b368-875">Changed to use Azure Red Hat Openshift GA API Version</span></span>
* <span data-ttu-id="8b368-876">Добавлен флаг `customer-admin-group-id` в `openshift create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-876">Added `customer-admin-group-id` flag to `openshift create`</span></span>
* <span data-ttu-id="8b368-877">[Общедоступная версия.] `(PREVIEW)` больше не используется для `aks create` в параметре `--network-policy`.</span><span class="sxs-lookup"><span data-stu-id="8b368-877">[GA] Removed `(PREVIEW)` from `aks create` option `--network-policy`</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-878">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-878">Appservice</span></span>
* <span data-ttu-id="8b368-879">[УСТАРЕЛО] Команда `functionapp devops-build` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="8b368-879">[DEPRECATED] Deprecated `functionapp devops-build` command</span></span>
  * <span data-ttu-id="8b368-880">Команда переименована в `functionapp devops-pipeline`.</span><span class="sxs-lookup"><span data-stu-id="8b368-880">Renamed to `functionapp devops-pipeline`</span></span>
* <span data-ttu-id="8b368-881">Исправлен процесс получения правильного имени пользователя для Cloud Shell, приводивший к ошибке выполнения `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="8b368-881">Fixed getting the correct username for cloudshell which was causing `webapp up` to fail</span></span>
* <span data-ttu-id="8b368-882">Обновлена документация по `appservice plan --sku` в соответствии с поддерживаемыми планами службы приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-882">Updated `appservice plan --sku` documentation updated to reflect the supported appserviceplans</span></span>
* <span data-ttu-id="8b368-883">Добавлены необязательные аргументы для группы ресурсов и план для `webapp up`.</span><span class="sxs-lookup"><span data-stu-id="8b368-883">Added optional arguments for resource group and plan to `webapp up`</span></span>
* <span data-ttu-id="8b368-884">Добавлена поддержка `webapp ssh` в соответствии с переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="8b368-884">Added support to `webapp ssh` to respect `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>
* <span data-ttu-id="8b368-885">Добавлена поддержка `appserviceplan create` для ценовой категории "Бесплатный" в Linux.</span><span class="sxs-lookup"><span data-stu-id="8b368-885">Added `appserviceplan create` support for Linux Free SKU</span></span>
* <span data-ttu-id="8b368-886">Внесено изменение в `webapp up` для перевода в спящий режим на 30 с после установки параметра приложения `SCM_DO_BUILD_DURING_DEPLOYMENT=true` для обработки холодного запуска Kudu.</span><span class="sxs-lookup"><span data-stu-id="8b368-886">Changed `webapp up` to have a 30s sleep after setting `SCM_DO_BUILD_DURING_DEPLOYMENT=true` appsetting to handle kudu cold start</span></span>
* <span data-ttu-id="8b368-887">Добавлена поддержка среды выполнения `powershell` для `functionapp create` в Windows.</span><span class="sxs-lookup"><span data-stu-id="8b368-887">Added support for `powershell` runtime to `functionapp create` on Windows</span></span>
* <span data-ttu-id="8b368-888">Добавлена команда `create-remote-connection`.</span><span class="sxs-lookup"><span data-stu-id="8b368-888">Added `create-remote-connection` command</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-889">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-889">Batch</span></span>
* <span data-ttu-id="8b368-890">Исправлена ошибка в проверяющем элементе управления для параметров `--application-package-references`.</span><span class="sxs-lookup"><span data-stu-id="8b368-890">Fixed bug in validator for `--application-package-references` options</span></span>

### <a name="botservice"></a><span data-ttu-id="8b368-891">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-891">Botservice</span></span>
* <span data-ttu-id="8b368-892">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` для создания пустого бота веб-приложения по умолчанию (т. е. бот не развертывается в Службе приложений).</span><span class="sxs-lookup"><span data-stu-id="8b368-892">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to create an empty Web App Bot by default (i.e. no bot is deployed to the App Service)</span></span>
* <span data-ttu-id="8b368-893">Добавлен флаг `--echo` в `bot create` для использования старого поведения с `-v v4`.</span><span class="sxs-lookup"><span data-stu-id="8b368-893">Added `--echo` flag to `bot create` to use the old behavior with `-v v4`</span></span>
* <span data-ttu-id="8b368-894">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено значение по умолчанию `--version` на `v4`.</span><span class="sxs-lookup"><span data-stu-id="8b368-894">[BREAKING CHANGE] Changed the default value of  `--version` to `v4`</span></span>
  * <span data-ttu-id="8b368-895">__ПРИМЕЧАНИЕ.__ `bot prepare-publish` по-прежнему использует старое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-895">__NOTE:__ `bot prepare-publish` still uses the its old default</span></span>
* <span data-ttu-id="8b368-896">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `--lang` — значение `Csharp` больше не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-896">[BREAKING CHANGE] Changed `--lang` to no longer default to `Csharp`.</span></span> <span data-ttu-id="8b368-897">Если команда требует `--lang`, который не указан, команда завершит работу с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="8b368-897">If the command requires `--lang` and it is not provided, the command will now error out</span></span>
* <span data-ttu-id="8b368-898">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в аргументы `--appid` и `--password` для `bot create` — теперь они являются обязательными и их можно создать с помощью `ad app create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-898">[BREAKING CHANGE] Changed the `--appid` and `--password` args for `bot create` to be required and can now be created via `ad app create`</span></span>
* <span data-ttu-id="8b368-899">Добавлена проверка `--appid` и `--password`.</span><span class="sxs-lookup"><span data-stu-id="8b368-899">Added `--appid` and `--password` validation</span></span>
* <span data-ttu-id="8b368-900">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4`, чтобы не создавать или не использовать учетную запись хранения или Application Insights.</span><span class="sxs-lookup"><span data-stu-id="8b368-900">[BREAKING CHANGE] Changed `bot create -v v4` to not create or use a Storage Account or Application Insights</span></span>
* <span data-ttu-id="8b368-901">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v3`, чтобы требовать регион, где доступна служба Application Insights.</span><span class="sxs-lookup"><span data-stu-id="8b368-901">[BREAKING CHANGE] Changed `bot create -v v3` to require a region where Application Insights is available</span></span>
* <span data-ttu-id="8b368-902">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot update`, чтобы влиять только на определенные свойства бота.</span><span class="sxs-lookup"><span data-stu-id="8b368-902">[BREAKING CHANGE] Changed `bot update` to now affect only specific properties of a bot</span></span>
* <span data-ttu-id="8b368-903">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в флаг `--lang` для принятия `Javascript` вместо `Node`.</span><span class="sxs-lookup"><span data-stu-id="8b368-903">[BREAKING CHANGE] Changed `--lang` flags to accept `Javascript` instead of `Node`</span></span>
* <span data-ttu-id="8b368-904">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`Node` больше не используется как допустимое значение `--lang`.</span><span class="sxs-lookup"><span data-stu-id="8b368-904">[BREAKING CHANGE] Removed `Node` as an allowed `--lang` value</span></span>
* <span data-ttu-id="8b368-905">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `bot create -v v4 -k webapp` — значение `SCM_DO_BUILD_DURING_DEPLOYMENT` больше не равно true.</span><span class="sxs-lookup"><span data-stu-id="8b368-905">[BREAKING CHANGE] Changed `bot create -v v4 -k webapp` to no longer set `SCM_DO_BUILD_DURING_DEPLOYMENT` to true.</span></span> <span data-ttu-id="8b368-906">Все развертывания через Kudu будут работать в соответствии с поведением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-906">All deployments through Kudu will act according to their default behavior</span></span>
* <span data-ttu-id="8b368-907">Внесено изменение в `bot download` для ботов без файлов `.bot`, чтобы создавать файл конфигурации для определенного языка со значениями из параметров приложения для бота.</span><span class="sxs-lookup"><span data-stu-id="8b368-907">Changed `bot download` for bots without `.bot` files to create the language-specific configuration file with values from the Application Settings for the bot</span></span>
* <span data-ttu-id="8b368-908">В команду `bot prepare-deploy` добавлена поддержка параметра `Typescript`.</span><span class="sxs-lookup"><span data-stu-id="8b368-908">Added `Typescript` support to `bot prepare-deploy`</span></span>
* <span data-ttu-id="8b368-909">Добавлено предупреждающее сообщение в `bot prepare-deploy` для ботов `Javascript` и `Typescript`, когда `--code-dir` не содержит `package.json`.</span><span class="sxs-lookup"><span data-stu-id="8b368-909">Added warning message to `bot prepare-deploy` for `Javascript` and `Typescript` bots for when `--code-dir` does not contain `package.json`</span></span>
* <span data-ttu-id="8b368-910">Внесено изменение в `bot prepare-deploy` для возврата `true` при успешном выполнении.</span><span class="sxs-lookup"><span data-stu-id="8b368-910">Changed `bot prepare-deploy` to return `true` if successful</span></span>
* <span data-ttu-id="8b368-911">Включено ведение подробного журнала для `bot prepare-deploy`.</span><span class="sxs-lookup"><span data-stu-id="8b368-911">Added verbose logging to `bot prepare-deploy`</span></span>
* <span data-ttu-id="8b368-912">Добавлены более доступные регионы Application Insights для `az bot create -v v3`.</span><span class="sxs-lookup"><span data-stu-id="8b368-912">Added more available Application Insights regions to `az bot create -v v3`</span></span>

### <a name="configure"></a><span data-ttu-id="8b368-913">Configure</span><span class="sxs-lookup"><span data-stu-id="8b368-913">Configure</span></span>
* <span data-ttu-id="8b368-914">Добавлена поддержка конфигурации по умолчанию для аргумента на основе папки.</span><span class="sxs-lookup"><span data-stu-id="8b368-914">Added support for folder based argument default value configurations</span></span>

### <a name="eventhubs"></a><span data-ttu-id="8b368-915">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="8b368-915">Eventhubs</span></span>
* <span data-ttu-id="8b368-916">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="8b368-916">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="8b368-917">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-917">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-918">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-918">Network</span></span>
* <span data-ttu-id="8b368-919">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен аргумент `--cache` на `--defer` для `vnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-919">[BREAKING CHANGE] Replaced `--cache` arugment with `--defer` for `vnet [create|update]`</span></span> 

### <a name="policy-insights"></a><span data-ttu-id="8b368-920">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="8b368-920">Policy Insights</span></span>
* <span data-ttu-id="8b368-921">Добавлена поддержка `--expand PolicyEvaluationDetails` для результатов оценки политики запросов для ресурса.</span><span class="sxs-lookup"><span data-stu-id="8b368-921">Added support for `--expand PolicyEvaluationDetails` to query policy evaluation details on the resource</span></span>

### <a name="role"></a><span data-ttu-id="8b368-922">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-922">Role</span></span>
* <span data-ttu-id="8b368-923">[УСТАРЕЛО] Внесено изменение в `create-for-rbac` для скрытия аргумента --password (поддержка прекращается в мае 2019 г.).</span><span class="sxs-lookup"><span data-stu-id="8b368-923">[DEPRECATED] Changed `create-for-rbac` hide '--password' argument - support will be removed in May 2019</span></span>

### <a name="service-bus"></a><span data-ttu-id="8b368-924">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="8b368-924">Service Bus</span></span>
* <span data-ttu-id="8b368-925">Добавлены команды `namespace network-rule`.</span><span class="sxs-lookup"><span data-stu-id="8b368-925">Added `namespace network-rule` commands</span></span>
* <span data-ttu-id="8b368-926">Добавлен аргумент `--default-action` для правил сети для `namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-926">Added `--default-action` argument for network rules to `namespace [create|update]`</span></span>
* <span data-ttu-id="8b368-927">Внесено исправление в `topic [create|update]` — теперь `--max-size` поддерживает значения 10, 20, 40 и 80 ГБ для номера SKU ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="8b368-927">Fixed `topic [create|update]` to allow `--max-size` support for 10, 20, 40 and 80GB values with premium SKU</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-928">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-928">SQL</span></span>
* <span data-ttu-id="8b368-929">Добавлены команды `sql virtual-cluster [list|show|delete]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-929">Added `sql virtual-cluster [list|show|delete]` commands</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-930">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-930">VM</span></span>
* <span data-ttu-id="8b368-931">Добавлены параметры `--protect-from-scale-in` и `--protect-from-scale-set-actions` для `vmss update`, чтобы включать обновления политики защиты для экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="8b368-931">Added `--protect-from-scale-in` and `--protect-from-scale-set-actions` to `vmss update` to enable updates to the protection policy of VMSS VM instances</span></span>
* <span data-ttu-id="8b368-932">Добавлены параметры `--instance-id` для `vmss update` для включения общего обновления экземпляров виртуальных машин из Масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="8b368-932">Added `--instance-id` to `vmss update` to enable generic update of VMSS VM instances</span></span>
* <span data-ttu-id="8b368-933">Добавлен параметр `--instance-id` для команды `vmss wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-933">Added `--instance-id` to `vmss wait`</span></span>
* <span data-ttu-id="8b368-934">Добавлена новая группа команд `ppg` для управления группами размещения близкого взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="8b368-934">Added new `ppg` command group for managing Proximity Placement Groups</span></span>
* <span data-ttu-id="8b368-935">Добавлен параметр `--ppg` для `[vm|vmss] create` и `vm availability-set create` для управления PPG.</span><span class="sxs-lookup"><span data-stu-id="8b368-935">Added `--ppg` to `[vm|vmss] create` and `vm availability-set create` for managing PPGs</span></span>
* <span data-ttu-id="8b368-936">Добавлен параметр `--hyper-v-generation` для команды `image create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-936">Added `--hyper-v-generation` parameter to `image create`</span></span>

## <a name="april-23-2019"></a><span data-ttu-id="8b368-937">23 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-937">April 23, 2019</span></span>

<span data-ttu-id="8b368-938">Версия 2.0.63</span><span class="sxs-lookup"><span data-stu-id="8b368-938">Version 2.0.63</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-939">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-939">ACS</span></span>
* <span data-ttu-id="8b368-940">Внесено изменение в `aks get-credentials` для запроса на перезапись повторяющихся значений.</span><span class="sxs-lookup"><span data-stu-id="8b368-940">Changed `aks get-credentials` to prompt to overwrite duplicated values</span></span>
* <span data-ttu-id="8b368-941">Удалено описание `(PREVIEW)` из команд Dev Spaces aks use-dev-spaces и aks remove-dev-spaces.</span><span class="sxs-lookup"><span data-stu-id="8b368-941">Removed `(PREVIEW)` from Dev Spaces commands "aks use-dev-spaces" and "aks remove-dev-spaces"</span></span>

### <a name="ams"></a><span data-ttu-id="8b368-942">AMS</span><span class="sxs-lookup"><span data-stu-id="8b368-942">AMS</span></span>
* <span data-ttu-id="8b368-943">Исправлена ошибка с обновлением фильтров ресурсов и учетных записей.</span><span class="sxs-lookup"><span data-stu-id="8b368-943">Fixed bug with asset and account filters update</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-944">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-944">AppService</span></span>
* <span data-ttu-id="8b368-945">Добавлена поддержка ASE и времени ожидания для `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="8b368-945">Added support for ASE and timeout to `webapp ssh`</span></span>
* <span data-ttu-id="8b368-946">Добавлена возможность настройки непрерывной интеграции и развертывания в конвейере Azure DevOps из репозитория Github для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="8b368-946">Added support for establishing CI CD to an Azure DevOps pipeline from a Github repository to Function apps</span></span>
* <span data-ttu-id="8b368-947">Добавлен аргумент `--github-pat` для `functionapp devops-build create` для получения личного маркера доступа Github.</span><span class="sxs-lookup"><span data-stu-id="8b368-947">Added `--github-pat` argument to `functionapp devops-build create` to accept Github personal access token</span></span>
* <span data-ttu-id="8b368-948">Добавлен аргумент `--github-repository` для `functionapp devops-build create` для подключения репозитория Github, который содержит исходный код приложения-функции.</span><span class="sxs-lookup"><span data-stu-id="8b368-948">Added `--github-repository` argument to `functionapp devops-build create` to accept Github repository that contains a functionapp source code</span></span>
* <span data-ttu-id="8b368-949">Исправлена проблема со сбоем `az webapp up --logs` и обновлением .Net Core до версии 2.1 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-949">Fixed issue where `az webapp up --logs` was failing with a error and updating default .NETCORE version to 2.1</span></span>
* <span data-ttu-id="8b368-950">Удалены ненужные параметры приложения-функции при создании приложения-функции с помощью плана потребления.</span><span class="sxs-lookup"><span data-stu-id="8b368-950">Removed unnecessary functionapp settings when creating a function app with consumption plan</span></span>
* <span data-ttu-id="8b368-951">Внесены изменения в `webapp up`, чтобы строка ASP по умолчанию добавляла номера в конец для создания плана службы приложений на основе параметров SKU.</span><span class="sxs-lookup"><span data-stu-id="8b368-951">Changed `webapp up` so the default asp string now appends number at the end to create a new ASP based on SKU options</span></span>
* <span data-ttu-id="8b368-952">Добавлен параметр `-b` для `webapp up` для запуска приложения в браузере.</span><span class="sxs-lookup"><span data-stu-id="8b368-952">Added `-b` as an option to `webapp up` to launch the app in the browser</span></span>
* <span data-ttu-id="8b368-953">Внесены изменения в `webapp deployment source config zip` для обработки переменной среды `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION`.</span><span class="sxs-lookup"><span data-stu-id="8b368-953">Changed `webapp deployment source config zip` to handle `AZURE_CLI_DISABLE_CONNECTION_VERIFICATION` environment variable</span></span>

### <a name="deployment-manager"></a><span data-ttu-id="8b368-954">Диспетчер развертывания</span><span class="sxs-lookup"><span data-stu-id="8b368-954">Deployment Manager</span></span>
* <span data-ttu-id="8b368-955">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Создание и администрирование артефактов, которые поддерживают развертывания</span><span class="sxs-lookup"><span data-stu-id="8b368-955">[PREVIEW] Create and manage artifacts that support rollouts</span></span>

### <a name="lab"></a><span data-ttu-id="8b368-956">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="8b368-956">Lab</span></span>
* <span data-ttu-id="8b368-957">Исправлена ошибка, которая приводила к неожиданному завершению работы.</span><span class="sxs-lookup"><span data-stu-id="8b368-957">Fixed bug which would cause an early exit</span></span>

### <a name="network"></a><span data-ttu-id="8b368-958">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-958">Network</span></span>
* <span data-ttu-id="8b368-959">Добавлено автоматическое делегирование сервера имен для `dns zone create` в родительском объекте во время создания дочерней зоны.</span><span class="sxs-lookup"><span data-stu-id="8b368-959">Added auto name server delegation to `dns zone create` in parent during child zone creation</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-960">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-960">Resource</span></span>
* <span data-ttu-id="8b368-961">[УСТАРЕЛО] Не рекомендуются к использованию аргументы `--link-id`, `--target-id` и `--filter-string` для `resource link`.</span><span class="sxs-lookup"><span data-stu-id="8b368-961">[DEPRECATED] Deprecated `--link-id`, `--target-id` and `--filter-string` arguments of `resource link`</span></span>
  * <span data-ttu-id="8b368-962">Используйте вместо них аргументы `--link`, `--target` и `--filter`.</span><span class="sxs-lookup"><span data-stu-id="8b368-962">Use the arguments `--link`, `--target`, and `--filter` instead</span></span>
* <span data-ttu-id="8b368-963">Исправлена проблема, из-за которой команды `resource link [create|update]` не работали.</span><span class="sxs-lookup"><span data-stu-id="8b368-963">Fixed issue where `resource link [create|update]` commands would not work</span></span>
* <span data-ttu-id="8b368-964">Исправлена проблема, из-за которой удаление с помощью идентификатора ресурса приводило к сбою или ошибке.</span><span class="sxs-lookup"><span data-stu-id="8b368-964">Fixed an issue where deleting using a resource ID could crash on error</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-965">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-965">SQL</span></span>
* <span data-ttu-id="8b368-966">Добавлена поддержка пользовательского часового пояса в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="8b368-966">Added support for custom time zone on managed instances</span></span>
* <span data-ttu-id="8b368-967">Внесено изменение, чтобы разрешить использовать имя эластичного пула с `sql db update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-967">Changed to allow elastic pool name to be used with `sql db update`</span></span>
* <span data-ttu-id="8b368-968">В команду `sql server [create|update]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-968">Added `--no-wait` support to `sql server [create|update]`</span></span>
* <span data-ttu-id="8b368-969">Добавлена команда `sql server wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-969">Added command `sql server wait`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-970">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-970">Storage</span></span>
* <span data-ttu-id="8b368-971">Устранена проблема с двойной кодировкой маркеров SAS в `storage blob generate-sas`.</span><span class="sxs-lookup"><span data-stu-id="8b368-971">Fixed issue with double-encoded SAS tokens in `storage blob generate-sas`</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-972">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-972">VM</span></span>
* <span data-ttu-id="8b368-973">Добавлен флаг `--skip-shutdown` для `vm|vmss stop` для выключения виртуальных машин без завершения работы.</span><span class="sxs-lookup"><span data-stu-id="8b368-973">Added `--skip-shutdown` flag to `vm|vmss stop` to power-off VMs without shutdown</span></span>
* <span data-ttu-id="8b368-974">Добавлен аргумент `--storage-account-type` для `sig image-version create` настройки типа учетной записи профиля публикации.</span><span class="sxs-lookup"><span data-stu-id="8b368-974">Added `--storage-account-type` argument to `sig image-version create` to set the publishing profile's account type</span></span>
* <span data-ttu-id="8b368-975">Добавлен аргумент `--target-regions` для `sig image-version create` для указания типов учетных записей хранения, связанных с регионами.</span><span class="sxs-lookup"><span data-stu-id="8b368-975">Added `--target-regions` argument to `sig image-version create` to allow setting region-specific storage account types</span></span>

## <a name="april-9-2019"></a><span data-ttu-id="8b368-976">9 апреля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-976">April 9, 2019</span></span>

### <a name="core"></a><span data-ttu-id="8b368-977">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-977">Core</span></span>
* <span data-ttu-id="8b368-978">Исправлена проблема, из-за которой для некоторых расширений отображалась версия `Unknown` и ее невозможно было обновить.</span><span class="sxs-lookup"><span data-stu-id="8b368-978">Fixed issue where some extensions showed a version of `Unknown` and could not be updated</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-979">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-979">ACR</span></span>
* <span data-ttu-id="8b368-980">Добавлена поддержка запуска образа без контекста.</span><span class="sxs-lookup"><span data-stu-id="8b368-980">Added support running an image contextlessly</span></span>

### <a name="ams"></a><span data-ttu-id="8b368-981">AMS</span><span class="sxs-lookup"><span data-stu-id="8b368-981">AMS</span></span>
* [УСТАРЕЛО]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
[DEPRECATED]: Deprecated the `--bitrate` parameter of `account-filter` and `asset-filter`
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Renamed the `--bitrate` parameter to `--first-quality`
[BREAKING CHANGE]: Renamed the `--bitrate` parameter to `--first-quality`
* <span data-ttu-id="8b368-984">Добавлена поддержка новых параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-984">Added new encryption parameters support in `ams streaming-policy create`</span></span>
* <span data-ttu-id="8b368-985">Добавлен новый параметр `--filters` для `ams streaming-locator create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-985">Added new paramter `--filters` to `ams streaming-locator create`</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-986">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-986">AppService</span></span>
* <span data-ttu-id="8b368-987">В команду `webapp up` добавлена поддержка параметра `--logs`.</span><span class="sxs-lookup"><span data-stu-id="8b368-987">Added `--logs` support to `webapp up`</span></span>
* <span data-ttu-id="8b368-988">Исправлены ошибки в команде `functionapp devops-build create` при создании файла `azure-pipelines.yml`.</span><span class="sxs-lookup"><span data-stu-id="8b368-988">Fixed `functionapp devops-build create` command `azure-pipelines.yml` generation issues</span></span>
* <span data-ttu-id="8b368-989">Улучшена обработка и индикаторы ошибок с `unctionapp devops-build create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-989">Improved `unctionapp devops-build create` error handling and indicators</span></span>
* <span data-ttu-id="8b368-990">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален флаг `--local-git` для команды `devops-build`. Обнаружение и обработка локального репозитория Git являются обязательными для создания конвейеров DevOps в Azure.</span><span class="sxs-lookup"><span data-stu-id="8b368-990">[BREAKING CHANGE] Removed the `--local-git` flag for `devops-build` command, local git detection and handling are compulsory for creating Azure DevOps pipelines</span></span>
* <span data-ttu-id="8b368-991">Добавлена поддержка создания плана функций Linux.</span><span class="sxs-lookup"><span data-stu-id="8b368-991">Added support for Linux functions plan creation</span></span>
* <span data-ttu-id="8b368-992">Добавлена возможность менять план для приложения-функции с помощью `functionapp update --plan`.</span><span class="sxs-lookup"><span data-stu-id="8b368-992">Added ability to switch a plan underneath a function app using `functionapp update --plan`</span></span>
* <span data-ttu-id="8b368-993">Добавлена поддержка параметров масштабирования плана "Премиум" для Функций Azure.</span><span class="sxs-lookup"><span data-stu-id="8b368-993">Added support for Azure Functions premium plan scale out settings</span></span>

### <a name="cdn"></a><span data-ttu-id="8b368-994">CDN</span><span class="sxs-lookup"><span data-stu-id="8b368-994">CDN</span></span>
* <span data-ttu-id="8b368-995">Добавлена поддержка `Microsoft_Standard` и `Standard_ChinaCdn`.</span><span class="sxs-lookup"><span data-stu-id="8b368-995">Added support for `Microsoft_Standard` and `Standard_ChinaCdn`</span></span>

### <a name="feedback"></a><span data-ttu-id="8b368-996">Отзывы</span><span class="sxs-lookup"><span data-stu-id="8b368-996">Feedback</span></span>
* <span data-ttu-id="8b368-997">Внесены изменения в `feedback` для отображения метаданных недавно выполненных команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-997">Changed `feedback` to show metadata on recently run commands</span></span>
* <span data-ttu-id="8b368-998">Внесены изменения в `feedback`. Теперь при регистрации проблемы отображается запрос, в соответствии с которым пользователь должен открыть браузер и воспользоваться шаблоном проблемы.</span><span class="sxs-lookup"><span data-stu-id="8b368-998">Changed `feedback` to prompt user to assist in issue creation process by opening a brower and using an issue template</span></span>
* <span data-ttu-id="8b368-999">Внесены изменения в `feedback`. Теперь текст проблемы выводится при запуске с параметром --verbose.</span><span class="sxs-lookup"><span data-stu-id="8b368-999">Changed `feedback` to print out issue body when run with '--verbose'</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-1000">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-1000">Monitor</span></span>
* <span data-ttu-id="8b368-1001">Исправлена проблема, из-за которой у параметра count было недопустимое значение в `metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1001">Fixed issue where "count" was not a permitted value with `metrics alert [create|update]`</span></span> 

### <a name="network"></a><span data-ttu-id="8b368-1002">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1002">Network</span></span>
* <span data-ttu-id="8b368-1003">Исправлен формат таблицы, которая не отображалась с помощью `vnet-gateway list-bgp-peer-status`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1003">Fixed table format not displaying with `vnet-gateway list-bgp-peer-status`</span></span>
* <span data-ttu-id="8b368-1004">Добавлены команды `list-request-headers` и `list-response-headers` для `application-gateway rewrite-rule`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1004">Added `list-request-headers` and `list-response-headers` commands to `application-gateway rewrite-rule`</span></span>
* <span data-ttu-id="8b368-1005">Добавлена команда `list-server-variables` для `application-gateway rewrite-rule condition`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1005">Added `list-server-variables` command to `application-gateway rewrite-rule condition`</span></span>
* <span data-ttu-id="8b368-1006">Исправлена проблема, из-за которой обновление состояния соединения на порту ExpressRoute вызывало неизвестное исключение атрибута `express-route port update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1006">Fixed an issue where updating link state on an express-route port would throw an unknown attribute exception `express-route port update`</span></span>

### <a name="privatedns"></a><span data-ttu-id="8b368-1007">Частная зона DNS</span><span class="sxs-lookup"><span data-stu-id="8b368-1007">PrivateDNS</span></span>
* <span data-ttu-id="8b368-1008">Добавлена команда `network private-dns` для частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="8b368-1008">Added `network private-dns` for Private DNS zones</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-1009">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-1009">Resource</span></span>
* <span data-ttu-id="8b368-1010">Исправлена проблема с `deployment create` и `group deployment create`, из-за которой файл параметров с пустым набором параметров не работал.</span><span class="sxs-lookup"><span data-stu-id="8b368-1010">Fixed issue with `deployment create` and `group deployment create` where a parameters file with an empty set of parameters would not work</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1011">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1011">Role</span></span>
* <span data-ttu-id="8b368-1012">Внесены исправления в `create-for-rbac`. Теперь `--years` обрабатывается правильно.</span><span class="sxs-lookup"><span data-stu-id="8b368-1012">Fixed `create-for-rbac` to handle `--years` correctly</span></span>
* <span data-ttu-id="8b368-1013">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `role assignment delete`. Теперь появляется запрос при удалении всех назначений в рамках подписки без дополнительных условий.</span><span class="sxs-lookup"><span data-stu-id="8b368-1013">[BREAKING CHANGE] Changed `role assignment delete` to prompt when deleting all assignments under the subscription unconditionally</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-1014">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-1014">SQL</span></span>
* <span data-ttu-id="8b368-1015">Команда `sql mi [create|update]` обновлена с помощью свойств proxyOverride и publicDataEndpointEnabled.</span><span class="sxs-lookup"><span data-stu-id="8b368-1015">Updated `sql mi [create|update]` with the properties proxyOverride and publicDataEndpointEnabled</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1016">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1016">Storage</span></span>
* <span data-ttu-id="8b368-1017">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален результат выполнения `storage blob delete`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1017">[BREAKING CHANGE] Removed result of `storage blob delete`</span></span>
* <span data-ttu-id="8b368-1018">В команду `storage blob generate-sas` добавлен параметр `--full-uri` для создания полного URI большого двоичного объекта с помощью SAS.</span><span class="sxs-lookup"><span data-stu-id="8b368-1018">Added `--full-uri` to `storage blob generate-sas` to create the full uri for the blob with sas</span></span>
* <span data-ttu-id="8b368-1019">В команду `storage file copy start` добавлен параметр `--file-snapshot` для копирования файла из моментального снимка.</span><span class="sxs-lookup"><span data-stu-id="8b368-1019">Added `--file-snapshot` to `storage file copy start` to copy file from snapshot</span></span>
* <span data-ttu-id="8b368-1020">Внесены изменения в `storage blob copy cancel`. Теперь вместо исключения для NoPendingCopyOperation отображается только сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="8b368-1020">Changed `storage blob copy cancel` to only show the error instead of exception for NoPendingCopyOperation</span></span>

## <a name="march-26-2019"></a><span data-ttu-id="8b368-1021">26 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1021">March 26, 2019</span></span>


### <a name="core"></a><span data-ttu-id="8b368-1022">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1022">Core</span></span>
* <span data-ttu-id="8b368-1023">Устранены проблемы с несовместимостью расширений для разработки.</span><span class="sxs-lookup"><span data-stu-id="8b368-1023">Fixed issues with dev extension incompatibility</span></span>
* <span data-ttu-id="8b368-1024">Функция обработки ошибок теперь указывает клиентам на страницу проблем.</span><span class="sxs-lookup"><span data-stu-id="8b368-1024">Error handling now points customers to issues page</span></span>

### <a name="cloud"></a><span data-ttu-id="8b368-1025">Cloud</span><span class="sxs-lookup"><span data-stu-id="8b368-1025">Cloud</span></span>
* <span data-ttu-id="8b368-1026">Исправлена ошибка с сообщением о не найденной подписке в `cloud set`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1026">Fixed a 'subscription not found' error in `cloud set`</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1027">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1027">ACR</span></span>
* <span data-ttu-id="8b368-1028">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="8b368-1028">Fixed redundant sources in image import</span></span>
* <span data-ttu-id="8b368-1029">Добавлено `--auth-mode` в команды `acr build`, `acr run`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1029">Added `--auth-mode` to `acr build`, `acr run`, `acr task create`, and `acr task update` commands</span></span>
* <span data-ttu-id="8b368-1030">Добавлена команда acr task credential для управления учетными данными для задачи.</span><span class="sxs-lookup"><span data-stu-id="8b368-1030">Added 'acr task credential' command group for managing credentials for a Task</span></span>
* <span data-ttu-id="8b368-1031">Добавлено --no-wait в команду `acr build`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1031">Added '--no-wait' to `acr build` command</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1032">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-1032">AppService</span></span>
* <span data-ttu-id="8b368-1033">Исправлена ошибка с `webapp up`, из-за которой нельзя было правильно выполнить запуск из пустого каталога или скрипта неизвестного кода.</span><span class="sxs-lookup"><span data-stu-id="8b368-1033">Fixed bug where `webapp up` was not handling running from empty directory or unknown code scenario correctly</span></span>
* <span data-ttu-id="8b368-1034">Исправлена ошибка, из-за которой не работали слоты для `[webapp|functionapp] config ssl bind`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1034">Fixed bug where slots didn't work for `[webapp|functionapp] config ssl bind`</span></span>

### <a name="bot-service"></a><span data-ttu-id="8b368-1035">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-1035">BOT Service</span></span>
* <span data-ttu-id="8b368-1036">Добавлено `bot prepare-deploy` для подготовки к развертыванию ботов с помощью `webapp`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1036">Added `bot prepare-deploy` to prepare for deploying bots via `webapp`</span></span>
* <span data-ttu-id="8b368-1037">Изменено `bot create --kind registration` для отображения пароля, если пароль не указан.</span><span class="sxs-lookup"><span data-stu-id="8b368-1037">Changed `bot create --kind registration` to show password if the password is not provided</span></span>
* <span data-ttu-id="8b368-1038">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--endpoint` в `bot create --kind registration` на пустую строку (по умолчанию) вместо запрашиваемой.</span><span class="sxs-lookup"><span data-stu-id="8b368-1038">[BREAKING CHANGE] Changed `--endpoint` in `bot create --kind registration` to default to an empty string instead of being required</span></span>
* <span data-ttu-id="8b368-1039">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="8b368-1039">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>

### <a name="cdn"></a><span data-ttu-id="8b368-1040">CDN</span><span class="sxs-lookup"><span data-stu-id="8b368-1040">CDN</span></span>
* <span data-ttu-id="8b368-1041">Добавлена поддержка параметра `--no-wait` в команде `cdn endpoint [create|update|start|stop|delete|load|purge]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1041">Added support for `--no-wait` to `cdn endpoint [create|update|start|stop|delete|load|purge]`</span></span>  
* <span data-ttu-id="8b368-1042">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено поведение кэширования строки запроса `cdn endpoint create` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1042">[BREAKING CHANGE]: Changed `cdn endpoint create` default query string caching behaviour.</span></span> <span data-ttu-id="8b368-1043">IgnoreQueryString больше не используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1043">No longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="8b368-1044">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="8b368-1044">It is now set by the service</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8b368-1045">Сosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-1045">Cosmosdb</span></span>
* <span data-ttu-id="8b368-1046">Добавлена поддержка `--enable-multiple-write-locations` для обновления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="8b368-1046">Added support for `--enable-multiple-write-locations` on account update</span></span>
* <span data-ttu-id="8b368-1047">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="8b368-1047">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-1048">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-1048">Interactive</span></span>
* <span data-ttu-id="8b368-1049">Исправлена несовместимость с интерактивным расширением, установленным с помощью azdev.</span><span class="sxs-lookup"><span data-stu-id="8b368-1049">Fixed incompatibility with Interactive extension installed through azdev</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-1050">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-1050">Monitor</span></span>
* <span data-ttu-id="8b368-1051">Внесено изменение, разрешающее использовать значение измерения `*` для `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1051">Changed to allow dimension value `*` for `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1052">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1052">Network</span></span>
* <span data-ttu-id="8b368-1053">Добавлена группа команд `rewrite-rule` для `application-gateway`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1053">Added `rewrite-rule` command group to `application-gateway`</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-1054">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-1054">Profile</span></span>
* <span data-ttu-id="8b368-1055">Включена поддержка учетной записи уровня клиентов для управляемого удостоверения службы для `login`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1055">Added tenant level account support for managed service identity to `login`</span></span>

### <a name="postgres"></a><span data-ttu-id="8b368-1056">Postgres</span><span class="sxs-lookup"><span data-stu-id="8b368-1056">Postgres</span></span> 
* <span data-ttu-id="8b368-1057">Добавлены команды postgresql `replica` и команда `restart server`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1057">Added postgresql `replica` commands and `restart server` command</span></span>
* <span data-ttu-id="8b368-1058">Внесены изменения для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1058">Changed to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-1059">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-1059">Resource</span></span>
* <span data-ttu-id="8b368-1060">Улучшены табличные выходные данные для `deployment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1060">Improved table output for `deployment [create|list|show]`</span></span>
* <span data-ttu-id="8b368-1061">Исправлена проблема с `deployment [create|validate]`, из-за которой secureObject типа не распознавался.</span><span class="sxs-lookup"><span data-stu-id="8b368-1061">Fixed issue with `deployment [create|validate]` where type secureObject was not recognized</span></span>

### <a name="graph"></a><span data-ttu-id="8b368-1062">График</span><span class="sxs-lookup"><span data-stu-id="8b368-1062">Graph</span></span>
* <span data-ttu-id="8b368-1063">Добавлена поддержка параметра `--end-date` в команде `ad [app|sp] credential reset`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1063">Added support for `--end-date` to `ad [app|sp] credential reset`</span></span>
* <span data-ttu-id="8b368-1064">Добавлена поддержка разрешений для `ad app permission add`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1064">Added support to add permissions with `ad app permission add`</span></span>
* <span data-ttu-id="8b368-1065">Исправлена проблема с `ad app permission list`, из-за которой отсутствовали разрешения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1065">Fixed a bug with `ad app permission list` when there were no permissions</span></span>
* <span data-ttu-id="8b368-1066">Изменено `ad sp delete` для пропуска удаления назначения роли, если текущая учетная запись не содержит подписок.</span><span class="sxs-lookup"><span data-stu-id="8b368-1066">Changed `ad sp delete` to skip role assignment delete if the current account has no subscription</span></span>
* <span data-ttu-id="8b368-1067">Изменено `ad app create` для использования `--identifier-uris` пустого списка (по умолчанию), если список не указан.</span><span class="sxs-lookup"><span data-stu-id="8b368-1067">Changed `ad app create` to have `--identifier-uris` default to empty list if not provided</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1068">носителей.</span><span class="sxs-lookup"><span data-stu-id="8b368-1068">storage</span></span>
* <span data-ttu-id="8b368-1069">Добавлено `--snapshot` для `storage file download-batch` для скачивания из моментального снимка общего ресурса.</span><span class="sxs-lookup"><span data-stu-id="8b368-1069">Added `--snapshot` to `storage file download-batch` to download from a share snapshot</span></span>
* <span data-ttu-id="8b368-1070">Изменен индикатор выполнения `storage blob [download-batch|upload-batch]`, чтобы обобщить сведения и указать текущий большой двоичный объект.</span><span class="sxs-lookup"><span data-stu-id="8b368-1070">Changed `storage blob [download-batch|upload-batch]` progress bar to be less verbose and indicate current blob</span></span>
* <span data-ttu-id="8b368-1071">Исправлена проблема с `storage account update` при обновлении параметров шифрования.</span><span class="sxs-lookup"><span data-stu-id="8b368-1071">Fixed issue with `storage account update` when updating encryption parameters</span></span>
* <span data-ttu-id="8b368-1072">Исправлена проблема со сбоем `storage blob show` при использовании OAuth (`--auth-mode=login`).</span><span class="sxs-lookup"><span data-stu-id="8b368-1072">Fixed issue where `storage blob show` would fail when using oauth (`--auth-mode=login`)</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1073">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1073">VM</span></span>
* <span data-ttu-id="8b368-1074">Добавлена команда `image update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1074">Added `image update` command</span></span>

## <a name="march-12-2019"></a><span data-ttu-id="8b368-1075">12 марта 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1075">March 12, 2019</span></span>

<span data-ttu-id="8b368-1076">Версия 2.0.60</span><span class="sxs-lookup"><span data-stu-id="8b368-1076">Version 2.0.60</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1077">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1077">Core</span></span>

* <span data-ttu-id="8b368-1078">Исправлена недопустимая ошибка в `cloud set` о том, что подписка не найдена.</span><span class="sxs-lookup"><span data-stu-id="8b368-1078">Fixed an incorrect error in `cloud set` about subscription not found</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1079">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1079">ACR</span></span>

* <span data-ttu-id="8b368-1080">Исправлена ошибка с избыточными источниками при импорте изображений.</span><span class="sxs-lookup"><span data-stu-id="8b368-1080">Fixed redundant sources in image import</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1081">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1081">ACS</span></span>

* <span data-ttu-id="8b368-1082">Внесены изменения, в соответствии с которыми параметр `--listen-address` для `aks browse` игнорируется, если он не поддерживается kubectl.</span><span class="sxs-lookup"><span data-stu-id="8b368-1082">Changed to ignore the `--listen-address` parameter for `aks browse` if it is not supported by kubectl</span></span> 

### <a name="appservice"></a><span data-ttu-id="8b368-1083">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-1083">AppService</span></span>

* <span data-ttu-id="8b368-1084">Добавлено `[webapp|functionapp] deployment list-publishing-credentials` для получения URL-адреса публикации Kudu и связанных учетных данных.</span><span class="sxs-lookup"><span data-stu-id="8b368-1084">Added `[webapp|functionapp] deployment list-publishing-credentials` to get the Kudu publishing url and its credentials</span></span>
* <span data-ttu-id="8b368-1085">Удалена ошибочная инструкция печати для `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1085">Removed erroneous print statement for `webapp auth update`</span></span>
* <span data-ttu-id="8b368-1086">Исправлено `functionapp` для настройки правильного образа для среды выполнения в планах службы приложений Linux.</span><span class="sxs-lookup"><span data-stu-id="8b368-1086">Fixed `functionapp` to set the correct image for runtime in Linux App Service plans</span></span>
* <span data-ttu-id="8b368-1087">Удален тег предварительной версии для `webapp up` и добавлены усовершенствования в команду.</span><span class="sxs-lookup"><span data-stu-id="8b368-1087">Removed preview tag for `webapp up` and added improvements to the command</span></span>

### <a name="botservice"></a><span data-ttu-id="8b368-1088">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-1088">Botservice</span></span>

* <span data-ttu-id="8b368-1089">Добавлено `SCM_DO_BUILD_DURING_DEPLOYMENT` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="8b368-1089">Added `SCM_DO_BUILD_DURING_DEPLOYMENT` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="8b368-1090">Добавлено `Microsoft-BotFramework-AppId` и `Microsoft-BotFramework-AppPassword` для параметров приложения шаблона ARM для ботов веб-приложений версии 4.</span><span class="sxs-lookup"><span data-stu-id="8b368-1090">Added `Microsoft-BotFramework-AppId` and `Microsoft-BotFramework-AppPassword` to ARM template's Application Settings for v4 Web App Bots</span></span>
* <span data-ttu-id="8b368-1091">Удалены одинарные кавычки из выходных данных команды `bot publish` в конце `bot create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1091">Removed single quotes from `bot publish` command output at end of `bot create`</span></span>
* <span data-ttu-id="8b368-1092">Изменено `bot publish` для включения поддержки асинхронных операций.</span><span class="sxs-lookup"><span data-stu-id="8b368-1092">Changed `bot publish` to be asynchronous</span></span>

### <a name="container"></a><span data-ttu-id="8b368-1093">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-1093">Container</span></span>

* <span data-ttu-id="8b368-1094">Добавлен аргумент `--no-wait` для команды `container [start|restart]`</span><span class="sxs-lookup"><span data-stu-id="8b368-1094">Added `--no-wait` argument to `container [start|restart]`</span></span>

### <a name="eventhub"></a><span data-ttu-id="8b368-1095">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="8b368-1095">EventHub</span></span>

* <span data-ttu-id="8b368-1096">Добавлен флаг `--skip-empty-archives` для `eventhub create|update` для включения поддержки пустых архивов при записи.</span><span class="sxs-lookup"><span data-stu-id="8b368-1096">Added `--skip-empty-archives` flag to `eventhub create|update` to support empty archives in capture</span></span>

### <a name="find"></a><span data-ttu-id="8b368-1097">Поиск</span><span class="sxs-lookup"><span data-stu-id="8b368-1097">Find</span></span>

* <span data-ttu-id="8b368-1098">Основные обновления функций</span><span class="sxs-lookup"><span data-stu-id="8b368-1098">Major functionality update</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8b368-1099">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b368-1099">HDInsight</span></span>

* <span data-ttu-id="8b368-1100">Добавлен параметр `--storage-account-managed-identity` для `hdinsight create` для включения поддержки MSI ADLS 2-го поколения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1100">Added the `--storage-account-managed-identity` parameter to `hdinsight create` to support ADLS Gen2 MSI</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1101">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1101">Network</span></span>

* <span data-ttu-id="8b368-1102">Исправлена проблема с `vpn-connection update`, когда обновление VPN-подключения между шлюзами в разных подписках завершается ошибкой.</span><span class="sxs-lookup"><span data-stu-id="8b368-1102">Fixed issue with `vpn-connection update` where updating a VPN connection between gateways in different subscriptions would fail</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-1103">Rdbms</span><span class="sxs-lookup"><span data-stu-id="8b368-1103">Rdbms</span></span>

* <span data-ttu-id="8b368-1104">Незначительные исправления для получения расположения по умолчанию из группы ресурсов, когда оно не предоставляется при создании серверов, и добавления проверки числа дней хранения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1104">Minor fixes to get default location from resource group when not provided for creating servers and add validation for retention days</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1105">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1105">Role</span></span>

* <span data-ttu-id="8b368-1106">Исправлено `role definition update` для использования идентификатора для правильного разрешения определения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1106">Fixed `role definition update` to use ID to resolve definition correctly</span></span>
* <span data-ttu-id="8b368-1107">Изменено `ad app credential reset` для исключения предположения о том, что субъект-служба приложения всегда существует.</span><span class="sxs-lookup"><span data-stu-id="8b368-1107">Changed `ad app credential reset` to remove the assumption that app's service principal always exists</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8b368-1108">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8b368-1108">Service Fabric</span></span>

* <span data-ttu-id="8b368-1109">Исправлена проблема с `sf cluster list` и невозможностью итерации.</span><span class="sxs-lookup"><span data-stu-id="8b368-1109">Fixed issue with `sf cluster list` was not iterable</span></span>

## <a name="february-26-2019"></a><span data-ttu-id="8b368-1110">26 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1110">February 26, 2019</span></span>

<span data-ttu-id="8b368-1111">Версия 2.0.59</span><span class="sxs-lookup"><span data-stu-id="8b368-1111">Version 2.0.59</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1112">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1112">Core</span></span>

* <span data-ttu-id="8b368-1113">Исправлена проблема, из-за которой в некоторых экземплярах с использованием `--subscription NAME` выдавалось исключение.</span><span class="sxs-lookup"><span data-stu-id="8b368-1113">Fixed issue where in some instances using `--subscription NAME` would throw an exception</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1114">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1114">ACR</span></span>

* <span data-ttu-id="8b368-1115">Добавлен параметр `--target` для команд `acr build`, `acr task create` и `acr task update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1115">Added `--target` parameter for `acr build`, `acr task create` and `acr task update` commands</span></span>
* <span data-ttu-id="8b368-1116">Улучшена обработка ошибок для команд среды выполнения без входа в Azure.</span><span class="sxs-lookup"><span data-stu-id="8b368-1116">Improved error handling for runtime commands when not logged into Azure</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1117">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1117">ACS</span></span>

* <span data-ttu-id="8b368-1118">Добавлен параметр `--listen-address` для команды `aks port-forward`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1118">Added `--listen-address` option to `aks port-forward`</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1119">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-1119">AppService</span></span>

* <span data-ttu-id="8b368-1120">Добавлена команда `functionapp devops-build`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1120">Added `functionapp devops-build` command</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-1121">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-1121">Batch</span></span>
* <span data-ttu-id="8b368-1122">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `batch pool upgrade os`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1122">[BREAKING CHANGE] Removed the `batch pool upgrade os` command</span></span>
* <span data-ttu-id="8b368-1123">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено свойство `Pacakges` из ответов `Application`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1123">[BREAKING CHANGE] Removed the `Pacakges` property from `Application` responses</span></span>
* <span data-ttu-id="8b368-1124">Добавлена команда `batch application package list` для вывода списка пакетов приложения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1124">Added the `batch application package list` command to list packages of an application</span></span>
* <span data-ttu-id="8b368-1125">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено `--application-id` на `--application-name` во всех командах `batch application`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1125">[BREAKING CHANGE] Changed `--application-id` to `--application-name` in all `batch application` commands,</span></span> 
* <span data-ttu-id="8b368-1126">Добавлен аргумент `--json-file` к командам для запрашивания необработанного ответа API.</span><span class="sxs-lookup"><span data-stu-id="8b368-1126">Added the `--json-file` argument to commands for requesting the raw API response</span></span>
* <span data-ttu-id="8b368-1127">Обновлена проверка для автоматического включения `https://` во все конечные точки, если они отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8b368-1127">Updated validation to automatically include `https://` in all endpoints if missing</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8b368-1128">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-1128">CosmosDB</span></span>

* <span data-ttu-id="8b368-1129">Добавлена подгруппа `network-rule` с командами `add`, `remove` и `list` для управления правилами виртуальной сети учетной записи Cosmos DB.</span><span class="sxs-lookup"><span data-stu-id="8b368-1129">Added `network-rule` subgroup with commands `add`, `remove`, and `list` for managing VNET rules of a Cosmos DB account</span></span>

### <a name="kusto"></a><span data-ttu-id="8b368-1130">Kusto</span><span class="sxs-lookup"><span data-stu-id="8b368-1130">Kusto</span></span>

* <span data-ttu-id="8b368-1131">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для типов `hot_cache_period` и `soft_delete_period` для базы данных изменен формат длительности ISO8601.</span><span class="sxs-lookup"><span data-stu-id="8b368-1131">[BREAKING CHANGE] Changed `hot_cache_period` and `soft_delete_period` types for database to ISO8601 duration format</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1132">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1132">Network</span></span>

* <span data-ttu-id="8b368-1133">Добавлен аргумент `--express-route-gateway-bypass` для команды `vpn-connection [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8b368-1133">Added `--express-route-gateway-bypass` argument to `vpn-connection [create|update]`</span></span>
* <span data-ttu-id="8b368-1134">Добавлены группы команд из расширения `express-route`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1134">Added command groups from `express-route` extensions</span></span>
* <span data-ttu-id="8b368-1135">Добавлены группы команд `express-route gateway` и `express-route port`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1135">Added `express-route gateway` and `express-route port` command groups</span></span>
* <span data-ttu-id="8b368-1136">Добавлен аргумент `--legacy-mode` в команду `express-route peering [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1136">Added argument `--legacy-mode` to `express-route peering [create|update]`</span></span> 
* <span data-ttu-id="8b368-1137">Добавлены аргументы `--allow-classic-operations` и `--express-route-port` для `express-route [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1137">Added arguments `--allow-classic-operations` and `--express-route-port` to `express-route [create|update]`</span></span>
* <span data-ttu-id="8b368-1138">Добавлен аргумент `--gateway-default-site` для команды `vnet-gateway [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8b368-1138">Added `--gateway-default-site` argument to `vnet-gateway [create|update]`</span></span>
* <span data-ttu-id="8b368-1139">Добавлены команды `ipsec-policy` для `vnet-gateway`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1139">Added `ipsec-policy` commands to `vnet-gateway`</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-1140">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-1140">Resource</span></span>

* <span data-ttu-id="8b368-1141">Исправлена проблема с `deployment create`, из-за которой в поле типа учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="8b368-1141">Fixed issue with `deployment create` where type field was case-sensitive</span></span>
* <span data-ttu-id="8b368-1142">Добавлена поддержка файла параметров на основе URI для `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1142">Added support for URI-based parameters file to `policy assignment create`</span></span>
* <span data-ttu-id="8b368-1143">Добавлена поддержка определений и параметров на основе URI для `policy set-definition update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1143">Added support for URI-based parameters and definitions to `policy set-definition update`</span></span>
* <span data-ttu-id="8b368-1144">Исправлена обработка параметров и правил для `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1144">Fixed handling of parameters and rules for `policy definition update`</span></span>
* <span data-ttu-id="8b368-1145">Исправлена проблема с `resource show/update/delete/tag/invoke-action`, из-за которой идентификаторы разных подписок не обрабатывали правильно идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="8b368-1145">Fixed issue with `resource show/update/delete/tag/invoke-action` where cross-subscription IDs did not properly honor the subscription ID</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1146">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1146">Role</span></span>

* <span data-ttu-id="8b368-1147">Добавлена поддержка ролей приложений для `ad app [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1147">Added support for app roles to `ad app [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1148">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1148">VM</span></span>

* <span data-ttu-id="8b368-1149">Исправлена проблема с отсутствием возможности включения `vm create where `--accelerated-networking\` по умолчанию для Ubuntu 18.0.</span><span class="sxs-lookup"><span data-stu-id="8b368-1149">Fixed issue with `vm create where `--accelerated-networking\` was not enabled by default for Ubuntu 18.0</span></span>

## <a name="february-12-2019"></a><span data-ttu-id="8b368-1150">12 февраля 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1150">February 12, 2019</span></span>

<span data-ttu-id="8b368-1151">Версия 2.0.58</span><span class="sxs-lookup"><span data-stu-id="8b368-1151">Version 2.0.58</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1152">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1152">Core</span></span>

* <span data-ttu-id="8b368-1153">`az --version` теперь отображает уведомление при наличии пакетов, которые можно обновить.</span><span class="sxs-lookup"><span data-stu-id="8b368-1153">`az --version` now displays a notification if you have packages that can be updated</span></span>
* <span data-ttu-id="8b368-1154">Исправлена регрессия, при которой `--ids` нельзя было больше использовать с выходными данными JSON.</span><span class="sxs-lookup"><span data-stu-id="8b368-1154">Fixed regression where `--ids` could no longer be used with JSON output</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1155">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1155">ACR</span></span>
* <span data-ttu-id="8b368-1156">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена группа команд `acr build-task`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1156">[BREAKING CHANGE] Removed `acr build-task` command group</span></span>
* <span data-ttu-id="8b368-1157">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `acr repository delete` удалены параметры `--tag` и `--manifest`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1157">[BREAKING CHANGE] Removed `--tag` and `--manifest` options from from `acr repository delete`</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1158">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1158">ACS</span></span>
* <span data-ttu-id="8b368-1159">`aks [enable-addons|disable-addons]` теперь поддерживает имена без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="8b368-1159">Added support for case-insensitive names to `aks [enable-addons|disable-addons]`</span></span>
* <span data-ttu-id="8b368-1160">Добавлена поддержка операции обновления Azure Active Directory с помощью `aks update-credentials --reset-aad`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1160">Added support for Azure Active Directory updating operation using `aks update-credentials --reset-aad`</span></span>
* <span data-ttu-id="8b368-1161">Добавлено пояснение, что значение `--output` для `aks get-credentials` игнорируется.</span><span class="sxs-lookup"><span data-stu-id="8b368-1161">Added clarification that `--output` is ignored for `aks get-credentials`</span></span>

### <a name="ams"></a><span data-ttu-id="8b368-1162">AMS</span><span class="sxs-lookup"><span data-stu-id="8b368-1162">AMS</span></span>
* <span data-ttu-id="8b368-1163">Добавлены команды `ams streaming-endpoint [start | stop | create | update] wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1163">Added `ams streaming-endpoint [start | stop | create | update] wait` commands</span></span>
* <span data-ttu-id="8b368-1164">Добавлены команды `ams live-event [create | start | stop | reset] wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1164">Added `ams live-event [create | start | stop | reset] wait` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1165">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-1165">Appservice</span></span>
* <span data-ttu-id="8b368-1166">Добавлена возможность создавать и настраивать функции с помощью контейнеров ACR.</span><span class="sxs-lookup"><span data-stu-id="8b368-1166">Added ability to create and configure functions using ACR containers</span></span>
* <span data-ttu-id="8b368-1167">Добавлена поддержка обновления конфигураций веб-приложений с помощью JSON.</span><span class="sxs-lookup"><span data-stu-id="8b368-1167">Added support for updating webapp configurations through json</span></span>
* <span data-ttu-id="8b368-1168">Улучшена справка для `appservice-plan-update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1168">Improved help for `appservice-plan-update`</span></span>
* <span data-ttu-id="8b368-1169">Добавлена поддержка App Insights при создании приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="8b368-1169">Added support for app insights on functionapp create</span></span>
* <span data-ttu-id="8b368-1170">Устранены проблемы с SSH для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-1170">Fixed issues with webapp SSH</span></span>

### <a name="botservice"></a><span data-ttu-id="8b368-1171">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-1171">Botservice</span></span>
* <span data-ttu-id="8b368-1172">Улучшен пользовательский интерфейс для `bot publish`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1172">Improved UX for `bot publish`</span></span>
* <span data-ttu-id="8b368-1173">Добавлены предупреждения для времени ожидания при выполнении `npm install` во время операции `az bot publish`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1173">Added warning for timeouts when running `npm install` during `az bot publish`</span></span>
* <span data-ttu-id="8b368-1174">Удален недопустимый символ `.` из значения `--name` в `az bot create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1174">Removed invalid char `.` from `--name`  in `az bot create`</span></span>
* <span data-ttu-id="8b368-1175">Имена ресурсов больше не выбираются в случайном порядке при создании службы хранилища Azure, плана службы приложений, функций, веб-приложений и Application Insights.</span><span class="sxs-lookup"><span data-stu-id="8b368-1175">Changed to stop randomizing resource names when creating Azure Storage, App Service Plan, Function/Web App and Application Insights</span></span>
* <span data-ttu-id="8b368-1176">[УСТАРЕЛО] Аргумент `--proj-name` не рекомендуется к использованию. Вместо него теперь используется `--proj-file-path`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1176">[DEPRECATED] Deprecated `--proj-name` argument in favor of `--proj-file-path`</span></span>
* <span data-ttu-id="8b368-1177">Теперь `az bot publish` удаляет полученные файлы развертывания IIS Node.js, если они уже не существуют.</span><span class="sxs-lookup"><span data-stu-id="8b368-1177">Changed `az bot publish` to remove fetched IIS Node.js deployment files if they did not already exist</span></span>
* <span data-ttu-id="8b368-1178">В `az bot publish` добавлен аргумент `--keep-node-modules`, чтобы не удалять папку `node_modules` в Службе приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-1178">Added `--keep-node-modules` argument to `az bot publish` to not delete `node_modules` folder on App Service</span></span>
* <span data-ttu-id="8b368-1179">Добавлена пара "ключ — значение" `"publishCommand"` в выходные данные `az bot create` при создании бота веб-приложения или функции Azure.</span><span class="sxs-lookup"><span data-stu-id="8b368-1179">Added `"publishCommand"` key-value pair to output from `az bot create` when creating an Azure Function or Web App bot</span></span>
  * <span data-ttu-id="8b368-1180">Значение `"publishCommand"` — это команда `az bot publish` с предварительно заданными обязательными параметрами для публикации созданного бота.</span><span class="sxs-lookup"><span data-stu-id="8b368-1180">The value of `"publishCommand"` is an `az bot publish` command prepopulated with the required parameters to publish the newly created bot</span></span>
* <span data-ttu-id="8b368-1181">Обновлено значение `"WEBSITE_NODE_DEFAULT_VERSION"` в шаблоне ARM для ботов SDK версии 4: теперь вместо 8.9.4 указана версия 10.14.1.</span><span class="sxs-lookup"><span data-stu-id="8b368-1181">Updated `"WEBSITE_NODE_DEFAULT_VERSION"` in ARM template for v4 SDK bots to use 10.14.1 instead of 8.9.4</span></span>

### <a name="key-vault"></a><span data-ttu-id="8b368-1182">Key Vault</span><span class="sxs-lookup"><span data-stu-id="8b368-1182">Key Vault</span></span>
* <span data-ttu-id="8b368-1183">Исправлена проблема с `keyvault secret backup`, из-за которой некоторые пользователи получали сообщение об ошибке `unexpected_keyword` при использовании `--id`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1183">Fixed issue with `keyvault secret backup` where some users received an `unexpected_keyword` error when using `--id`</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-1184">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-1184">Monitor</span></span>
* <span data-ttu-id="8b368-1185">Параметр `monitor metrics alert [create|update]` теперь допускает значение измерения `*`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1185">Changed `monitor metrics alert [create|update]` to allow dimension value `*`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1186">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1186">Network</span></span>
* <span data-ttu-id="8b368-1187">Изменено значение `dns zone export` для поддержки экспорта записей CNAME как FQDN.</span><span class="sxs-lookup"><span data-stu-id="8b368-1187">Changed `dns zone export` to ensure exported CNAMEs are FQDNs</span></span>
* <span data-ttu-id="8b368-1188">В `nic ip-config address-pool [add|remove]` добавлен параметр `--gateway-name` для поддержки серверных пулов адресов шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-1188">Added `--gateway-name` parameter to `nic ip-config address-pool [add|remove]` to support application gateway backend address pools</span></span>
* <span data-ttu-id="8b368-1189">В `network watcher flow-log configure` добавлены аргументы `--traffic-analytics` и `--workspace` для поддержки аналитики трафика через рабочую область Log Analytics.</span><span class="sxs-lookup"><span data-stu-id="8b368-1189">Added `--traffic-analytics` and `--workspace` arguments to `network watcher flow-log configure` to support traffic analytics through a Log Analytics workspace</span></span>
* <span data-ttu-id="8b368-1190">В `lb inbound-nat-pool [create|update]` добавлены аргументы `--idle-timeout` и `--floating-ip`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1190">Added `--idle-timeout` and `--floating-ip` to `lb inbound-nat-pool [create|update]`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="8b368-1191">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="8b368-1191">Policy Insights</span></span>
* <span data-ttu-id="8b368-1192">Добавлены команды `policy remediation` для поддержки функций исправления политики ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1192">Added `policy remediation` commands to support resource policy remediation features</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-1193">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="8b368-1193">RDBMS</span></span>
* <span data-ttu-id="8b368-1194">Улучшено справочное сообщение и параметры команды.</span><span class="sxs-lookup"><span data-stu-id="8b368-1194">Improved help message and command parameters</span></span>

### <a name="redis"></a><span data-ttu-id="8b368-1195">Redis</span><span class="sxs-lookup"><span data-stu-id="8b368-1195">Redis</span></span>
* <span data-ttu-id="8b368-1196">Добавлены команды для управления правилами брандмауэра (create, update, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="8b368-1196">Added commands for managing firewall-rules (create, update, delete, show, list)</span></span>
* <span data-ttu-id="8b368-1197">Добавлены команды для управления подключением к серверу (create, delete, show, list).</span><span class="sxs-lookup"><span data-stu-id="8b368-1197">Added commands for managing server-link (create, delete, show, list)</span></span>
* <span data-ttu-id="8b368-1198">Добавлены команды для управления расписанием установки исправлений (create, update, delete, show).</span><span class="sxs-lookup"><span data-stu-id="8b368-1198">Added commands for managing patch-schedule (create, update, delete, show)</span></span>
* <span data-ttu-id="8b368-1199">Добавлена поддержка Зон доступности и минимальной версии TLS для операции \`redis create.</span><span class="sxs-lookup"><span data-stu-id="8b368-1199">Added support for Availability Zones and Minimum TLS Version to \`redis create</span></span>
* <span data-ttu-id="8b368-1200">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены команды `redis update-settings` и `redis list-all`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1200">[BREAKING CHANGE] Removed `redis update-settings` and `redis list-all` commands</span></span>
* <span data-ttu-id="8b368-1201">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр для `redis create`: 'tenant settings' не принимается в формате key[=value].</span><span class="sxs-lookup"><span data-stu-id="8b368-1201">[BREAKING CHANGE] Parameter for `redis create`: 'tenant settings' is not accepted in key[=value] format</span></span>
* <span data-ttu-id="8b368-1202">[УСТАРЕЛО] Добавлено предупреждающее сообщение о том, что команда `redis import-method` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b368-1202">[DEPRECATED] Added warning message for deprecating `redis import-method` command</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1203">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1203">Role</span></span>
* <span data-ttu-id="8b368-1204">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в этот раздел из группы команд `vm`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1204">[BREAKING CHANGE] Moved `az identity` command here from `vm` commands</span></span>

### <a name="sql-vm"></a><span data-ttu-id="8b368-1205">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-1205">SQL VM</span></span>
* <span data-ttu-id="8b368-1206">[УСТАРЕЛО] Аргумент `--boostrap-acc-pwd` больше не поддерживается из-за опечатки.</span><span class="sxs-lookup"><span data-stu-id="8b368-1206">[DEPRECATED] Deprecated `--boostrap-acc-pwd` argument due to typo</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1207">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1207">VM</span></span>
* <span data-ttu-id="8b368-1208">С параметром `vm list-skus` теперь можно использовать `--all` вместо `--all true`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1208">Changed `vm list-skus` to allow use of `--all` in place of `--all true`</span></span>
* <span data-ttu-id="8b368-1209">Добавлена команда `vmss run-command [invoke | list | show]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1209">Added `vmss run-command [invoke | list | show]`</span></span>
* <span data-ttu-id="8b368-1210">Исправлена ошибка, из-за которой ранее запущенная команда `vmss encryption enable` прекращала работу.</span><span class="sxs-lookup"><span data-stu-id="8b368-1210">Fixed bug where `vmss encryption enable` would fail if run previously</span></span>
* <span data-ttu-id="8b368-1211">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `az identity` перемещена в группу команд `role`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1211">[BREAKING CHANGE] Moved `az identity` command to `role` commands</span></span>

## <a name="january-31-2019"></a><span data-ttu-id="8b368-1212">31 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1212">January 31, 2019</span></span>

<span data-ttu-id="8b368-1213">Версия 2.0.57</span><span class="sxs-lookup"><span data-stu-id="8b368-1213">Version 2.0.57</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1214">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1214">Core</span></span>

* <span data-ttu-id="8b368-1215">Исправлена [проблема 8399](https://github.com/Azure/azure-cli/issues/8399).</span><span class="sxs-lookup"><span data-stu-id="8b368-1215">Hot Fix for [issue 8399](https://github.com/Azure/azure-cli/issues/8399).</span></span>

## <a name="january-28-2019"></a><span data-ttu-id="8b368-1216">28 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1216">January 28, 2019</span></span>

<span data-ttu-id="8b368-1217">Версия 2.0.56</span><span class="sxs-lookup"><span data-stu-id="8b368-1217">Version 2.0.56</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1218">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1218">ACR</span></span>
* <span data-ttu-id="8b368-1219">Добавлена поддержка правил виртуальной сети и IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1219">Added support for VNet/IP rules</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1220">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1220">ACS</span></span>
* <span data-ttu-id="8b368-1221">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1221">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="8b368-1222">Добавлены команды управляемой платформы OpenShift.</span><span class="sxs-lookup"><span data-stu-id="8b368-1222">Added Managed OpenShift commands</span></span>
* <span data-ttu-id="8b368-1223">Добавлена поддержка операции обновления субъекта-службы с помощью `aks update-credentials -reset-service-principal`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1223">Added support for service principal updates operation with `aks update-credentials -reset-service-principal`</span></span>

### <a name="ams"></a><span data-ttu-id="8b368-1224">AMS</span><span class="sxs-lookup"><span data-stu-id="8b368-1224">AMS</span></span>
* <span data-ttu-id="8b368-1225">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams asset get-streaming-locators` переименована в `ams asset list-streaming-locators`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1225">[BREAKING CHANGE] Renamed `ams asset get-streaming-locators` to `ams asset list-streaming-locators`</span></span>
* <span data-ttu-id="8b368-1226">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming-locator get-content-keys` переименована в `ams streaming-locator list-content-keys`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1226">[BREAKING CHANGE] Renamed `ams streaming-locator get-content-keys` to `ams streaming-locator list-content-keys`</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1227">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-1227">Appservice</span></span>
* <span data-ttu-id="8b368-1228">Добавлена поддержка аналитики приложений для `functionapp create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1228">Added support for app insights on `functionapp create`</span></span>
* <span data-ttu-id="8b368-1229">Добавлена поддержка создания плана службы приложений (включая эластичный план "Премиум") для приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="8b368-1229">Added support for app service plan creation (including Elastic Premium) to Function Apps</span></span>
* <span data-ttu-id="8b368-1230">Исправлены проблемы с настройкой приложений для эластичных планов "Премиум".</span><span class="sxs-lookup"><span data-stu-id="8b368-1230">Fixed app setting issues with Elastic Premium plans</span></span>

### <a name="container"></a><span data-ttu-id="8b368-1231">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-1231">Container</span></span>
* <span data-ttu-id="8b368-1232">Добавлена команда `container start`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1232">Added `container start` command</span></span>
* <span data-ttu-id="8b368-1233">Теперь можно использовать десятичные значения для ЦП при создании контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-1233">Changed to allow using decimal values for CPU during container creation</span></span>

### <a name="eventgrid"></a><span data-ttu-id="8b368-1234">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="8b368-1234">EventGrid</span></span>
* <span data-ttu-id="8b368-1235">Добавлен параметр `--deadletter-endpoint` для команды `event-subscription [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1235">Added `--deadletter-endpoint` parameter to `event-subscription [create|update]`</span></span>
* <span data-ttu-id="8b368-1236">Добавлены новые значения storagequeue и hybridconnection для 'event-subscription [create|update] --endpoint-type\`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1236">Added storagequeue and hybridconnection as new values for 'event-subscription [create|update] --endpoint-type\`</span></span>
* <span data-ttu-id="8b368-1237">В `event-subscription create` добавлены параметры `--max-delivery-attempts` и `--event-ttl`, чтобы указывать политику повтора для событий.</span><span class="sxs-lookup"><span data-stu-id="8b368-1237">Added `--max-delivery-attempts` and `--event-ttl` parameters to `event-subscription create` to specify the retry policy for events</span></span>
* <span data-ttu-id="8b368-1238">В `event-subscription [create|update]` добавлено предупреждающее сообщение, которое отображается, когда в качестве целевого объекта для подписки на события используется веб-перехватчик.</span><span class="sxs-lookup"><span data-stu-id="8b368-1238">Added a warning message to `event-subscription [create|update]` when webhook as destination is used for an event subscription</span></span>
* <span data-ttu-id="8b368-1239">Добавлен параметр source-resource-id для всех команд, связанных с подпиской на событие, при этом все остальные параметры исходного ресурса помечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="8b368-1239">Added source-resource-id parameter for all event subscription related commands and mark all other source resource related parameters as deprecated</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8b368-1240">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b368-1240">HDInsight</span></span>
* <span data-ttu-id="8b368-1241">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight [application] create` удалены параметры `--virtual-network` и `--subnet-name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1241">[BREAKING CHANGE] Removed the `--virtual-network` and `--subnet-name` parameters from `hdinsight [application] create`</span></span>
* <span data-ttu-id="8b368-1242">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`hdinsight create --storage-account` теперь принимает имя или идентификатор учетной записи хранения вместо конечных точек BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1242">[BREAKING CHANGE] Changed `hdinsight create --storage-account` to accept name or id of storage account instead of blob endpoints</span></span>
* <span data-ttu-id="8b368-1243">Добавлены параметры `--vnet-name` и `--subnet-name` для `hdinsight create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1243">Added `--vnet-name` and `--subnet-name` parameters to `hdinsight create`</span></span>
* <span data-ttu-id="8b368-1244">Для `hdinsight create` добавлена поддержка Корпоративного пакета безопасности и шифрования дисков.</span><span class="sxs-lookup"><span data-stu-id="8b368-1244">Added support for Enterprise Security Package and disk encryption to `hdinsight create`</span></span> 
* <span data-ttu-id="8b368-1245">Добавлена команда `hdinsight rotate-disk-encryption-key`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1245">Added `hdinsight rotate-disk-encryption-key` command</span></span>
* <span data-ttu-id="8b368-1246">Добавлена команда `hdinsight update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1246">Added `hdinsight update` command</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-1247">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-1247">IoT</span></span>
* <span data-ttu-id="8b368-1248">Добавлен формат кодирования для команды routing-endpoint.</span><span class="sxs-lookup"><span data-stu-id="8b368-1248">Added encoding format to routing-endpoint command</span></span>

### <a name="kusto"></a><span data-ttu-id="8b368-1249">Kusto</span><span class="sxs-lookup"><span data-stu-id="8b368-1249">Kusto</span></span>
* <span data-ttu-id="8b368-1250">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="8b368-1250">Preview release</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-1251">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-1251">Monitor</span></span>
* <span data-ttu-id="8b368-1252">Теперь при сравнении идентификаторов не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="8b368-1252">Changed ID comparison to be case insensitive</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-1253">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-1253">Profile</span></span>
* <span data-ttu-id="8b368-1254">Теперь при операции `login` можно использовать учетную запись уровня клиента для управляемого удостоверения службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-1254">Enable tenant level account for managed service identity for `login`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1255">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1255">Network</span></span>
* <span data-ttu-id="8b368-1256">Исправлена проблема с `express-route update`, из-за которой игнорировался аргумент `--bandwidth`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1256">Fixed issue with `express-route update`: where `--bandwidth` argument was ignored</span></span>
* <span data-ttu-id="8b368-1257">Исправлена проблема с `ddos-protection update`, из-за которой определение набора вызывало трассировку стека.</span><span class="sxs-lookup"><span data-stu-id="8b368-1257">Fixed issue with `ddos-protection update` where set comprehension caused stack trace</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-1258">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-1258">Resource</span></span>
* <span data-ttu-id="8b368-1259">Добавлена поддержка файла параметров URI для `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1259">Added support for URI parameters file to `group deployment create`</span></span>
* <span data-ttu-id="8b368-1260">Добавлена поддержка управляемого удостоверения для `policy assignment [create|list|show]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1260">Added support for managed identity to `policy assignment [create|list|show]`</span></span>

### <a name="sql-virtual-machine"></a><span data-ttu-id="8b368-1261">Виртуальная машина SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-1261">SQL Virtual Machine</span></span>
* <span data-ttu-id="8b368-1262">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="8b368-1262">Preview release</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1263">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1263">Storage</span></span>
* <span data-ttu-id="8b368-1264">Теперь исправление обновляет только свойства, измененные в том же объекте.</span><span class="sxs-lookup"><span data-stu-id="8b368-1264">Changed fix to update only properties that are changed on the same object</span></span>
* <span data-ttu-id="8b368-1265">Исправлена проблема 8021. Двоичные данные кодируются в кодировке Base64 при возврате.</span><span class="sxs-lookup"><span data-stu-id="8b368-1265">Fixed #8021, binary data is encoded in base 64 when returned</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1266">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1266">VM</span></span>
* <span data-ttu-id="8b368-1267">`vm encryption enable` теперь проверяет хранилище ключей для шифрования диска и наличие хранилища ключей для шифрования ключа.</span><span class="sxs-lookup"><span data-stu-id="8b368-1267">Changed `vm encryption enable` to validate disk encryption keyvault and that key encryption keyvault exists</span></span>
* <span data-ttu-id="8b368-1268">Добавлен флаг `--force` в `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1268">Added `--force` flag to `vm encryption enable`</span></span>

## <a name="january-15-2019"></a><span data-ttu-id="8b368-1269">15 января 2019 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1269">January 15, 2019</span></span>

<span data-ttu-id="8b368-1270">Версия 2.0.55</span><span class="sxs-lookup"><span data-stu-id="8b368-1270">Version 2.0.55</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1271">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1271">ACR</span></span>
* <span data-ttu-id="8b368-1272">Теперь можно принудительно отправлять несуществующую диаграмму Helm.</span><span class="sxs-lookup"><span data-stu-id="8b368-1272">Changed to allow force push a helm chart that doesn't exist</span></span>
* <span data-ttu-id="8b368-1273">Разрешены операции среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="8b368-1273">changed to allow runtime operations without ARM requests</span></span>
* <span data-ttu-id="8b368-1274">[УСТАРЕЛО] Параметр `--resource-group` больше не поддерживается в следующих командах:</span><span class="sxs-lookup"><span data-stu-id="8b368-1274">[DEPRECATED] Deprecated `--resource-group` parameter in the commands:</span></span>
  * `acr login`
  * `acr repository`
  * `acr helm`

### <a name="acs"></a><span data-ttu-id="8b368-1275">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1275">ACS</span></span>
* <span data-ttu-id="8b368-1276">Добавлена поддержка новых регионов ACI.</span><span class="sxs-lookup"><span data-stu-id="8b368-1276">Added support for new ACI regions</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1277">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-1277">Appservice</span></span>
* <span data-ttu-id="8b368-1278">Устранена проблема с отправкой сертификатов для приложений, размещенных в среде службы приложений (ASE) с разными группами ресурсов ASE и приложения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1278">Fixed issue with uploading certificates for apps that are hosted on an ASE, where the ASE RG & App RG are different</span></span>
* <span data-ttu-id="8b368-1279">Теперь `webapp up` по умолчанию использует SKU P1V1 для Linux.</span><span class="sxs-lookup"><span data-stu-id="8b368-1279">Changed `webapp up` to use SKU P1V1 as default for Linux</span></span>
* <span data-ttu-id="8b368-1280">Теперь `[webapp|functionapp] deployment source config-zip` отображает правильное сообщение об ошибке при неудачном развертывании.</span><span class="sxs-lookup"><span data-stu-id="8b368-1280">Fixed `[webapp|functionapp] deployment source config-zip` to show the right error message when a deployment fails</span></span> 
* <span data-ttu-id="8b368-1281">Добавлена команда `webapp ssh`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1281">Added `webapp ssh` command</span></span>

### <a name="botservice"></a><span data-ttu-id="8b368-1282">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-1282">Botservice</span></span>
* <span data-ttu-id="8b368-1283">Добавлены обновления состояния развертывания для `bot create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1283">Added deployment status updates to `bot create`</span></span>

### <a name="configure"></a><span data-ttu-id="8b368-1284">Configure</span><span class="sxs-lookup"><span data-stu-id="8b368-1284">Configure</span></span>
* <span data-ttu-id="8b368-1285">Добавлен настраиваемый формат выходных данных `none`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1285">Added `none` as a configurable output format</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8b368-1286">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-1286">CosmosDB</span></span>
* <span data-ttu-id="8b368-1287">Добавлена поддержка создания базы данных с общей пропускной способностью.</span><span class="sxs-lookup"><span data-stu-id="8b368-1287">Added support for creating database with shared throughput</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8b368-1288">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b368-1288">HDInsight</span></span>
* <span data-ttu-id="8b368-1289">Добавлены команды для управления приложениями.</span><span class="sxs-lookup"><span data-stu-id="8b368-1289">Added commands for managing applications</span></span>
* <span data-ttu-id="8b368-1290">Добавлены команды для управления действиями скриптов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1290">Added commands for managing script actions</span></span>
* <span data-ttu-id="8b368-1291">Добавлены команды для управления Operations Management Suite (OMS).</span><span class="sxs-lookup"><span data-stu-id="8b368-1291">Added commands for managing Operations Management Suite (OMS)</span></span>
* <span data-ttu-id="8b368-1292">Добавлена поддержка регионального использования списка для `hdinsight list-usage`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1292">Added support to list regional usage to `hdinsight list-usage`</span></span>
* <span data-ttu-id="8b368-1293">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Из `hdinsight create` удален тип кластера по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1293">[BREAKING CHANGE] Removed default cluster type from `hdinsight create`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1294">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1294">Network</span></span>
* <span data-ttu-id="8b368-1295">Добавлены аргументы `--custom-headers` и `--status-code-ranges` для команды `traffic-manager profile [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8b368-1295">Added `--custom-headers` and `--status-code-ranges` arguments to `traffic-manager profile [create|update]`</span></span>
* <span data-ttu-id="8b368-1296">Добавлены новые типы маршрутизации: "Подсеть" и "Многозначный".</span><span class="sxs-lookup"><span data-stu-id="8b368-1296">Added new routing types: Subnet and Multivalue</span></span>
* <span data-ttu-id="8b368-1297">Добавлены аргументы `--custom-headers` и `--subnets` для команды `traffic-manager endpoint [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8b368-1297">Added `--custom-headers` and `--subnets` arguments to `traffic-manager endpoint [create|update]`</span></span>  
* <span data-ttu-id="8b368-1298">Исправлена проблема с возникновением ошибки при указании значения `--vnets ""` для `ddos-protection update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1298">Fixed issue where supplying `--vnets ""` to `ddos-protection update` caused an error</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1299">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1299">Role</span></span>
* <span data-ttu-id="8b368-1300">[УСТАРЕЛО] Аргумент `--password` для `create-for-rbac` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b368-1300">[DEPRECATED] Deprecated `--password` argument for `create-for-rbac`.</span></span> <span data-ttu-id="8b368-1301">Используйте вместо него надежные пароли, сгенерированные CLI.</span><span class="sxs-lookup"><span data-stu-id="8b368-1301">Use secure passwords generated by the CLI instead</span></span>

### <a name="security"></a><span data-ttu-id="8b368-1302">безопасность</span><span class="sxs-lookup"><span data-stu-id="8b368-1302">Security</span></span>
* <span data-ttu-id="8b368-1303">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="8b368-1303">Initial Release</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1304">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1304">Storage</span></span>
* <span data-ttu-id="8b368-1305">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Количество результатов по умолчанию для `storage [blob|file|container|share] list` теперь 5000.</span><span class="sxs-lookup"><span data-stu-id="8b368-1305">[BREAKING CHANGE] Changed `storage [blob|file|container|share] list` default number of results to be 5,000.</span></span> <span data-ttu-id="8b368-1306">Для возврата всех результатов как ранее используйте `--num-results *`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1306">Use `--num-results *` for original behavior of returning all results</span></span>
* <span data-ttu-id="8b368-1307">Добавлен параметр `--marker` для команды `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1307">Added `--marker` parameter to `storage [blob|file|container|share] list`</span></span>
* <span data-ttu-id="8b368-1308">Добавлена отметка журнала для следующей страницы в STDERR для `storage [blob|file|container|share] list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1308">Added log marker for next page to STDERR for `storage [blob|file|container|share] list`</span></span> 
* <span data-ttu-id="8b368-1309">Добавлена команда `storage blob service-properties update` с поддержкой статических веб-сайтов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1309">Added `storage blob service-properties update` command with support for static websites</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1310">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1310">VM</span></span>
* <span data-ttu-id="8b368-1311">`vm [disk|unmanaged-disk]` и `vmss disk` изменены для лучшего согласования параметров.</span><span class="sxs-lookup"><span data-stu-id="8b368-1311">Changed `vm [disk|unmanaged-disk]` and `vmss disk` to have more consistent parameters</span></span>
* <span data-ttu-id="8b368-1312">Добавлена поддержка перекрестных ссылок на образы клиента для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1312">Added support for cross tenant image referencing to `[vm|vmss] create`</span></span>
* <span data-ttu-id="8b368-1313">Исправлена ошибка конфигурации по умолчанию в `vm diagnostics get-default-config --windows-os`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1313">Fixed bug with default configuration in `vm diagnostics get-default-config --windows-os`</span></span>
* <span data-ttu-id="8b368-1314">В `vmss extension set` добавлен аргумент `--provision-after-extensions` для определения расширений, которые необходимо подготовить перед настройкой.</span><span class="sxs-lookup"><span data-stu-id="8b368-1314">Added argument `--provision-after-extensions` to `vmss extension set` to define what extensions must be provisioned before the extension being set</span></span>
* <span data-ttu-id="8b368-1315">В `sig image-version update` добавлен аргумент `--replica-count` для определения числа репликаций по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1315">Added argument `--replica-count` to `sig image-version update` for setting the default replication count</span></span>
* <span data-ttu-id="8b368-1316">Исправлена ошибка `image create --source`, из-за которой диск ОС ошибочно принимался за виртуальную машину с тем же именем даже при указании полного идентификатора ресурса.</span><span class="sxs-lookup"><span data-stu-id="8b368-1316">Fixed bug with `image create --source` where source os disk is mistaken for a VM with the same name, even if the full resource ID is provided</span></span>

## <a name="december-20-2018"></a><span data-ttu-id="8b368-1317">20 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1317">December 20, 2018</span></span>

<span data-ttu-id="8b368-1318">Версия 2.0.54</span><span class="sxs-lookup"><span data-stu-id="8b368-1318">Version 2.0.54</span></span>
### <a name="appservice"></a><span data-ttu-id="8b368-1319">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-1319">Appservice</span></span>
* <span data-ttu-id="8b368-1320">Исправлена ошибка, когда при повторном развертывании `webapp up` возникала ошибка.</span><span class="sxs-lookup"><span data-stu-id="8b368-1320">Fixed issue where `webapp up` would fail to redeploy</span></span>
* <span data-ttu-id="8b368-1321">Добавлена возможность вывода списка моментальных снимков веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="8b368-1321">Added support for listing and restoring webapp snapshots</span></span>
* <span data-ttu-id="8b368-1322">Добавлена поддержка флага `--runtime` в приложениях-функциях Windows.</span><span class="sxs-lookup"><span data-stu-id="8b368-1322">Added support for `--runtime` flag to Windows function apps</span></span>

### <a name="iotcentral"></a><span data-ttu-id="8b368-1323">IoT Central</span><span class="sxs-lookup"><span data-stu-id="8b368-1323">IoTCentral</span></span>
* <span data-ttu-id="8b368-1324">Исправлен вызов API в команде обновления.</span><span class="sxs-lookup"><span data-stu-id="8b368-1324">Fixed update command API call</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1325">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1325">Role</span></span>
* <span data-ttu-id="8b368-1326">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию `ad [app|sp] list` теперь возвращает только первые 100 объектов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1326">[BREAKING CHANGE] Changed `ad [app|sp] list` to only list the first 100 objects by default</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-1327">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-1327">SQL</span></span>
* <span data-ttu-id="8b368-1328">Добавлена поддержка пользовательских параметров сортировки в управляемых экземплярах.</span><span class="sxs-lookup"><span data-stu-id="8b368-1328">Added support for custom collation on managed instances</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1329">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1329">VM</span></span>
* <span data-ttu-id="8b368-1330">Добавлен параметр `---os-type` для команды `disk create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1330">Added `---os-type` parameter to `disk create`</span></span>

## <a name="december-18-2018"></a><span data-ttu-id="8b368-1331">18 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1331">December 18, 2018</span></span>

<span data-ttu-id="8b368-1332">Версия 2.0.53</span><span class="sxs-lookup"><span data-stu-id="8b368-1332">Version 2.0.53</span></span>
### <a name="acr"></a><span data-ttu-id="8b368-1333">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1333">ACR</span></span>
* <span data-ttu-id="8b368-1334">Добавлена поддержка импорта изображений из внешних реестров контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-1334">Added support for image import from external Container Registries</span></span>
* <span data-ttu-id="8b368-1335">Сжатый табличный макет для списка задач.</span><span class="sxs-lookup"><span data-stu-id="8b368-1335">Condensed the table layout for task list</span></span>
* <span data-ttu-id="8b368-1336">Добавлена поддержка URL-адресов Azure DevOps.</span><span class="sxs-lookup"><span data-stu-id="8b368-1336">Added support for Azure DevOps URLs</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1337">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1337">ACS</span></span>
* <span data-ttu-id="8b368-1338">Добавлена предварительная версия виртуальных узлов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1338">Added Virtual Nodes Preview</span></span>
* <span data-ttu-id="8b368-1339">Из аргументов команды `aks create` удалено "(PREVIEW)".</span><span class="sxs-lookup"><span data-stu-id="8b368-1339">Removed "(PREVIEW)" from AAD arguments to `aks create`</span></span>
* <span data-ttu-id="8b368-1340">[УСТАРЕЛО] Команды `az acs` больше не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8b368-1340">[DEPRECATED] Deprecated `az acs` commands.</span></span> <span data-ttu-id="8b368-1341">Служба ACS будет выведена из эксплуатации 31 января 2020 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1341">The ACS service will retire on January 31, 2020</span></span>
* <span data-ttu-id="8b368-1342">Добавлена поддержка политики сети для создания новых кластеров AKS.</span><span class="sxs-lookup"><span data-stu-id="8b368-1342">Added support of Network Policy when creating new AKS clusters</span></span>
* <span data-ttu-id="8b368-1343">Аргумент `--nodepool-name` команды `aks scale` больше не является обязательным, если есть только один пул узлов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1343">Removed requirement of `--nodepool-name` argument for `aks scale` if there's only one nodepool</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1344">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-1344">Appservice</span></span>
* <span data-ttu-id="8b368-1345">Исправлена проблема, когда команда `webapp config container` не учитывала параметр `--slot`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1345">Fixed issue where `webapp config container` did not honor `--slot` parameter</span></span>

### <a name="botservice"></a><span data-ttu-id="8b368-1346">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-1346">Botservice</span></span>
* <span data-ttu-id="8b368-1347">Добавлена поддержка анализа файла `.bot` при вызове `bot show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1347">Added support for `.bot` file parsing when calling `bot show`</span></span>
* <span data-ttu-id="8b368-1348">Исправлена ошибка подготовки AppInsights.</span><span class="sxs-lookup"><span data-stu-id="8b368-1348">Fixed AppInsights provisioning bug</span></span>
* <span data-ttu-id="8b368-1349">Исправлена ошибка с пробелами при работе с путями к файлам.</span><span class="sxs-lookup"><span data-stu-id="8b368-1349">Fixed whitespace bug when dealing with file paths</span></span>
* <span data-ttu-id="8b368-1350">Уменьшено количество сетевых вызовов Kudu.</span><span class="sxs-lookup"><span data-stu-id="8b368-1350">Reduced Kudu network calls</span></span>
* <span data-ttu-id="8b368-1351">Улучшен пользовательский интерфейс общих команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-1351">General command UX improvements</span></span>

### <a name="consumption"></a><span data-ttu-id="8b368-1352">Потребление</span><span class="sxs-lookup"><span data-stu-id="8b368-1352">Consumption</span></span>
* <span data-ttu-id="8b368-1353">Исправлены ошибки в API бюджета для отображения уведомлений.</span><span class="sxs-lookup"><span data-stu-id="8b368-1353">Fixed bugs for budget API to show notifications</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8b368-1354">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-1354">CosmosDB</span></span>
* <span data-ttu-id="8b368-1355">Добавлена возможность преобразования учетной записи из типа "несколько источников" в тип "один источник".</span><span class="sxs-lookup"><span data-stu-id="8b368-1355">Added support for updating account from multi-master to single-master</span></span>

### <a name="maps"></a><span data-ttu-id="8b368-1356">Maps</span><span class="sxs-lookup"><span data-stu-id="8b368-1356">Maps</span></span>
* <span data-ttu-id="8b368-1357">В `maps account [create|update]` добавлена поддержка SKU S1.</span><span class="sxs-lookup"><span data-stu-id="8b368-1357">Added support for the S1 SKU to `maps account [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1358">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1358">Network</span></span>
* <span data-ttu-id="8b368-1359">В команду `watcher flow-log configure` добавлена поддержка аргументов `--format` и `--log-version`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1359">Added support for `--format` and `--log-version` to `watcher flow-log configure`</span></span>
* <span data-ttu-id="8b368-1360">Исправлена проблема с командой `dns zone update`, когда использование "" для очистки виртуальных сетей разрешения имен и регистрации не работало.</span><span class="sxs-lookup"><span data-stu-id="8b368-1360">Fixed issue with `dns zone update` where using "" to clear resolution and registration VNets didn't work</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-1361">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-1361">Resource</span></span>
* <span data-ttu-id="8b368-1362">Исправлена обработка параметра области для групп управления в `policy assignment [create|list|delete|show|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1362">Fixed handling of scope parameter for management groups in `policy assignment [create|list|delete|show|update]`</span></span> 
* <span data-ttu-id="8b368-1363">Добавлена новая команда `resource wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1363">Added new command `resource wait`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1364">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1364">Storage</span></span>
*  <span data-ttu-id="8b368-1365">В `storage logging update` добавлена возможность обновления версии схемы журнала для служб хранилища.</span><span class="sxs-lookup"><span data-stu-id="8b368-1365">Added ability to update log schema version for storage services in `storage logging update`</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1366">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1366">VM</span></span>
* <span data-ttu-id="8b368-1367">Исправлено аварийное завершение команды `vm identity remove`, когда указанной виртуальной машине не назначены удостоверения управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-1367">Fixed crash in `vm identity remove` when the specified vm has no assigned managed service identities</span></span>

## <a name="december-4-2018"></a><span data-ttu-id="8b368-1368">4 декабря 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1368">December 4, 2018</span></span>

<span data-ttu-id="8b368-1369">Версия 2.0.52</span><span class="sxs-lookup"><span data-stu-id="8b368-1369">Version 2.0.52</span></span>
### <a name="core"></a><span data-ttu-id="8b368-1370">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1370">Core</span></span>
* <span data-ttu-id="8b368-1371">Добавлена поддержка подготовки ресурсов нескольких клиентов для мультитенантного субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-1371">Added support for cross tenant resource provisioning for multi-tenant service principal</span></span>
* <span data-ttu-id="8b368-1372">Исправлена ошибка, когда идентификаторы, передаваемые по конвейеру из команды в формате выходных данных TSV, неправильно анализировались.</span><span class="sxs-lookup"><span data-stu-id="8b368-1372">Fixed bug where ids piped from a command with tsv output was improperly parsed</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1373">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-1373">Appservice</span></span>
* <span data-ttu-id="8b368-1374">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена команда `webapp up`, которая помогает создавать и развертывать содержимое для приложения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1374">[PREVIEW] Added `webapp up` command that helps in creating & deploying contents to app</span></span>
* <span data-ttu-id="8b368-1375">Исправлена ошибка в контейнерном приложении Windows из-за изменения в серверной части.</span><span class="sxs-lookup"><span data-stu-id="8b368-1375">Fixed a bug on container based windows app due to backend change</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1376">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1376">Network</span></span>
* <span data-ttu-id="8b368-1377">Добавлен аргумент `--exclusion` в `application-gateway waf-config set` для поддержки исключений WAF.</span><span class="sxs-lookup"><span data-stu-id="8b368-1377">Added `--exclusion` argument to `application-gateway waf-config set` to support WAF exclusions</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1378">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1378">Role</span></span>
* <span data-ttu-id="8b368-1379">Добавлена поддержка пользовательских идентификаторов для учетных данных и паролей.</span><span class="sxs-lookup"><span data-stu-id="8b368-1379">Added support for custom identifiers for password credential</span></span> 

### <a name="vm"></a><span data-ttu-id="8b368-1380">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1380">VM</span></span>
* <span data-ttu-id="8b368-1381">[УСТАРЕЛО] Параметр `vm extension [show|wait] --expand` больше не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8b368-1381">[DEPRECATED] Deprecated `vm extension [show|wait] --expand` parameter</span></span>
* <span data-ttu-id="8b368-1382">Добавлен параметр`--force` в `vm restart` для повторного развертывания виртуальных машин, которые не отвечают.</span><span class="sxs-lookup"><span data-stu-id="8b368-1382">Added `--force` parameter to `vm restart` to redeploy unresponsive VMs</span></span>
* <span data-ttu-id="8b368-1383">Изменено `[vm|vmss] create --authentication-type` для принятия all и создания виртуальной машины с использованием проверки подлинности на основе пароля и SSH.</span><span class="sxs-lookup"><span data-stu-id="8b368-1383">Changed `[vm|vmss] create --authentication-type` to accept "all" to create a VM with both password and ssh authentication</span></span>
* <span data-ttu-id="8b368-1384">Добавлен параметр `image create --os-disk-caching` для настройки кэширования дисков операционной системы для образа.</span><span class="sxs-lookup"><span data-stu-id="8b368-1384">Added `image create --os-disk-caching` parameter to set os disk caching for an image</span></span>

## <a name="november-20-2018"></a><span data-ttu-id="8b368-1385">20 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1385">November 20, 2018</span></span>

<span data-ttu-id="8b368-1386">Версия 2.0.51</span><span class="sxs-lookup"><span data-stu-id="8b368-1386">Version 2.0.51</span></span>
### <a name="core"></a><span data-ttu-id="8b368-1387">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1387">Core</span></span>
* <span data-ttu-id="8b368-1388">Изменена процедура входа с помощью MSI, чтобы исключить повторное использование имени подписки в удостоверении.</span><span class="sxs-lookup"><span data-stu-id="8b368-1388">Changed MSI login to not reuse subscription name in identity</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1389">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1389">ACR</span></span>
* <span data-ttu-id="8b368-1390">В шаг задачи добавлен токен контекста.</span><span class="sxs-lookup"><span data-stu-id="8b368-1390">Added context token to task step</span></span>
* <span data-ttu-id="8b368-1391">Добавлена поддержка для настройки секретов при запуске ACR для зеркалирования задачи ACR.</span><span class="sxs-lookup"><span data-stu-id="8b368-1391">Added support for setting secrets in acr run to mirror acr task</span></span>
* <span data-ttu-id="8b368-1392">Улучшена поддержка параметров `--top` и `--orderby` в командах `show-tags` и `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1392">Improved support for `--top` and `--orderby` for `show-tags` and `show-manifests` commands</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1393">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-1393">Appservice</span></span>
* <span data-ttu-id="8b368-1394">Для развертываний из ZIP-архивов изменено время ожидания по умолчанию при запросе состояния. Время ожидания увеличено до 5 минут, а также добавлено свойство timeout для настройки этого значения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1394">Changed zip deployment default timeout to poll for the status increased to 5 mins, also adding a timeout property to customize this value</span></span>
* <span data-ttu-id="8b368-1395">Обновлен номер версии `node_version` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1395">Updated the default `node_version`.</span></span> <span data-ttu-id="8b368-1396">При сбросе операции обмена слотами во время двухэтапного обмена сохраняются все настройки приложения и строки подключения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1396">Resetting slot swap action, during a two phase swap preserves all the appsettings & connection strings</span></span>
* <span data-ttu-id="8b368-1397">Отменена проверка номера SKU на стороне клиента при создании плана службы приложений для Linux.</span><span class="sxs-lookup"><span data-stu-id="8b368-1397">Removed client-side SKU check for Linux app service plan create</span></span>
* <span data-ttu-id="8b368-1398">Исправлена ошибка при попытке получения сведений о состоянии для развертывания из ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="8b368-1398">Fixed error when trying to get zipdeploy status</span></span>

### <a name="iotcentral"></a><span data-ttu-id="8b368-1399">IotCentral</span><span class="sxs-lookup"><span data-stu-id="8b368-1399">IotCentral</span></span>
* <span data-ttu-id="8b368-1400">Добавлена проверка доступности поддоменов при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="8b368-1400">Added subdomain availability check when creating an IoT Central application</span></span>

### <a name="keyvault"></a><span data-ttu-id="8b368-1401">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8b368-1401">KeyVault</span></span>
* <span data-ttu-id="8b368-1402">Исправлена проблема, при которой ошибки могли игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="8b368-1402">Fixed bug where errors may have been ignored</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1403">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1403">Network</span></span>
* <span data-ttu-id="8b368-1404">Добавлены подкоманды `root-cert` в `application-gateway` для обработки доверенных корневых сертификатов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1404">Added `root-cert` subcommands to `application-gateway` to handle trusted root certifcates</span></span>
* <span data-ttu-id="8b368-1405">В команду `application-gateway [create|update]` добавлены параметры `--min-capacity` и `--custom-error-pages`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1405">Added `--min-capacity` and `--custom-error-pages` options to `application-gateway [create|update]`:</span></span>
* <span data-ttu-id="8b368-1406">В команду `application-gateway create` добавлен параметр `--zones` для поддержки зоны доступности.</span><span class="sxs-lookup"><span data-stu-id="8b368-1406">Added `--zones` for availability zone support to `application-gateway create`</span></span> 
* <span data-ttu-id="8b368-1407">В команды `--request-body-check` и `application-gateway waf-config set` добавлены аргументы `--file-upload-limit` и `--max-request-body-size`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1407">Added arguments `--file-upload-limit`, `--max-request-body-size` and `--request-body-check` to `application-gateway waf-config set`</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-1408">Rdbms</span><span class="sxs-lookup"><span data-stu-id="8b368-1408">Rdbms</span></span>
* <span data-ttu-id="8b368-1409">Добавлены команды для виртуальной сети MariaDB.</span><span class="sxs-lookup"><span data-stu-id="8b368-1409">Added mariadb vnet commands</span></span>

### <a name="rbac"></a><span data-ttu-id="8b368-1410">RBAC:</span><span class="sxs-lookup"><span data-stu-id="8b368-1410">Rbac</span></span>
* <span data-ttu-id="8b368-1411">Исправлена проблема при попытке обновления неизменяемых учетных данных в `ad app update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1411">Fixed an issue with attempting to update immutable credentials in `ad app update`</span></span>
* <span data-ttu-id="8b368-1412">В выходные данные `ad [app|sp] list` добавлены предупреждения о критических изменениях, ожидаемых в ближайшем будущем.</span><span class="sxs-lookup"><span data-stu-id="8b368-1412">Added output warnings to communicate breaking changes in the near future for `ad [app|sp] list`</span></span> 

### <a name="storage"></a><span data-ttu-id="8b368-1413">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1413">Storage</span></span>
* <span data-ttu-id="8b368-1414">Улучшена обработка нетипичных случаев в командах копирования хранилища.</span><span class="sxs-lookup"><span data-stu-id="8b368-1414">Improved handling of corner cases for storage copy commands</span></span>
* <span data-ttu-id="8b368-1415">Исправлена проблема, когда команда `storage blob copy start-batch` не использовала учетные данные для входа при совпадении учетных записей для исходного и целевого объектов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1415">Fixed issue with `storage blob copy start-batch` not using login credentials when the destination and source accounts are the same</span></span>
* <span data-ttu-id="8b368-1416">Исправлена ошибка в команде `storage [blob|file] url`, когда параметр `sas_token` не включался в URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="8b368-1416">Fixed bug with`storage [blob|file] url` where `sas_token` wasn't incorporated into URL</span></span>
* <span data-ttu-id="8b368-1417">В команду `[blob|container] list` добавлено предупреждение о критическом изменении со сведениями о том, что по умолчанию будут выводиться только первые 5000 результатов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1417">Added breaking change warning to `[blob|container] list`: will soon output only first 5000 results by default</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1418">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1418">VM</span></span>
* <span data-ttu-id="8b368-1419">В `[vm|vmss] create --storage-sku` добавлена возможность указать номер SKU учетной записи хранения отдельно для управляемых дисков с ОС и данными.</span><span class="sxs-lookup"><span data-stu-id="8b368-1419">Added support to `[vm|vmss] create --storage-sku` to specify the storage account SKU for managed OS and data disks separately</span></span>
* <span data-ttu-id="8b368-1420">Изменены параметры для имени версии в `sig image-version`. Теперь используются параметры `--image-version -e`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1420">Changed version name parameters to `sig image-version` to be `--image-version -e`</span></span>
* <span data-ttu-id="8b368-1421">Аргумент `--image-version-name` в команде `sig image-version` отмечен как нерекомендуемый. Он заменен на `--image-version`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1421">Deprecated `sig image-version` argument `--image-version-name`, replaced by `--image-version`</span></span>
* <span data-ttu-id="8b368-1422">В `[vm|vmss] create --ephemeral-os-disk` добавлена поддержка для использования локального диска с ОС.</span><span class="sxs-lookup"><span data-stu-id="8b368-1422">Added support to use local OS disk to `[vm|vmss] create --ephemeral-os-disk`</span></span>
* <span data-ttu-id="8b368-1423">Добавлена поддержка параметра `--no-wait` в команде `snapshot create/update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1423">Added support for `--no-wait` to `snapshot create/update`</span></span>
* <span data-ttu-id="8b368-1424">Добавлена команда `snapshot wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1424">Added `snapshot wait` command</span></span>
* <span data-ttu-id="8b368-1425">Добавлена поддержка для использования имени экземпляра в `[vm|vmss] extension set --extension-instance-name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1425">Added support for using instance name with `[vm|vmss] extension set --extension-instance-name`</span></span>

## <a name="november-6-2018"></a><span data-ttu-id="8b368-1426">6 ноября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1426">November 6, 2018</span></span>

<span data-ttu-id="8b368-1427">Версия 2.0.50</span><span class="sxs-lookup"><span data-stu-id="8b368-1427">Version 2.0.50</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1428">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1428">Core</span></span>
* <span data-ttu-id="8b368-1429">Добавлена поддержка аутентификации субъекта-службы с помощью имени и издателя сертификата.</span><span class="sxs-lookup"><span data-stu-id="8b368-1429">Added support for service principal sn+issuer auth</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1430">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1430">ACR</span></span>
* <span data-ttu-id="8b368-1431">Добавлена поддержка событий git для фиксаций и запросов на вытягивание для исходного триггера задачи.</span><span class="sxs-lookup"><span data-stu-id="8b368-1431">Added support for commit and pull request git events for Task source trigger</span></span>
* <span data-ttu-id="8b368-1432">Внесено изменение для использования файла Dockerfile по умолчанию, если он не указан в команде build.</span><span class="sxs-lookup"><span data-stu-id="8b368-1432">Changed to use default Dockerfile if it's not specified in build command</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1433">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1433">ACS</span></span>
* <span data-ttu-id="8b368-1434">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `enable_cloud_console_aks_browse`, чтобы активировать az aks browse по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1434">[BREAKING CHANGE] Removed `enable_cloud_console_aks_browse` to enable 'az aks browse' by default</span></span>

### <a name="advisor"></a><span data-ttu-id="8b368-1435">Помощник</span><span class="sxs-lookup"><span data-stu-id="8b368-1435">Advisor</span></span>
* <span data-ttu-id="8b368-1436">Выпуск общедоступной версии</span><span class="sxs-lookup"><span data-stu-id="8b368-1436">GA release</span></span>

### <a name="ams"></a><span data-ttu-id="8b368-1437">AMS</span><span class="sxs-lookup"><span data-stu-id="8b368-1437">AMS</span></span>
* <span data-ttu-id="8b368-1438">Добавлены новые группы команд:</span><span class="sxs-lookup"><span data-stu-id="8b368-1438">Added new command groups:</span></span>
  *  `ams account-filter`
  *  `ams asset-filter`
  *  `ams content-key-policy`
  *  `ams live-event`
  *  `ams live-output`
  *  `ams streaming-endpoint`
  *  `ams mru`
* <span data-ttu-id="8b368-1439">Добавлены новые команды:</span><span class="sxs-lookup"><span data-stu-id="8b368-1439">Added new commands:</span></span>
  * `ams account check-name`
  * `ams job update`
  * `ams asset get-encryption-key`
  * `ams asset get-streaming-locators`
  * `ams streaming-locator get-content-keys`
* <span data-ttu-id="8b368-1440">Добавлена поддержка параметров шифрования в `ams streaming-policy create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1440">Added encryption parameters support to `ams streaming-policy create`</span></span>
* <span data-ttu-id="8b368-1441">Добавлена поддержка операции `ams transform output remove` путем передачи выходного индекса для удаления.</span><span class="sxs-lookup"><span data-stu-id="8b368-1441">Added support to `ams transform output remove` now can be performed by passing the output index to remove</span></span>
* <span data-ttu-id="8b368-1442">Добавлены аргументы `--correlation-data` и `--label` в группу команд `ams job`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1442">Added `--correlation-data` and `--label` arguments to `ams job` command group</span></span>
* <span data-ttu-id="8b368-1443">Добавлены аргументы `--storage-account` и `--container` в группу команд `ams asset`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1443">Added `--storage-account` and `--container` arguments to `ams asset` command group</span></span>
* <span data-ttu-id="8b368-1444">Добавлены значения по умолчанию для времени истечения срока действия (23 часа от текущего момента) и разрешений (чтение) в команду `ams asset get-sas-url`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1444">Added default values for expiry time (Now+23h) and permissions (Read) in `ams asset get-sas-url` command</span></span> 
* <span data-ttu-id="8b368-1445">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming locator` заменена на `ams streaming-locator`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1445">[BREAKING CHANGE] Replaced `ams streaming locator` command with `ams streaming-locator`</span></span>
* <span data-ttu-id="8b368-1446">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Обновлен аргумент `--content-keys` в `ams streaming locator`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1446">[BREAKING CHANGE] Updated `--content-keys` argument of `ams streaming locator`</span></span>
* <span data-ttu-id="8b368-1447">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--content-policy-name` команды `ams streaming locator` переименован в `--content-key-policy-name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1447">[BREAKING CHANGE] Renamed `--content-policy-name` to `--content-key-policy-name` in `ams streaming locator` command</span></span>
* <span data-ttu-id="8b368-1448">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `ams streaming policy` заменена на `ams streaming-policy`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1448">[BREAKING CHANGE] Replaced `ams streaming policy` command with `ams streaming-policy`</span></span>
* <span data-ttu-id="8b368-1449">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--preset-names` в группе команд `ams transform` заменен на `--preset`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1449">[BREAKING CHANGE] Replaced `--preset-names` argument with `--preset` in `ams transform` command group.</span></span> <span data-ttu-id="8b368-1450">Теперь можно одновременно задавать только один вывод/набор параметров (для добавления дополнительных нужно запустить команду `ams transform output add`).</span><span class="sxs-lookup"><span data-stu-id="8b368-1450">Now you can only set 1 output/preset at a time (to add more you have to run `ams transform output add`).</span></span> <span data-ttu-id="8b368-1451">Также можно задать пользовательский параметр StandardEncoderPreset, указав путь к пользовательскому файлу JSON.</span><span class="sxs-lookup"><span data-stu-id="8b368-1451">Also, you can set custom StandardEncoderPreset by passing the path to your custom JSON</span></span>
* <span data-ttu-id="8b368-1452">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Аргумент `--output-asset-names ` команды `ams job start` переименован в `--output-assets`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1452">[BREAKING CHANGE] Renamed `--output-asset-names ` to `--output-assets` in `ams job start` command.</span></span> <span data-ttu-id="8b368-1453">Теперь он принимает список ресурсов, разделенных пробелами, в формате assetName=label.</span><span class="sxs-lookup"><span data-stu-id="8b368-1453">Now it accepts a space-separated list of assets in 'assetName=label' format.</span></span> <span data-ttu-id="8b368-1454">Ресурс без метки можно передать следующим образом: assetName=.</span><span class="sxs-lookup"><span data-stu-id="8b368-1454">An asset without label can be sent like this: 'assetName='</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1455">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-1455">AppService</span></span>
* <span data-ttu-id="8b368-1456">Исправлена ошибка в `az webapp config backup update`, которая не давала установить расписание резервного копирования при наличии существующего расписания.</span><span class="sxs-lookup"><span data-stu-id="8b368-1456">Fixed a bug in `az webapp config backup update` that prevents setting a backup schedule if one is not already set</span></span>

### <a name="configure"></a><span data-ttu-id="8b368-1457">Configure</span><span class="sxs-lookup"><span data-stu-id="8b368-1457">Configure</span></span>
* <span data-ttu-id="8b368-1458">Добавлен YAML в список поддерживаемых форматов выходных данных.</span><span class="sxs-lookup"><span data-stu-id="8b368-1458">Added YAML to output format options</span></span>

### <a name="container"></a><span data-ttu-id="8b368-1459">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-1459">Container</span></span>
* <span data-ttu-id="8b368-1460">Внесено изменение для показа идентификатора при экспорте группы контейнеров в файл YAML.</span><span class="sxs-lookup"><span data-stu-id="8b368-1460">Changed to show identity when exporting a container group to yaml</span></span>

### <a name="eventhub"></a><span data-ttu-id="8b368-1461">концентратор событий.</span><span class="sxs-lookup"><span data-stu-id="8b368-1461">EventHub</span></span>
* <span data-ttu-id="8b368-1462">Добавлен флаг `--enable-kafka` для поддержки Kafka в `eventhub namespace [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1462">Added `--enable-kafka` flag to support Kafka in `eventhub namespace [create|update]`</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-1463">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-1463">Interactive</span></span>
* <span data-ttu-id="8b368-1464">Interactive теперь устанавливает расширение `interactive`, которое обеспечивает более быстрые обновления и поддержку.</span><span class="sxs-lookup"><span data-stu-id="8b368-1464">Interactive now installs the `interactive` extension, which will allow for faster updates and support</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-1465">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-1465">Monitor</span></span>
* <span data-ttu-id="8b368-1466">Добавлена поддержка имен метрик, которые включают символы прямой косой черты (/) и точки (.), в параметр `--condition` команды `monitor metrics alert [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1466">Added support for metric names  which include characters forward-slash (/) and period (.) to `--condition` in `monitor metrics alert [create|update]`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1467">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1467">Network</span></span>
* <span data-ttu-id="8b368-1468">Имена команд `network interface-endpoint` не рекомендуются к использованию. Вместо них следует использовать `network private-endpoint`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1468">Deprecated `network interface-endpoint` command names in favor of `network private-endpoint`</span></span>
* <span data-ttu-id="8b368-1469">Исправлена ошибка, при которой аргумент `--peer-circuit` в `express-route peering connection create` не принимал идентификатор.</span><span class="sxs-lookup"><span data-stu-id="8b368-1469">Fixed issue with where `--peer-circuit` argument in `express-route peering connection create`would not accept an ID</span></span>
* <span data-ttu-id="8b368-1470">Исправлена ошибка, приводившая к неправильной работе аргумента `--ip-tags` в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1470">Fixed issue where `--ip-tags` did not work correctly with `public-ip create`</span></span> 

### <a name="profile"></a><span data-ttu-id="8b368-1471">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-1471">Profile</span></span>
* <span data-ttu-id="8b368-1472">Добавлен аргумент `--use-cert-sn-issuer` в команду `az login` для входа субъекта-службы с автоматической ротацией сертификатов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1472">Added `--use-cert-sn-issuer` to `az login` for service principal login with cert auto-rolls</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-1473">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="8b368-1473">RDBMS</span></span>
* <span data-ttu-id="8b368-1474">Добавлены команды для работы с репликами MySQL.</span><span class="sxs-lookup"><span data-stu-id="8b368-1474">Added mysql replica commands</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-1475">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-1475">Resource</span></span>
* <span data-ttu-id="8b368-1476">Добавлена поддержка групп управления и подписок в команды `policy definition|set-definition`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1476">Added support for management groups and subscriptions to `policy definition|set-definition` commands</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1477">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1477">Role</span></span>
* <span data-ttu-id="8b368-1478">Добавлена поддержка управления разрешениями API, входа пользователя, а также управления паролями и сертификатами приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-1478">Added support for API permission management, signed-in-user, and application password & certificate credential management</span></span>
* <span data-ttu-id="8b368-1479">Изменена команда `ad sp create-for-rbac`, чтобы устранить путаницу между параметром displayName и именем субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-1479">Changed `ad sp create-for-rbac` to clarify the confusion between displayName and service principal name</span></span>
* <span data-ttu-id="8b368-1480">Добавлена поддержка назначения разрешения для приложений AAD.</span><span class="sxs-lookup"><span data-stu-id="8b368-1480">Added support to grant permissions to AAD apps</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1481">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1481">Storage</span></span>
* <span data-ttu-id="8b368-1482">Добавлена поддержка подключения к службам хранения с использованием только подписанных URL-адресов и конечных точек (без имени или ключа учетной записи), как описано в `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1482">Added support to connect to storage services only with SAS and endpoints (without an account name or a key) as described in `Configure Azure Storage connection strings <https://docs.microsoft.com/azure/storage/common/storage-configure-connection-string>`</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1483">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1483">VM</span></span>
* <span data-ttu-id="8b368-1484">Добавлен аргумент `storage-sku` в команду `image create`, позволяющий указать тип учетной записи хранения по умолчанию для образа.</span><span class="sxs-lookup"><span data-stu-id="8b368-1484">Added `storage-sku` argument to `image create` for setting the image's default storage account type</span></span>
* <span data-ttu-id="8b368-1485">Исправлена ошибка в команде `vm resize`, из-за которой использование параметра `--no-wait` приводило к аварийному завершению команды.</span><span class="sxs-lookup"><span data-stu-id="8b368-1485">Fixed bug with `vm resize` where `--no-wait` option causes command to crash</span></span>
* <span data-ttu-id="8b368-1486">Изменен формат выходных данных команды `vm encryption show` в виде таблицы для отображения состояния.</span><span class="sxs-lookup"><span data-stu-id="8b368-1486">Changed `vm encryption show` table output format to show status</span></span>
* <span data-ttu-id="8b368-1487">Изменена команда `vm secret format`, которая теперь требует выходных данных в формате JSON/JSONC.</span><span class="sxs-lookup"><span data-stu-id="8b368-1487">Changed `vm secret format` to require json/jsonc output.</span></span> <span data-ttu-id="8b368-1488">Команда выводит предупреждение и по умолчанию использует для выходных данных формат JSON, если выбран нежелательный формат выходных данных.</span><span class="sxs-lookup"><span data-stu-id="8b368-1488">Warns user and defaults to json output if an undesired output format is selected</span></span>
* <span data-ttu-id="8b368-1489">Улучшена проверка аргументов команды `vm create --image`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1489">Improved argument validation for `vm create --image`</span></span>

## <a name="october-23-2018"></a><span data-ttu-id="8b368-1490">23 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1490">October 23, 2018</span></span>

<span data-ttu-id="8b368-1491">Версия 2.0.49</span><span class="sxs-lookup"><span data-stu-id="8b368-1491">Version 2.0.49</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1492">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1492">Core</span></span>
* <span data-ttu-id="8b368-1493">Исправлена проблема с аргументом `--ids`, из-за которой аргумент `--subscription` имел приоритет над подпиской, указанной с использованием `--ids`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1493">Fixed issue with `--ids` where `--subscription` would take precedence over the subscription in `--ids`</span></span>
* <span data-ttu-id="8b368-1494">Добавлены явные предупреждения о том, что параметры будут игнорироваться при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1494">Added explicit warnings when parameters would be ignored by use of `--ids`</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1495">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1495">ACR</span></span>
* <span data-ttu-id="8b368-1496">Исправлена ошибка, связанная с шифрованием сборки ACR в Python2.</span><span class="sxs-lookup"><span data-stu-id="8b368-1496">Fixed an ACR Build encoding issue in Python2</span></span>

### <a name="cdn"></a><span data-ttu-id="8b368-1497">CDN</span><span class="sxs-lookup"><span data-stu-id="8b368-1497">CDN</span></span>
* <span data-ttu-id="8b368-1498">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменено стандартное поведение при кешировании строки запроса `cdn endpoint create`. Теперь IgnoreQueryString не является значением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1498">[BREAKING CHANGE] Changed `cdn endpoint create`'s default query string caching behaviour to no longer defaults to "IgnoreQueryString".</span></span> <span data-ttu-id="8b368-1499">Это значение задает служба.</span><span class="sxs-lookup"><span data-stu-id="8b368-1499">It is now set by the service</span></span>

### <a name="container"></a><span data-ttu-id="8b368-1500">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-1500">Container</span></span>
* <span data-ttu-id="8b368-1501">Добавлен тип `Private` в качестве допустимого типа для передачи в --ip-address.</span><span class="sxs-lookup"><span data-stu-id="8b368-1501">Added `Private` as a valid type to pass to '--ip-address'</span></span>
* <span data-ttu-id="8b368-1502">При настройке подсети для группы контейнеров разрешено использовать только идентификатор подсети.</span><span class="sxs-lookup"><span data-stu-id="8b368-1502">Changed to allow using only subnet ID to setup a virtual network for the container group</span></span>
* <span data-ttu-id="8b368-1503">Разрешено указывать имя виртуальной сети или идентификатор ресурса для использования виртуальных сетей из разных групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1503">Changed to allow using vnet name or resource id to enable using vnets from different resource groups</span></span>
* <span data-ttu-id="8b368-1504">Добавлен параметр `--assign-identity`, позволяющий добавить удостоверение MSI для группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-1504">Added `--assign-identity` for adding a MSI identity to a container group</span></span>
* <span data-ttu-id="8b368-1505">Добавлен параметр `--scope`, позволяющий создать назначение ролей для удостоверения MSI, назначаемого системой.</span><span class="sxs-lookup"><span data-stu-id="8b368-1505">Added `--scope` to create a role assignment for the system assigned MSI identity</span></span>
* <span data-ttu-id="8b368-1506">Добавлено предупреждение, которое появляется при создании группы контейнеров с помощью образа без использования длительного процесса.</span><span class="sxs-lookup"><span data-stu-id="8b368-1506">Added a warning when creating a container group with an image without a long running process</span></span>
* <span data-ttu-id="8b368-1507">Исправлены ошибки, связанные с табличными выходными данными для команд `list` и `show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1507">Fixed table output issues for `list` and `show` commands</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8b368-1508">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-1508">CosmosDB</span></span>
* <span data-ttu-id="8b368-1509">В команду `cosmosdb create` добавлена поддержка параметра `--enable-multiple-write-locations`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1509">Added `--enable-multiple-write-locations` support to `cosmosdb create`</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-1510">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-1510">Interactive</span></span>
* <span data-ttu-id="8b368-1511">Внесены изменения, которые обеспечивают отображение параметра глобальных подписок в списке параметров.</span><span class="sxs-lookup"><span data-stu-id="8b368-1511">Changed to ensure global subscription parameter appears in parameters</span></span>

### <a name="iot-central"></a><span data-ttu-id="8b368-1512">IoT Central</span><span class="sxs-lookup"><span data-stu-id="8b368-1512">IoT Central</span></span>
* <span data-ttu-id="8b368-1513">Добавлены параметры для шаблона и отображаемого имени, используемые при создании приложения IoT Central.</span><span class="sxs-lookup"><span data-stu-id="8b368-1513">Added template and display name options for IoT Central Application creation</span></span>
* <span data-ttu-id="8b368-1514">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена поддержка номера SKU F1. Вместо него используйте S1.</span><span class="sxs-lookup"><span data-stu-id="8b368-1514">[BREAKING CHANGE] Removed support for the F1 SKU; Use S1 SKU instead</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-1515">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-1515">Monitor</span></span>
* <span data-ttu-id="8b368-1516">Изменения в `monitor activity-log list`:</span><span class="sxs-lookup"><span data-stu-id="8b368-1516">Changes to `monitor activity-log list`:</span></span>
  * <span data-ttu-id="8b368-1517">Добавлена поддержка для вывода списка всех событий на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="8b368-1517">Added support for listing all events at the subscription level</span></span>
  * <span data-ttu-id="8b368-1518">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="8b368-1518">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="8b368-1519">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="8b368-1519">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
  * <span data-ttu-id="8b368-1520">Добавлен параметр `--namespace` в качестве псевдонима для нерекомендуемого параметра `--resource-provider`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1520">Added `--namespace` as alias for deprecated option `--resource-provider`</span></span>
  * <span data-ttu-id="8b368-1521">Параметр `--filters` отмечен как нерекомендуемый, так как служба не поддерживает значения, отличные от значений со строгой типизацией.</span><span class="sxs-lookup"><span data-stu-id="8b368-1521">Deprecated `--filters` because no values other than those with strongly-typed options are supported by the service</span></span>
* <span data-ttu-id="8b368-1522">Изменения в `monitor metrics list`:</span><span class="sxs-lookup"><span data-stu-id="8b368-1522">Changes to `monitor metrics list`:</span></span>
  * <span data-ttu-id="8b368-1523">Добавлен параметр `--offset`, чтобы упростить создание запросов времени.</span><span class="sxs-lookup"><span data-stu-id="8b368-1523">Added `--offset` parameter to more easily create time queries</span></span>
  * <span data-ttu-id="8b368-1524">Улучшена проверка для `--start-time` и `--end-time`, что позволяет применять широкий диапазон форматов ISO 8601 и более понятные форматы даты и времени.</span><span class="sxs-lookup"><span data-stu-id="8b368-1524">Improved validation for `--start-time` and `--end-time` to use wider range of ISO8601 formats and more user-friendly datetime formats</span></span>
* <span data-ttu-id="8b368-1525">Улучшена проверка аргументов `--event-hub` и `--event-hub-rule` для `monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1525">Improved validation for `--event-hub` and `--event-hub-rule` arguments to `monitor diagnostic-settings create`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1526">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1526">Network</span></span>
* <span data-ttu-id="8b368-1527">Для `nic create` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="8b368-1527">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic create`, to support adding application gateway backend address pools to a NIC</span></span>
* <span data-ttu-id="8b368-1528">Для `nic ip-config create/update` добавлены аргументы `--app-gateway-address-pools` и `--gateway-name`, которые позволяют добавить внутренний пул адресов Шлюза приложений для сетевого адаптера.</span><span class="sxs-lookup"><span data-stu-id="8b368-1528">Added `--app-gateway-address-pools` and `--gateway-name` arguments to `nic ip-config create/update`, to support adding application gateway backend address pools to a NIC</span></span>

### <a name="servicebus"></a><span data-ttu-id="8b368-1529">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="8b368-1529">ServiceBus</span></span>
* <span data-ttu-id="8b368-1530">В класс MigrationConfigProperties добавлено свойство `migration_state` с доступом только для чтения. Это свойство позволяет получить сведения о текущем состоянии миграции с ценовой категории Служебной шины "Стандартный" на ценовую категорию "Премиум".</span><span class="sxs-lookup"><span data-stu-id="8b368-1530">Added Read-Only `migration_state` to MigrationConfigProperties to show current Service Bus Standard to Premium namespace migration state</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-1531">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-1531">SQL</span></span>
* <span data-ttu-id="8b368-1532">Исправлены `sql failover-group create` и `sql failover-group update` для работы с политикой перехода на другой ресурс вручную.</span><span class="sxs-lookup"><span data-stu-id="8b368-1532">Fixed `sql failover-group create` and `sql failover-group update` to work with Manual failover policy</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1533">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1533">Storage</span></span>
* <span data-ttu-id="8b368-1534">Исправлен формат выходных данных `az storage cors list`: для всех элементов отображается правильный ключ службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-1534">Fixed `az storage cors list` output formatting, all items show correct "Service" key</span></span>
* <span data-ttu-id="8b368-1535">Добавлен параметр `--bypass-immutability-policy`, который позволяет удалить контейнер, блокируемый политикой неизменяемости.</span><span class="sxs-lookup"><span data-stu-id="8b368-1535">Added `--bypass-immutability-policy` parameter for immutability-policy blocked container deletion</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1536">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1536">VM</span></span>
* <span data-ttu-id="8b368-1537">Для режима кэширования диска принудительно применяется значение `None` при использовании команды `[vm|vmss] create` для виртуальных машин серии Lv или Lv2.</span><span class="sxs-lookup"><span data-stu-id="8b368-1537">Enforce disk caching mode be `None` for Lv/Lv2 series of machines in `[vm|vmss] create`</span></span>
* <span data-ttu-id="8b368-1538">Для `vm create` обновлен список поддерживаемых размеров для поддерживаемого сетевого ускорителя.</span><span class="sxs-lookup"><span data-stu-id="8b368-1538">Updated supported size list supporting networking accelerator for `vm create`</span></span>
* <span data-ttu-id="8b368-1539">Для `disk create` добавлены строго типизированные аргументы, которые позволяют настроить скорость операций ввода-вывода и передачи данных в секунду для дисков SSD ценовой категории "Ультра".</span><span class="sxs-lookup"><span data-stu-id="8b368-1539">Added strong typed arguments for ultrassd iops and mbps configs for `disk create`</span></span>

## <a name="october-16-2018"></a><span data-ttu-id="8b368-1540">16 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1540">October 16, 2018</span></span>

<span data-ttu-id="8b368-1541">Версия 2.0.48</span><span class="sxs-lookup"><span data-stu-id="8b368-1541">Version 2.0.48</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1542">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1542">VM</span></span>
* <span data-ttu-id="8b368-1543">Исправлена проблема с пакетом SDK, из-за которой установка Homebrew завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="8b368-1543">Fixed SDK issue that caused Homebrew instllation to fail</span></span>

## <a name="october-9-2018"></a><span data-ttu-id="8b368-1544">9 октября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1544">October 9, 2018</span></span>

<span data-ttu-id="8b368-1545">Версия 2.0.47</span><span class="sxs-lookup"><span data-stu-id="8b368-1545">Version 2.0.47</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1546">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1546">Core</span></span>
* <span data-ttu-id="8b368-1547">Улучшена обработка ошибок типа Bad Request (Недопустимый запрос).</span><span class="sxs-lookup"><span data-stu-id="8b368-1547">Improved error handling for "Bad Request" errors</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1548">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1548">ACR</span></span>
* <span data-ttu-id="8b368-1549">Добавлена поддержка табличного формата, как в клиенте Helm.</span><span class="sxs-lookup"><span data-stu-id="8b368-1549">Added support for similar table format as helm client</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1550">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1550">ACS</span></span>
* <span data-ttu-id="8b368-1551">Добавлен параметр `aks [create|scale] --nodepool-name` для настройки имени пула узлов. Длина имени ограничена 12 символами. Имя по умолчанию — nodepool1.</span><span class="sxs-lookup"><span data-stu-id="8b368-1551">Added `aks [create|scale] --nodepool-name` to configure nodepool name, truncated to 12 characters, default - nodepool1</span></span> 
* <span data-ttu-id="8b368-1552">Исправлен возврат к scp при сбое Paramiko.</span><span class="sxs-lookup"><span data-stu-id="8b368-1552">Fixed to fall back to 'scp' when Parimiko fails</span></span>
* <span data-ttu-id="8b368-1553">Изменена команда `aks create`, которая больше не требует `--aad-tenant-id`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1553">Changed `aks create` to no longer require `--aad-tenant-id`</span></span>
* <span data-ttu-id="8b368-1554">Улучшена функция слияния учетных данных Kubernetes при наличии дублированных записей.</span><span class="sxs-lookup"><span data-stu-id="8b368-1554">Improved merging of Kubernetes credentials when duplicate entries are present</span></span>

### <a name="container"></a><span data-ttu-id="8b368-1555">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-1555">Container</span></span>
* <span data-ttu-id="8b368-1556">Изменена команда `functionapp create`, которая теперь поддерживает создание типа для плана потребления Linux с конкретной средой выполнения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1556">Changed `functionapp create` to support creating a Linux consumption plan type with a specific runtime</span></span>
* <span data-ttu-id="8b368-1557">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для размещения веб-приложений в контейнерах Windows.</span><span class="sxs-lookup"><span data-stu-id="8b368-1557">[PREVIEW] Added support for hosting webapps on Windows containers</span></span>

### <a name="event-hub"></a><span data-ttu-id="8b368-1558">Концентратор событий</span><span class="sxs-lookup"><span data-stu-id="8b368-1558">Event Hub</span></span>
* <span data-ttu-id="8b368-1559">Исправлена команда `eventhub update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1559">Fixed `eventhub update` command</span></span>
* <span data-ttu-id="8b368-1560">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="8b368-1560">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="extensions"></a><span data-ttu-id="8b368-1561">Модули</span><span class="sxs-lookup"><span data-stu-id="8b368-1561">Extensions</span></span>
* <span data-ttu-id="8b368-1562">Исправлена проблема при попытке добавить расширение, которое уже установлено.</span><span class="sxs-lookup"><span data-stu-id="8b368-1562">Fixed issue with attempting to add an extension that is already installed</span></span>

### <a name="hdinsight"></a><span data-ttu-id="8b368-1563">HDInsight</span><span class="sxs-lookup"><span data-stu-id="8b368-1563">HDInsight</span></span>
* <span data-ttu-id="8b368-1564">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="8b368-1564">Initial release</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-1565">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-1565">IoT</span></span>
* <span data-ttu-id="8b368-1566">На баннер, отображаемый при первом запуске, добавлена команда для установки расширений.</span><span class="sxs-lookup"><span data-stu-id="8b368-1566">Added extension installation comand to first-run banner</span></span>

### <a name="keyvault"></a><span data-ttu-id="8b368-1567">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8b368-1567">KeyVault</span></span>
* <span data-ttu-id="8b368-1568">Изменены команды для работы с хранилищем ключей.Теперь они ограничены последним профилем API.</span><span class="sxs-lookup"><span data-stu-id="8b368-1568">Changed to restrict keyvault storage commmands to the latest API profile</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1569">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1569">Network</span></span>
* <span data-ttu-id="8b368-1570">Исправлена команда `network dns zone create`. Теперь команда выполняется успешно, даже если пользователь настроил расположение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1570">Fixed `network dns zone create`: Command succeeds even if the user has configured a default location.</span></span> <span data-ttu-id="8b368-1571">См. № 6052.</span><span class="sxs-lookup"><span data-stu-id="8b368-1571">See #6052</span></span>
* <span data-ttu-id="8b368-1572">`--remote-vnet-id` не рекомендуется к использованию для `network vnet peering create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1572">Deprecated `--remote-vnet-id` for `network vnet peering create`</span></span>
* <span data-ttu-id="8b368-1573">Добавлена параметр `--remote-vnet` в команду `network vnet peering create`, который принимает имя или идентификатор.</span><span class="sxs-lookup"><span data-stu-id="8b368-1573">Added `--remote-vnet` to `network vnet peering create` which accepts a name or ID</span></span>
* <span data-ttu-id="8b368-1574">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet create` с параметром `--subnet-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1574">Added support for multiple subnet prefixes to `network vnet create` with `--subnet-prefixes`</span></span>
* <span data-ttu-id="8b368-1575">Добавлена поддержка нескольких префиксов подсетей в команде `network vnet subnet [create|update]` с параметром `--address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1575">Added support for multiple subnet prefixes to `network vnet subnet [create|update]` with `--address-prefixes`</span></span>
* <span data-ttu-id="8b368-1576">Исправлена ошибка в команде `network application-gateway create`, из-за которой было невозможно создать шлюзы с номером SKU `WAF_v2` или `Standard_v2`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1576">Fixed issue with `network application-gateway create` that prevented creating gateways with `WAF_v2` or `Standard_v2` SKU</span></span>
* <span data-ttu-id="8b368-1577">Добавлен вспомогательный аргумент `--service-endpoint-policy` в команду `network vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1577">Added `--service-endpoint-policy` convenience argument to `network vnet subnet update`</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1578">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1578">Role</span></span>
* <span data-ttu-id="8b368-1579">Добавлена поддержка для списка владельцев приложения Azure AD в команду `ad app owner`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1579">Added support for listing Azure AD app owners to `ad app owner`</span></span>
* <span data-ttu-id="8b368-1580">Добавлена поддержка для списка владельцев субъекта-службы Azure AD в команду `ad sp owner`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1580">Added support for listing Azure AD service principal owners to `ad sp owner`</span></span>
* <span data-ttu-id="8b368-1581">Изменены команды для создания и обновления определений ролей, которые теперь принимают несколько конфигураций разрешений.</span><span class="sxs-lookup"><span data-stu-id="8b368-1581">Changed to ensure role definition create & update commands accept multiple permission configurations</span></span>
* <span data-ttu-id="8b368-1582">Изменена команда `ad sp create-for-rbac`, чтобы универсальный код ресурса (URI) для домашней страницы всегда начинался с https.</span><span class="sxs-lookup"><span data-stu-id="8b368-1582">Changed `ad sp create-for-rbac` to ensure home page URI is always "https"</span></span>

### <a name="service-bus"></a><span data-ttu-id="8b368-1583">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="8b368-1583">Service Bus</span></span>
* <span data-ttu-id="8b368-1584">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды `list` для обработки ошибок NotFound (404) от ресурсов. Теперь ошибки обрабатываются обычным образом вместо отображения пустого списка.</span><span class="sxs-lookup"><span data-stu-id="8b368-1584">[BREAKING CHANGE] Changed `list` commands to handle errors for resource(s) NotFound(404) in the typical way instead of showing empty list</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1585">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1585">VM</span></span>
* <span data-ttu-id="8b368-1586">Исправлено пустое поле `accessSas` в `disk grant-access`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1586">Fixed empty `accessSas` field in `disk grant-access`</span></span>
* <span data-ttu-id="8b368-1587">Изменена команда `vmss create`, которая теперь резервирует достаточно большой диапазон внешних портов для обработки избыточной подготовки.</span><span class="sxs-lookup"><span data-stu-id="8b368-1587">Changed `vmss create` to reserve large enough frontend port range to handle overprovisioning</span></span>
* <span data-ttu-id="8b368-1588">Исправлены команды обновления для `sig`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1588">Fixed update commands for `sig`</span></span>
* <span data-ttu-id="8b368-1589">Добавлена поддержка `--no-wait` для управления версиями образов в `sig`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1589">Added `--no-wait` support for managing image versions in `sig`</span></span>
* <span data-ttu-id="8b368-1590">Изменена команда `vm list-ip-addresses` для отображения зоны доступности общедоступного IP-адреса.</span><span class="sxs-lookup"><span data-stu-id="8b368-1590">Changed `vm list-ip-addresses` to show availability zone of public IP addresses</span></span>
* <span data-ttu-id="8b368-1591">Изменена команда `[vm|vmss] disk attach`, которая теперь по умолчанию устанавливает для логического номера диска первое доступно значение.</span><span class="sxs-lookup"><span data-stu-id="8b368-1591">Changed `[vm|vmss] disk attach` to set disk's default lun to the first available spot</span></span>

## <a name="september-21-2018"></a><span data-ttu-id="8b368-1592">21 сентября 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1592">September 21, 2018</span></span>

<span data-ttu-id="8b368-1593">Версия 2.0.46</span><span class="sxs-lookup"><span data-stu-id="8b368-1593">Version 2.0.46</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1594">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1594">ACR</span></span>
* <span data-ttu-id="8b368-1595">Добавлены команды задач ACR.</span><span class="sxs-lookup"><span data-stu-id="8b368-1595">Added ACR Task commands</span></span>
* <span data-ttu-id="8b368-1596">Добавлена команда быстрого запуска.</span><span class="sxs-lookup"><span data-stu-id="8b368-1596">Added quick run command</span></span>
* <span data-ttu-id="8b368-1597">Группа команд `build-task` не рекомендуется к использованию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1597">Deprecated `build-task` command group</span></span>
* <span data-ttu-id="8b368-1598">Добавлена группа команд `helm` для поддержки управления чартами Helm в ACR.</span><span class="sxs-lookup"><span data-stu-id="8b368-1598">Added `helm` command group to support managing helm charts with ACR</span></span>
* <span data-ttu-id="8b368-1599">Добавлена поддержка создания идемпотентных элементов для управляемого реестра.</span><span class="sxs-lookup"><span data-stu-id="8b368-1599">Added support for idempotent create for managed registry</span></span>
* <span data-ttu-id="8b368-1600">Добавлен флаг отсутствия форматирования для отображения журналов сборки.</span><span class="sxs-lookup"><span data-stu-id="8b368-1600">Added a no-format flag for displaying build logs</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1601">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1601">ACS</span></span>
* <span data-ttu-id="8b368-1602">Изменена команда `install-connector` для указания главного полного доменного имени в AKS.</span><span class="sxs-lookup"><span data-stu-id="8b368-1602">Changed the `install-connector` command to set the AKS Master FQDN</span></span>
* <span data-ttu-id="8b368-1603">Исправлена ошибка при назначении ролей для идентификатора подсети виртуальной сети, если не указан субъект-служба и пропущен шаг назначения ролей.</span><span class="sxs-lookup"><span data-stu-id="8b368-1603">Fixed creating role assignment for vnet-subnet-id when not specifying service principal and skip-role-assignemnt</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1604">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-1604">AppService</span></span>

* <span data-ttu-id="8b368-1605">Добавлена поддержка операций управления веб-заданиями (как непрерывных, так и активируемых).</span><span class="sxs-lookup"><span data-stu-id="8b368-1605">Added support for webjobs (continuous and triggered) operations management</span></span>
* <span data-ttu-id="8b368-1606">Добавлена поддержка свойства fts-state в az webapp config set. Также добавлена поддержка команд az functionapp config set и az functionapp config show.</span><span class="sxs-lookup"><span data-stu-id="8b368-1606">az webapp config set supports --fts-state propertyAlso added support fot az functionapp config set & show</span></span>
* <span data-ttu-id="8b368-1607">Добавлена возможность использования собственного хранилища для веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-1607">Added support for bring your own storage for webapps</span></span>
* <span data-ttu-id="8b368-1608">Добавлена возможность вывода списка удаленных веб-приложений и их восстановления.</span><span class="sxs-lookup"><span data-stu-id="8b368-1608">Added support for listing and restoring deleted webapps</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-1609">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-1609">Batch</span></span>
* <span data-ttu-id="8b368-1610">Изменена функция добавления задач с помощью `--json-file` для поддержки синтаксиса AddTaskCollectionParameter.</span><span class="sxs-lookup"><span data-stu-id="8b368-1610">Changed adding tasks through `--json-file` to support AddTaskCollectionParameter syntax</span></span>
* <span data-ttu-id="8b368-1611">Обновлена документация в принятом формате `--json-file`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1611">Updated documentation of accepted `--json-file` formats</span></span>
* <span data-ttu-id="8b368-1612">Добавлен параметр `--max-tasks-per-node-option` для команды `batch pool create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1612">Added `--max-tasks-per-node-option` to `batch pool create`</span></span>
* <span data-ttu-id="8b368-1613">Изменен режим работы `batch account` на отображение учетной записи, в которую выполнен вход, если не заданы другие параметры.</span><span class="sxs-lookup"><span data-stu-id="8b368-1613">Changed behavior of `batch account` to show currently logged in account if no options are specified</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8b368-1614">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8b368-1614">Batch AI</span></span> 
* <span data-ttu-id="8b368-1615">Исправлен сбой при автоматическом создании учетной записи хранения при выполнении команды `batchai cluster create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1615">Fixed auto storage account creation failure in `batchai cluster create` command</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8b368-1616">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="8b368-1616">Cognitive Services</span></span>
* <span data-ttu-id="8b368-1617">Добавлено средство заполнения для аргументов `--sku`, `--kind` и `--location`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1617">Added completer for  `--sku`, `--kind`, `--location` arguments</span></span>
* <span data-ttu-id="8b368-1618">Добавлена команда `cognitiveservices account list-usage`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1618">Added command `cognitiveservices account list-usage`</span></span>
* <span data-ttu-id="8b368-1619">Добавлена команда `cognitiveservices account list-kinds`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1619">Added command `cognitiveservices account list-kinds`</span></span>
* <span data-ttu-id="8b368-1620">Добавлена команда `cognitiveservices account list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1620">Added command `cognitiveservices account list`</span></span>
* <span data-ttu-id="8b368-1621">Команда `cognitiveservices list` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="8b368-1621">Deprecated `cognitiveservices list`</span></span>
* <span data-ttu-id="8b368-1622">Изменен параметр `--name`, который теперь является необязательным для `cognitiveservices account list-skus`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1622">Changed `--name` to be optional for `cognitiveservices account list-skus`</span></span>

### <a name="container"></a><span data-ttu-id="8b368-1623">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-1623">Container</span></span>
* <span data-ttu-id="8b368-1624">Добавлена возможность перезапуска и остановки выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-1624">Added ability to restart and stop a running container group</span></span>
* <span data-ttu-id="8b368-1625">Добавлен параметр `--network-profile` для передачи в сетевой профиль.</span><span class="sxs-lookup"><span data-stu-id="8b368-1625">Added `--network-profile` for passing in a network profile</span></span>
* <span data-ttu-id="8b368-1626">Добавлены параметры `--subnet` и `--vnet_name` для создания групп контейнеров в виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="8b368-1626">Added `--subnet`, `--vnet_name`, to allow creating container groups in a VNET</span></span>
* <span data-ttu-id="8b368-1627">Изменены табличные выходные данные для отображения состояния группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-1627">Changed table output to show the status of the container group</span></span>

### <a name="datalake"></a><span data-ttu-id="8b368-1628">Data Lake</span><span class="sxs-lookup"><span data-stu-id="8b368-1628">Datalake</span></span>
* <span data-ttu-id="8b368-1629">Добавлены команды для правил виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="8b368-1629">Added commands for virtual network rules</span></span>

### <a name="interactive-shell"></a><span data-ttu-id="8b368-1630">Интерактивная оболочка</span><span class="sxs-lookup"><span data-stu-id="8b368-1630">Interactive Shell</span></span>
* <span data-ttu-id="8b368-1631">Исправлена ошибка в Windows, связанная со сбоем при выполнении команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-1631">Fixed error on Windows where commands fail to run properly</span></span>
* <span data-ttu-id="8b368-1632">Исправлена проблема с загрузкой команд в интерактивной оболочке из-за использования нерекомендуемых объектов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1632">Fixed command loading problem in interactive that was caused by deprecated objects</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-1633">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-1633">IoT</span></span>
* <span data-ttu-id="8b368-1634">Добавлена поддержка маршрутизации Центров Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="8b368-1634">Added support for routing IoT Hubs</span></span>

### <a name="key-vault"></a><span data-ttu-id="8b368-1635">Key Vault</span><span class="sxs-lookup"><span data-stu-id="8b368-1635">Key Vault</span></span>
* <span data-ttu-id="8b368-1636">Исправлена ошибка импорта ключа в Key Vault для ключей RSA.</span><span class="sxs-lookup"><span data-stu-id="8b368-1636">Fixed Key Vault key import for RSA keys</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1637">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1637">Network</span></span>
* <span data-ttu-id="8b368-1638">Добавлены команды `network public-ip prefix` для поддержки операций с префиксами общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1638">Add `network public-ip prefix` commands to support public IP prefixes features</span></span>
* <span data-ttu-id="8b368-1639">Добавлены команды `network service-endpoint` для поддержки операций с политиками конечной точки службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-1639">Add `network service-endpoint` commands to support service endpoint policy features</span></span>
* <span data-ttu-id="8b368-1640">Добавлены команды `network lb outbound-rule` для поддержки создания правил для исходящего трафика в Load Balancer (цен. категория "Стандартный").</span><span class="sxs-lookup"><span data-stu-id="8b368-1640">Add `network lb outbound-rule` commands to support creation of Standard Load Balancer outbound rules</span></span>
* <span data-ttu-id="8b368-1641">Добавлен параметр `--public-ip-prefix` для `network lb frontend-ip create/update` для поддержки конфигурации IP внешнего интерфейса с помощью префиксов общедоступных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1641">Add `--public-ip-prefix` to `network lb frontend-ip create/update` to support frontend IP configurations using public IP prefixes</span></span>
* <span data-ttu-id="8b368-1642">Добавлен параметр `--enable-tcp-reset` для `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1642">Add `--enable-tcp-reset` to `network lb rule/inbound-nat-rule/inbound-nat-pool create/update`</span></span>
* <span data-ttu-id="8b368-1643">Добавлен параметр `--disable-outbound-snat` для `network lb rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1643">Add `--disable-outbound-snat` to `network lb rule create/update`</span></span>
* <span data-ttu-id="8b368-1644">Добавлена возможность использования `network watcher flow-log show/configure` с классическими группами безопасности сети.</span><span class="sxs-lookup"><span data-stu-id="8b368-1644">Allow `network watcher flow-log show/configure` to be used with classic NSGs</span></span>
* <span data-ttu-id="8b368-1645">Добавлена команда `network watcher run-configuration-diagnostic`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1645">Add `network watcher run-configuration-diagnostic` command</span></span>
* <span data-ttu-id="8b368-1646">Исправлена команда `network watcher test-connectivity` и добавлены свойства `--method`, `--valid-status-codes` и `--headers`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1646">Fix `network watcher test-connectivity` command and add `--method`, `--valid-status-codes` and `--headers` properties</span></span>
* <span data-ttu-id="8b368-1647">`network express-route create/update`: добавлен флаг `--allow-global-reach`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1647">`network express-route create/update`: Add `--allow-global-reach` flag</span></span>
* <span data-ttu-id="8b368-1648">`network vnet subnet create/update`: добавлена поддержка `--delegation`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1648">`network vnet subnet create/update`: Add support for `--delegation`</span></span>
* <span data-ttu-id="8b368-1649">Добавлена команда `network vnet subnet list-available-delegations`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1649">Added `network vnet subnet list-available-delegations` command</span></span>
* <span data-ttu-id="8b368-1650">`network traffic-manager profile create/update`: добавлена поддержка `--interval`, `--timeout` и `--max-failures` для конфигурации мониторинга. Не рекомендуются к использованию параметры `--monitor-path`, `--monitor-port` и `--monitor-protocol`, которые следует заменить на `--path`, `--port` и `--protocol`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1650">`network traffic-manager profile create/update`: Added support for `--interval`, `--timeout` and `--max-failures` for Monitor configuration Deprecated options `--monitor-path`, `--monitor-port` and `--monitor-protocol` in favor of `--path`, `--port`, `--protocol`</span></span>
* <span data-ttu-id="8b368-1651">`network lb frontend-ip create/update`: исправлена логика указания метода распределения частных IP-адресов. Если назначается частный IP-адрес, он назначается статически. Если частный IP-адрес не назначается или строка с данными о частных IP-адресах не заполнена, происходит динамическое распределение.</span><span class="sxs-lookup"><span data-stu-id="8b368-1651">`network lb frontend-ip create/update`: Fixed the logic for setting private IP allocation methodIf a private IP address is provided, the allocation will be staticIf no private IP address is provided, or empty string is provided for private IP address, allocation is dynamic.</span></span>
* <span data-ttu-id="8b368-1652">`dns record-set * create/update`: добавлена поддержка `--target-resource`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1652">`dns record-set * create/update`: Add support for `--target-resource`</span></span>
* <span data-ttu-id="8b368-1653">Добавлены команды `network interface-endpoint` для обращения к объектам конечных точек интерфейса.</span><span class="sxs-lookup"><span data-stu-id="8b368-1653">Add `network interface-endpoint` commands to query interface endpoint objects</span></span>
* <span data-ttu-id="8b368-1654">Добавлено `network profile show/list/delete` для частичного управления сетевыми профилями.</span><span class="sxs-lookup"><span data-stu-id="8b368-1654">Add `network profile show/list/delete` for partial management of network profiles</span></span>
* <span data-ttu-id="8b368-1655">Добавлено `network express-route peering connection` для управления пиринговыми подключениями через ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="8b368-1655">Add `network express-route peering connection` commands to manage peering connections between ExpressRoutes</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-1656">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="8b368-1656">RDBMS</span></span>
* <span data-ttu-id="8b368-1657">Добавлена поддержка MariaDB.</span><span class="sxs-lookup"><span data-stu-id="8b368-1657">Added support for MariaDB service</span></span>

### <a name="reservation"></a><span data-ttu-id="8b368-1658">резервирование.</span><span class="sxs-lookup"><span data-stu-id="8b368-1658">Reservation</span></span>
* <span data-ttu-id="8b368-1659">База данных CosmosDB добавлена в тип перечисления зарезервированных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1659">Added CosmosDb in the reserved resource enum type</span></span>
* <span data-ttu-id="8b368-1660">Добавлено свойство имени в модели Patch.</span><span class="sxs-lookup"><span data-stu-id="8b368-1660">Added name property in Patch model</span></span>

### <a name="manage-app"></a><span data-ttu-id="8b368-1661">Управление приложением</span><span class="sxs-lookup"><span data-stu-id="8b368-1661">Manage App</span></span>
* <span data-ttu-id="8b368-1662">Исправлена ошибка в `managedapp create --kind MarketPlace`, приводившая к аварийному завершению создания экземпляра управляемого приложения Marketplace.</span><span class="sxs-lookup"><span data-stu-id="8b368-1662">Fixed bug in `managedapp create --kind MarketPlace` causing instance creation of a Marketplace managed app to crash</span></span>
* <span data-ttu-id="8b368-1663">Изменены команды`feature`, действие которых теперь ограничено поддерживаемыми профилями.</span><span class="sxs-lookup"><span data-stu-id="8b368-1663">Changed `feature` commands to be restricted to supported profiles</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1664">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1664">Role</span></span>
* <span data-ttu-id="8b368-1665">Добавлена функция перечисления членства пользователя в группах.</span><span class="sxs-lookup"><span data-stu-id="8b368-1665">Added support for listing user's group memberships</span></span>

### <a name="signalr"></a><span data-ttu-id="8b368-1666">SignalR</span><span class="sxs-lookup"><span data-stu-id="8b368-1666">SignalR</span></span>
* <span data-ttu-id="8b368-1667">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="8b368-1667">First release</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1668">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1668">Storage</span></span>
* <span data-ttu-id="8b368-1669">Добавлен параметр `--auth-mode login` для использования учетных данных пользователя для авторизации в больших двоичных объектах и очереди.</span><span class="sxs-lookup"><span data-stu-id="8b368-1669">Added `--auth-mode login` parameter for use of user's login credentials for blob and queue authorization</span></span>
* <span data-ttu-id="8b368-1670">Добавлена команда `storage container immutability-policy/legal-hold` для управления неизменяемым хранилищем.</span><span class="sxs-lookup"><span data-stu-id="8b368-1670">Added `storage container immutability-policy/legal-hold` to manage immutable storage</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1671">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1671">VM</span></span>
* <span data-ttu-id="8b368-1672">Исправлена ошибка, при которой команда `vm create --generate-ssh-keys` перезаписывала файл закрытого ключа, если отсутствовал файл открытого ключа (#4725, #6780).</span><span class="sxs-lookup"><span data-stu-id="8b368-1672">Fixed issue where `vm create --generate-ssh-keys` overwrites private key file if public key file is missing (#4725, #6780)</span></span>
* <span data-ttu-id="8b368-1673">Добавлена поддержка общей коллекции изображений с помощью команды `az sig`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1673">Added support for shared image gallery through `az sig`</span></span>

## <a name="august-28-2018"></a><span data-ttu-id="8b368-1674">28 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1674">August 28, 2018</span></span>

<span data-ttu-id="8b368-1675">Версия 2.0.45</span><span class="sxs-lookup"><span data-stu-id="8b368-1675">Version 2.0.45</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1676">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1676">Core</span></span>

* <span data-ttu-id="8b368-1677">Исправлена проблема с загрузкой пустого файла конфигурации.</span><span class="sxs-lookup"><span data-stu-id="8b368-1677">Fixed issue of loading empty configuration file</span></span>
* <span data-ttu-id="8b368-1678">Добавлена поддержка профиля `2018-03-01-hybrid` для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8b368-1678">Added support for profile `2018-03-01-hybrid` for Azure Stack</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1679">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1679">ACR</span></span>

* <span data-ttu-id="8b368-1680">Добавлено решение для операций среды выполнения без запросов ARM.</span><span class="sxs-lookup"><span data-stu-id="8b368-1680">Added a workaround for runtime operations without ARM requests</span></span>
* <span data-ttu-id="8b368-1681">Внесено изменение для исключения файлов управления версиями (например, файлов с расширениями .git, .gitignore) из отправляемого файла с расширением .tar по умолчанию для команды `build`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1681">Changed to exclude version control files (eg, .git, .gitignore) from uploaded tar by default in `build` command</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1682">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1682">ACS</span></span>

* <span data-ttu-id="8b368-1683">Внесено изменение в `aks create` с заменой параметрами по умолчанию для виртуальных машин `Standard_DS2_v2`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1683">Changed `aks create` to defaults to `Standard_DS2_v2` VMs</span></span>
* <span data-ttu-id="8b368-1684">Внесено изменение в `aks get-credentials` для вызова новых API и получения учетных данных кластера.</span><span class="sxs-lookup"><span data-stu-id="8b368-1684">Changed `aks get-credentials` to now call new apis to get cluster credential</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1685">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-1685">AppService</span></span>

* <span data-ttu-id="8b368-1686">Добавлена поддержка CORS в приложениях-функциях и веб-приложениях.</span><span class="sxs-lookup"><span data-stu-id="8b368-1686">Added support for CORS on functionapp & webapp</span></span>
* <span data-ttu-id="8b368-1687">Добавлена поддержка тегов ARM для команды создания.</span><span class="sxs-lookup"><span data-stu-id="8b368-1687">Added ARM tag support on create commands</span></span>
* <span data-ttu-id="8b368-1688">Внесено изменение в `[webapp|functionapp] identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="8b368-1688">Changed `[webapp|functionapp] identity show` to exit with code 3 upon a missing resource</span></span>

### <a name="backup"></a><span data-ttu-id="8b368-1689">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="8b368-1689">Backup</span></span>

* <span data-ttu-id="8b368-1690">Внесено изменение в `backup vault backup-properties show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="8b368-1690">Changed `backup vault backup-properties show` to exit with code 3 upon a missing resource</span></span>

### <a name="bot-service"></a><span data-ttu-id="8b368-1691">Служба Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-1691">Bot Service</span></span>

* <span data-ttu-id="8b368-1692">Начальный выпуск CLI для службы Azure Bot</span><span class="sxs-lookup"><span data-stu-id="8b368-1692">Initial Bot Service CLI Release</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8b368-1693">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="8b368-1693">Cognitive Services</span></span>

* <span data-ttu-id="8b368-1694">Добавлен новый параметр `--api-properties,`, требуемый для создания некоторых служб.</span><span class="sxs-lookup"><span data-stu-id="8b368-1694">Added new parameter `--api-properties,` which is required for creating some of the services</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-1695">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-1695">IoT</span></span>

* <span data-ttu-id="8b368-1696">Исправлена проблема со связыванием связанных центров.</span><span class="sxs-lookup"><span data-stu-id="8b368-1696">Fixed issue with associating linked hubs</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-1697">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-1697">Monitor</span></span>

* <span data-ttu-id="8b368-1698">Добавлены команды `monitor metrics alert` для создания оповещений метрик почти в реальном времени.</span><span class="sxs-lookup"><span data-stu-id="8b368-1698">Added `monitor metrics alert` commands for near-realtime metric alerts</span></span>
* <span data-ttu-id="8b368-1699">Команды `monitor alert` не рекомендуются к использованию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1699">Deprecated `monitor alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1700">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1700">Network</span></span>

* <span data-ttu-id="8b368-1701">Внесено изменение в `network application-gateway ssl-policy predefined show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="8b368-1701">Changed `network application-gateway ssl-policy predefined show` to exit with code 3 upon a missing resource</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-1702">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-1702">Resource</span></span>

* <span data-ttu-id="8b368-1703">Внесено изменение в `provider operation show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="8b368-1703">Changed `provider operation show` to exit with code 3 upon a missing resource</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1704">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1704">Storage</span></span>

* <span data-ttu-id="8b368-1705">Внесено изменение в `storage share policy show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="8b368-1705">Changed `storage share policy show` to exit with code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1706">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1706">VM</span></span>

* <span data-ttu-id="8b368-1707">Внесено изменение в `vm/vmss identity show` для выхода с кодом 3 при отсутствующем ресурсе.</span><span class="sxs-lookup"><span data-stu-id="8b368-1707">Changed `vm/vmss identity show` to exit with code 3 upon a missing resource</span></span> 
* <span data-ttu-id="8b368-1708">`--storage-caching` не рекомендуется к использованию для `vm create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1708">Deprecated `--storage-caching` for `vm create`</span></span>

## <a name="auguest-14-2018"></a><span data-ttu-id="8b368-1709">14 августа 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1709">Auguest 14, 2018</span></span>

<span data-ttu-id="8b368-1710">Версия 2.0.44</span><span class="sxs-lookup"><span data-stu-id="8b368-1710">Version 2.0.44</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1711">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1711">Core</span></span>

* <span data-ttu-id="8b368-1712">Исправлено отображение чисел в выходных данных `table`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1712">Fixed numeric display in `table` output</span></span>
* <span data-ttu-id="8b368-1713">Добавлен формат выходных данных YAML.</span><span class="sxs-lookup"><span data-stu-id="8b368-1713">Added YAML output format</span></span>

### <a name="telemetry"></a><span data-ttu-id="8b368-1714">Телеметрия</span><span class="sxs-lookup"><span data-stu-id="8b368-1714">Telemetry</span></span>

* <span data-ttu-id="8b368-1715">Улучшены функции отчетности телеметрии.</span><span class="sxs-lookup"><span data-stu-id="8b368-1715">Improved telemetry reporting</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1716">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1716">ACR</span></span>

* <span data-ttu-id="8b368-1717">Добавлены команды `content-trust policy`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1717">Added `content-trust policy` commands</span></span>
* <span data-ttu-id="8b368-1718">Исправлена проблема с правильной обработкой `.dockerignore`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1718">Fixed issue where `.dockerignore` was not handled properly</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1719">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1719">ACS</span></span>

* <span data-ttu-id="8b368-1720">Внесено изменение в `az acs/aks install-cli` для установки в разделе `%USERPROFILE%\.azure-kubectl` в Windows.</span><span class="sxs-lookup"><span data-stu-id="8b368-1720">Changed `az acs/aks install-cli` to install under `%USERPROFILE%\.azure-kubectl` on Windows</span></span>
* <span data-ttu-id="8b368-1721">Внесено изменение в `az aks install-connector` для определения RBAC в кластере и правильной настройки соединителя ACI.</span><span class="sxs-lookup"><span data-stu-id="8b368-1721">Changed `az aks install-connector` to detect if the cluster has RBAC and configure ACI Connector appropriately</span></span>
* <span data-ttu-id="8b368-1722">Внесено изменение в назначение ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="8b368-1722">Changed to role assignment to the subnet when it's provided</span></span>
* <span data-ttu-id="8b368-1723">Внесен новый параметр пропуска назначения ролей для подсети в соответствующем случае.</span><span class="sxs-lookup"><span data-stu-id="8b368-1723">Added new option to "skip role assignment" for subnet when it's provided</span></span>                                 
* <span data-ttu-id="8b368-1724">Внесено изменение в параметр пропуска назначения ролей для подсети, если назначение уже существует.</span><span class="sxs-lookup"><span data-stu-id="8b368-1724">Changed to skip role assignment to subnet when assignment already exists</span></span>                

### <a name="appservice"></a><span data-ttu-id="8b368-1725">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-1725">AppService</span></span>

* <span data-ttu-id="8b368-1726">Исправлена ошибка с созданием приложения-функции с помощью учетных записей хранения во внешних группах ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1726">Fixed a bug that prevent from creating a function-app using storage accounts in external resource groups</span></span>
* <span data-ttu-id="8b368-1727">Исправлен сбой при развертывании ZIP-архива.</span><span class="sxs-lookup"><span data-stu-id="8b368-1727">Fixed a crash on zip deployment</span></span>

### <a name="batchai"></a><span data-ttu-id="8b368-1728">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8b368-1728">BatchAI</span></span>

* <span data-ttu-id="8b368-1729">Внесены изменения в выходные данные средства ведения журнала для автоматического создания учетной записи хранения и определения *группы ресурсов*.</span><span class="sxs-lookup"><span data-stu-id="8b368-1729">Changed logger output for auto-storage account creation to specifies "resource *group*".</span></span>        

### <a name="container"></a><span data-ttu-id="8b368-1730">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-1730">Container</span></span>

* <span data-ttu-id="8b368-1731">Добавлено `--secure-environment-variables` для передачи переменных среды в контейнер.</span><span class="sxs-lookup"><span data-stu-id="8b368-1731">Added `--secure-environment-variables` for passing secure environment variables to a container</span></span>      

### <a name="iot"></a><span data-ttu-id="8b368-1732">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-1732">IoT</span></span>

* <span data-ttu-id="8b368-1733">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены устаревшие команды, которые были перемещены в расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="8b368-1733">[BREAKING CHANGE] Removed deprecated commands which have moved to the iot extension</span></span>
* <span data-ttu-id="8b368-1734">Обновлены элементы для игнорирования домена `azure-devices.net`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1734">Updated elements to not assume `azure-devices.net` domain</span></span>

### <a name="iot-central"></a><span data-ttu-id="8b368-1735">IoT Central</span><span class="sxs-lookup"><span data-stu-id="8b368-1735">Iot Central</span></span>

* <span data-ttu-id="8b368-1736">Начальный выпуск модуля IoT Central</span><span class="sxs-lookup"><span data-stu-id="8b368-1736">Initial release of IoT Central module</span></span>

### <a name="keyvault"></a><span data-ttu-id="8b368-1737">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8b368-1737">KeyVault</span></span>


* <span data-ttu-id="8b368-1738">Добавлены команды для управления учетными записями хранения и определений SAS.</span><span class="sxs-lookup"><span data-stu-id="8b368-1738">Added commands for managing storage accounts and sas-definitions</span></span>
* <span data-ttu-id="8b368-1739">Добавлены команды для правил сети.</span><span class="sxs-lookup"><span data-stu-id="8b368-1739">Added commands for network-rules</span></span>                                                           
* <span data-ttu-id="8b368-1740">Добавлен параметр `--id` для операций с секретами, ключами и сертификатами.</span><span class="sxs-lookup"><span data-stu-id="8b368-1740">Added `--id` parameter to secret, key, and certificate operations</span></span>
* <span data-ttu-id="8b368-1741">Добавлена поддержка версии с несколькими API управления хранилищем ключей.</span><span class="sxs-lookup"><span data-stu-id="8b368-1741">Added support for KV mgmt multi-api version</span></span>
* <span data-ttu-id="8b368-1742">Добавлена поддержка версии с несколькими API плоскости данных хранилища ключей.</span><span class="sxs-lookup"><span data-stu-id="8b368-1742">Added support for KV data plane multi-api version</span></span>

### <a name="relay"></a><span data-ttu-id="8b368-1743">Ретрансляция</span><span class="sxs-lookup"><span data-stu-id="8b368-1743">Relay</span></span>

* <span data-ttu-id="8b368-1744">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="8b368-1744">Initial release</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-1745">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-1745">Sql</span></span>

* <span data-ttu-id="8b368-1746">Добавлены команды `sql failover-group`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1746">Added `sql failover-group` commands</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1747">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1747">Storage</span></span>

* <span data-ttu-id="8b368-1748">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесено изменение в `storage account show-usage` для запроса параметра `--location` и отображения по регионам.</span><span class="sxs-lookup"><span data-stu-id="8b368-1748">[BREAKING CHANGE] Changed `storage account show-usage` to require `--location` parameter and will list by region</span></span>
* <span data-ttu-id="8b368-1749">Внесено изменение в параметр `--resource-group` для команд `storage account`, который теперь необязателен.</span><span class="sxs-lookup"><span data-stu-id="8b368-1749">Changed `--resource-group` parameter to be optional for `storage account` commands</span></span>
* <span data-ttu-id="8b368-1750">Удалены предупреждения о нарушении необходимого условия для отдельных сбоев в командах пакетной службы для одного сообщения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1750">Removed 'Failed precondition' warnings for individual failures in batch commands for single aggregated message</span></span>
* <span data-ttu-id="8b368-1751">Внесено изменение в команды `[blob|file] delete-batch`, которые больше не выводят выходной массив значений NULL.</span><span class="sxs-lookup"><span data-stu-id="8b368-1751">Changed `[blob|file] delete-batch` commands to no longer output array of nulls</span></span>
* <span data-ttu-id="8b368-1752">Внесено изменение в команды `blob [download|upload|delete-batch]`, которые теперь считывают маркер SAS из URL-адреса контейнера.</span><span class="sxs-lookup"><span data-stu-id="8b368-1752">Changed `blob [download|upload|delete-batch]` commands to read sas-token from container url</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1753">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1753">VM</span></span>

* <span data-ttu-id="8b368-1754">Добавлены общие фильтры для `vm list-skus` для удобства использования.</span><span class="sxs-lookup"><span data-stu-id="8b368-1754">Added common filters to `vm list-skus` for ease of use</span></span>

## <a name="july-31-2018"></a><span data-ttu-id="8b368-1755">31 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1755">July 31, 2018</span></span>

<span data-ttu-id="8b368-1756">Версия 2.0.43</span><span class="sxs-lookup"><span data-stu-id="8b368-1756">Version 2.0.43</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1757">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1757">ACR</span></span>

* <span data-ttu-id="8b368-1758">В команду `acr build-task show` добавлен флаг `--with-secure-properties`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1758">Added `--with-secure-properties` flag to `acr build-task show` command</span></span>
* <span data-ttu-id="8b368-1759">Добавлена команда `acr build-task update-build`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1759">Added `acr build-task update-build` command</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1760">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1760">ACS</span></span>

* <span data-ttu-id="8b368-1761">При завершении команды `az aks browse` нажатием клавиш CTRL + C теперь возвращается значение 0 (успешное завершение).</span><span class="sxs-lookup"><span data-stu-id="8b368-1761">Changed to return return 0 (success) when ending `az aks browse` by pressing [Ctrl+C]</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-1762">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-1762">Batch</span></span>

* <span data-ttu-id="8b368-1763">Исправлена ошибка при отображении маркера AAD в CloudShell.</span><span class="sxs-lookup"><span data-stu-id="8b368-1763">Fixed bug when showing AAD token in cloudshell</span></span>

### <a name="container"></a><span data-ttu-id="8b368-1764">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-1764">Container</span></span>

* <span data-ttu-id="8b368-1765">Удалено требование указания `--log-analytics-workspace-key` для имени или идентификатора при выборе подписки.</span><span class="sxs-lookup"><span data-stu-id="8b368-1765">Removed requirement for `--log-analytics-workspace-key` for name or ID when in set subscription</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1766">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1766">Network</span></span>

* <span data-ttu-id="8b368-1767">В профиль 2017-03-09-profile для Azure Stack добавлена поддержка DNS.</span><span class="sxs-lookup"><span data-stu-id="8b368-1767">Added dns support to 2017-03-09-profile for Azure Stack</span></span> 

### <a name="resource"></a><span data-ttu-id="8b368-1768">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-1768">Resource</span></span>

* <span data-ttu-id="8b368-1769">В `group deployment create` добавлен параметр `--rollback-on-error` для выполнения достоверно корректного развертывания в случае возникновения ошибки.</span><span class="sxs-lookup"><span data-stu-id="8b368-1769">Added `--rollback-on-error` to `group deployment create` to execute a known-good deployment on error</span></span>
* <span data-ttu-id="8b368-1770">Исправлена проблема, из-за которой использование `--parameters {}` с `group deployment create` приводило к ошибке.</span><span class="sxs-lookup"><span data-stu-id="8b368-1770">Fixed issue where `--parameters {}` with `group deployment create` resulted in an error</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1771">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1771">Role</span></span>

* <span data-ttu-id="8b368-1772">Добавлена поддержка профиля 2017-03-09-profile для Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8b368-1772">Added support for stack profile 2017-03-09-profile</span></span>
* <span data-ttu-id="8b368-1773">Исправлена проблема, из-за которой универсальные параметры обновления `app update` работали неправильно.</span><span class="sxs-lookup"><span data-stu-id="8b368-1773">Fixed issue where generic update parameters to `app update` would not work correctly</span></span>

### <a name="search"></a><span data-ttu-id="8b368-1774">Поиск</span><span class="sxs-lookup"><span data-stu-id="8b368-1774">Search</span></span>

* <span data-ttu-id="8b368-1775">Добавлены команды для службы "Поиск Azure".</span><span class="sxs-lookup"><span data-stu-id="8b368-1775">Added commands for Azure Search service</span></span>

### <a name="service-bus"></a><span data-ttu-id="8b368-1776">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="8b368-1776">Service Bus</span></span>

* <span data-ttu-id="8b368-1777">Добавлена группа команд migration для переноса пространства имен из служебной шины ценовой категории "Стандартный" в служебную шину ценовой категории "Премиум".</span><span class="sxs-lookup"><span data-stu-id="8b368-1777">Added migration command group to migrate a namespace from Service Bus Standard to Premium</span></span>
* <span data-ttu-id="8b368-1778">Добавлены новые необязательные свойства для очереди и подписки служебной шины:</span><span class="sxs-lookup"><span data-stu-id="8b368-1778">Added new optional properties to Service Bus queue and Subscription</span></span>
  *  <span data-ttu-id="8b368-1779">`--enable-batched-operations` и `--enable-dead-lettering-on-message-expiration` в `queue`;</span><span class="sxs-lookup"><span data-stu-id="8b368-1779">`--enable-batched-operations` and `--enable-dead-lettering-on-message-expiration` in `queue`</span></span>
  *  <span data-ttu-id="8b368-1780">`--dead-letter-on-filter-exceptions` в `subscriptions`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1780">`--dead-letter-on-filter-exceptions` in `subscriptions`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1781">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1781">Storage</span></span>

* <span data-ttu-id="8b368-1782">Добавлена поддержка скачивания больших файлов с помощью одного подключения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1782">Added support for download of large files using a single connection</span></span>
* <span data-ttu-id="8b368-1783">Преобразованы команды `show`, которые ранее отсутствовали: теперь в случае отсутствия ресурса не возвращается код завершения 3.</span><span class="sxs-lookup"><span data-stu-id="8b368-1783">Converted `show` commands that were missed from failing with exit code 3 upon a missing resource</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1784">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1784">VM</span></span>

* <span data-ttu-id="8b368-1785">Добавлена поддержка вывода списка групп доступности по подпискам.</span><span class="sxs-lookup"><span data-stu-id="8b368-1785">Added support to list availability sets by subscription</span></span>
* <span data-ttu-id="8b368-1786">Добавлена поддержка параметра `StandardSSD_LRS`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1786">Added support for `StandardSSD_LRS`</span></span>
* <span data-ttu-id="8b368-1787">Добавлена поддержка групп безопасности приложений при создании масштабируемого набора виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="8b368-1787">Added support for application security group on creating VM scale set</span></span>
* <span data-ttu-id="8b368-1788">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены `[vm|vmss] create`, `[vm|vmss] identity assign` и `[vm|vmss] identity remove` для вывода пользовательских удостоверений в формате словаря.</span><span class="sxs-lookup"><span data-stu-id="8b368-1788">[BREAKING CHANGE] Changed `[vm|vmss] create`, `[vm|vmss] identity assign`, and `[vm|vmss] identity remove` to output user assigned identities in dictionary format</span></span>

## <a name="july-18-2018"></a><span data-ttu-id="8b368-1789">18 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1789">July 18, 2018</span></span>

<span data-ttu-id="8b368-1790">Версия 2.0.42</span><span class="sxs-lookup"><span data-stu-id="8b368-1790">Version 2.0.42</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1791">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1791">Core</span></span>

* <span data-ttu-id="8b368-1792">Добавлена поддержка входа в окно WSL bash из браузера.</span><span class="sxs-lookup"><span data-stu-id="8b368-1792">Added support for browser-based login in WSL bash window</span></span>
* <span data-ttu-id="8b368-1793">Добавлен флаг `--force-string` для всех универсальных команд обновления.</span><span class="sxs-lookup"><span data-stu-id="8b368-1793">Added `--force-string` flag to all generic update commands</span></span>
* <span data-ttu-id="8b368-1794">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены команды show: сообщения об ошибках записываются в журнал, а команды возвращают код выхода 3, если ресурс отсутствует.</span><span class="sxs-lookup"><span data-stu-id="8b368-1794">[BREAKING CHANGE] Changed 'show' commands to log error message and fail with exit code of 3 upon a missing resource</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1795">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1795">ACR</span></span>

* <span data-ttu-id="8b368-1796">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр --no-push в команде acr build сделан обычным флагом.</span><span class="sxs-lookup"><span data-stu-id="8b368-1796">[BREAKING CHANGE] Updated '--no-push' to a pure flag in 'acr build' command</span></span>
* <span data-ttu-id="8b368-1797">В группу `acr repository` добавлены команды `show` и `update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1797">Added `show` and `update` commands under `acr repository` group</span></span>
* <span data-ttu-id="8b368-1798">Добавлен флаг `--detail` для `show-manifests` и `show-tags`, позволяющий выводить более подробные сведения.</span><span class="sxs-lookup"><span data-stu-id="8b368-1798">Added `--detail` flag for `show-manifests` and `show-tags` to show more detailed information</span></span>
* <span data-ttu-id="8b368-1799">Добавлен параметр `--image`, позволяющий получать сведения о сборке или журналы для определенного образа.</span><span class="sxs-lookup"><span data-stu-id="8b368-1799">Added `--image` parameter to support get build details or logs by an image</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1800">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1800">ACS</span></span>

* <span data-ttu-id="8b368-1801">Поведение `az aks create` изменено так, чтобы выдавалась ошибка, если `--max-pods` меньше 5.</span><span class="sxs-lookup"><span data-stu-id="8b368-1801">Changed `az aks create` to error out if `--max-pods` is less than 5</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1802">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-1802">AppService</span></span>

* <span data-ttu-id="8b368-1803">Добавлена поддержка номеров SKU для PremiumV2.</span><span class="sxs-lookup"><span data-stu-id="8b368-1803">Added support for PremiumV2 skus</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-1804">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-1804">Batch</span></span>

* <span data-ttu-id="8b368-1805">Исправлена ошибка при использовании учетных данных токена в режиме Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="8b368-1805">Fixed bug on using token credential on cloud shell mode</span></span>
* <span data-ttu-id="8b368-1806">Регистр во входных данных JSON теперь не учитывается.</span><span class="sxs-lookup"><span data-stu-id="8b368-1806">Changed JSON input to be case-insensitive</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8b368-1807">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8b368-1807">Batch AI</span></span>

* <span data-ttu-id="8b368-1808">Исправлена команда `az batchai job exec`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1808">Fixed `az batchai job exec` command</span></span>

### <a name="container"></a><span data-ttu-id="8b368-1809">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-1809">Container</span></span>

* <span data-ttu-id="8b368-1810">Удалено требование указывать имя пользователя и пароль для реестров, не связанных с dockerhub.</span><span class="sxs-lookup"><span data-stu-id="8b368-1810">Removed the requirement for username and password for non dockerhub registries</span></span>
* <span data-ttu-id="8b368-1811">Исправлена ошибка, возникающая при создании групп контейнеров из файла YAML.</span><span class="sxs-lookup"><span data-stu-id="8b368-1811">Fixed error when creating container groups from yaml file</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1812">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1812">Network</span></span>

* <span data-ttu-id="8b368-1813">В команду `network nic [create|update|delete]` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1813">Added `--no-wait` support to `network nic [create|update|delete]`</span></span> 
* <span data-ttu-id="8b368-1814">Добавлена команда `network nic wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1814">Added `network nic wait`</span></span>
* <span data-ttu-id="8b368-1815">Аргумент `--ids` команды `network vnet [subnet|peering] list` объявлен устаревшим.</span><span class="sxs-lookup"><span data-stu-id="8b368-1815">Deprecated `--ids` argument for `network vnet [subnet|peering] list`</span></span>
* <span data-ttu-id="8b368-1816">Добавлен флаг `--include-default`, позволяющий включать в выходные данные команды `network nsg rule list` стандартные правила безопасности.</span><span class="sxs-lookup"><span data-stu-id="8b368-1816">Added `--include-default` flag to include default security rules in the output of `network nsg rule list`</span></span>  

### <a name="resource"></a><span data-ttu-id="8b368-1817">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-1817">Resource</span></span>

* <span data-ttu-id="8b368-1818">В команду `group deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1818">Added `--no-wait` support to `group deployment delete`</span></span>
* <span data-ttu-id="8b368-1819">В команду `deployment delete` добавлена поддержка параметра `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1819">Added `--no-wait` support to `deployment delete`</span></span>
* <span data-ttu-id="8b368-1820">Добавлена команда `deployment wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1820">Added `deployment wait` command</span></span>
* <span data-ttu-id="8b368-1821">Исправлена проблема, когда для профиля 2017-03-09-profile по ошибке отображались команды `az deployment` для работы с подписками.</span><span class="sxs-lookup"><span data-stu-id="8b368-1821">Fixed issue where the subscription-level `az deployment` commands erroneously appeared for profile 2017-03-09-profile</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-1822">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-1822">SQL</span></span>

* <span data-ttu-id="8b368-1823">Исправлена ошибка "The provided resource group name ... did not match the name in the Url" (Указанное имя группы ресурсов ... не соответствовало имени в URL-адресе), которая возникала при указании имени эластичного пула для команд `sql db copy` и `sql db replica create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1823">Fixed 'The provided resource group name ... did not match the name in the Url' error when specifying elastic pool name for `sql db copy` and `sql db replica create` commands</span></span>
* <span data-ttu-id="8b368-1824">Разрешена настройка сервера SQL Server по умолчанию с помощью команды `az configure --defaults sql-server=<name>`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1824">Allow configuring default sql server by executing `az configure --defaults sql-server=<name>`</span></span>
* <span data-ttu-id="8b368-1825">Реализованы модули форматирования таблиц для команд `sql server`, `sql server firewall-rule`, `sql list-usages` и `sql show-usage`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1825">Implemented table formatters for `sql server`, `sql server firewall-rule`, `sql list-usages`, and `sql show-usage` commands</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1826">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1826">Storage</span></span>

* <span data-ttu-id="8b368-1827">В выходные данные команды `storage blob show` добавлено свойство `pageRanges`, которое будет заполняться для страничных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1827">Added `pageRanges` property to `storage blob show` output that will be populated for page blobs</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1828">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1828">VM</span></span>

* <span data-ttu-id="8b368-1829">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] По умолчанию команда `vmss create` теперь использует `Standard_DS1_v2` как размер экземпляра по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1829">[BREAKING CHANGE] Changed `vmss create` to use `Standard_DS1_v2` as the default instance size</span></span>
* <span data-ttu-id="8b368-1830">Добавлена поддержка параметра `--no-wait` для `vm extension [set|delete]` и `vmss extension [set|delete]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1830">Added `--no-wait` support to `vm extension [set|delete]` and `vmss extension [set|delete]`</span></span>
* <span data-ttu-id="8b368-1831">Добавлена команда `vm extension wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1831">Added `vm extension wait`</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="8b368-1832">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1832">July 3, 2018</span></span>

<span data-ttu-id="8b368-1833">Версия 2.0.41</span><span class="sxs-lookup"><span data-stu-id="8b368-1833">Version 2.0.41</span></span>

### <a name="aks"></a><span data-ttu-id="8b368-1834">AKS</span><span class="sxs-lookup"><span data-stu-id="8b368-1834">AKS</span></span>

* <span data-ttu-id="8b368-1835">Теперь для мониторинга используется идентификатор подписки.</span><span class="sxs-lookup"><span data-stu-id="8b368-1835">Changed monitoring to use subscription ID</span></span>

## <a name="july-3-2018"></a><span data-ttu-id="8b368-1836">3 июля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1836">July 3, 2018</span></span>

<span data-ttu-id="8b368-1837">Версия 2.0.40</span><span class="sxs-lookup"><span data-stu-id="8b368-1837">Version 2.0.40</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1838">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1838">Core</span></span>

* <span data-ttu-id="8b368-1839">Добавлен новый поток кода авторизации для интерактивного входа.</span><span class="sxs-lookup"><span data-stu-id="8b368-1839">Added a new authorization code flow for interactive login</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1840">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1840">ACR</span></span>

* <span data-ttu-id="8b368-1841">Добавлено состояние сборки опроса.</span><span class="sxs-lookup"><span data-stu-id="8b368-1841">Added polling build status</span></span>
* <span data-ttu-id="8b368-1842">Добавлена поддержка значений перечисления без учета регистра.</span><span class="sxs-lookup"><span data-stu-id="8b368-1842">Added support for case-insensitive enum values</span></span>
* <span data-ttu-id="8b368-1843">Добавлены параметры `--top` и `--orderby` для `show-manifests`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1843">Added `--top` and `--orderby` parameters for `show-manifests`</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1844">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1844">ACS</span></span>

* <span data-ttu-id="8b368-1845">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Управление доступом на основе ролей Kubernetes включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1845">[BREAKING CHANGE] Enable Kubernetes role-based access control by default</span></span>
* <span data-ttu-id="8b368-1846">Добавлен аргумент `--disable-rbac`. Аргумент `--enable-rbac` не рекомендуется использовать, так как теперь это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1846">Added `--disable-rbac` argument and deprecated `--enable-rbac` since it's the default now</span></span>
* <span data-ttu-id="8b368-1847">Обновлены параметры команды `aks browse`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1847">Updated options for `aks browse` command.</span></span> <span data-ttu-id="8b368-1848">Добавлена поддержка параметра `--listen-port`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1848">Added `--listen-port` support</span></span>
* <span data-ttu-id="8b368-1849">Обновлен пакет диаграмм Helm по умолчанию для команды `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1849">Updated the default helm chart package for `aks install-connector` command.</span></span> <span data-ttu-id="8b368-1850">Используйте файл virtual-kubelet-for-aks-latest.tgz.</span><span class="sxs-lookup"><span data-stu-id="8b368-1850">Use virtual-kubelet-for-aks-latest.tgz</span></span>
* <span data-ttu-id="8b368-1851">Для обновления существующего кластера добавлены команды `aks enable-addons` и `aks disable-addons`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1851">Added `aks enable-addons` and `aks disable-addons` commands to update an existing cluster</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1852">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-1852">AppService</span></span>

* <span data-ttu-id="8b368-1853">Добавлена поддержка отключения удостоверения с помощью команды `webapp identity remove`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1853">Added support for disabling identity via `webapp identity remove`</span></span>
* <span data-ttu-id="8b368-1854">Удален тег `preview` для функции идентификации.</span><span class="sxs-lookup"><span data-stu-id="8b368-1854">Removed `preview` tag for Identity feature</span></span>

### <a name="backup"></a><span data-ttu-id="8b368-1855">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="8b368-1855">Backup</span></span>

* <span data-ttu-id="8b368-1856">Обновлено определение модуля.</span><span class="sxs-lookup"><span data-stu-id="8b368-1856">Updated module definition</span></span>

### <a name="batchai"></a><span data-ttu-id="8b368-1857">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8b368-1857">BatchAI</span></span>

* <span data-ttu-id="8b368-1858">Исправлены табличные выходные данные для команд `batchai cluster node list` и `batchai job node list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1858">Fixed table output for `batchai cluster node list` and `batchai job node list` commands</span></span>

### <a name="cloud"></a><span data-ttu-id="8b368-1859">Cloud</span><span class="sxs-lookup"><span data-stu-id="8b368-1859">Cloud</span></span>

* <span data-ttu-id="8b368-1860">В облачную конфигурацию добавлен суффикс сервера `acr login`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1860">Added `acr login` server suffix to cloud config</span></span>

### <a name="container"></a><span data-ttu-id="8b368-1861">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-1861">Container</span></span>

* <span data-ttu-id="8b368-1862">Для команды `container create` действие по умолчанию изменено на длительную операцию.</span><span class="sxs-lookup"><span data-stu-id="8b368-1862">Changed `container create` to default to long running operation</span></span>
* <span data-ttu-id="8b368-1863">Добавлены параметры Log Analytics `--log-analytics-workspace` и `--log-analytics-workspace-key`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1863">Added Log Analytics parameters `--log-analytics-workspace` and `--log-analytics-workspace-key`</span></span>
* <span data-ttu-id="8b368-1864">Добавлен параметр `--protocol`, с помощью которого можно указать сетевой протокол для использования.</span><span class="sxs-lookup"><span data-stu-id="8b368-1864">Added `--protocol` parameter to specify which network protocol to use</span></span>

### <a name="extension"></a><span data-ttu-id="8b368-1865">Расширение</span><span class="sxs-lookup"><span data-stu-id="8b368-1865">Extension</span></span>

* <span data-ttu-id="8b368-1866">Изменена команда `extension list-available`. Теперь с ее помощью отображаются только расширения, совместимые с текущей версией CLI.</span><span class="sxs-lookup"><span data-stu-id="8b368-1866">Changed `extension list-available` to only show extensions compatible with CLI version</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1867">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1867">Network</span></span>

* <span data-ttu-id="8b368-1868">Исправлена проблема с зависимостью типов записей от регистра ([#6602](https://github.com/Azure/azure-cli/issues/6602)).</span><span class="sxs-lookup"><span data-stu-id="8b368-1868">Fixed issue where record types were case-sensitive ([#6602](https://github.com/Azure/azure-cli/issues/6602))</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-1869">Rdbms</span><span class="sxs-lookup"><span data-stu-id="8b368-1869">Rdbms</span></span>

* <span data-ttu-id="8b368-1870">Добавлены команды `[postgres|myql] server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1870">Added `[postgres|myql] server vnet-rule` commands</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-1871">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-1871">Resource</span></span>

* <span data-ttu-id="8b368-1872">Добавлена новая группа операций `deployment`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1872">Added new operation group `deployment`</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1873">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1873">VM</span></span>

* <span data-ttu-id="8b368-1874">Добавлена поддержка удаления удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="8b368-1874">Added support for removing system assigned identity</span></span>

## <a name="june-25-2018"></a><span data-ttu-id="8b368-1875">25 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1875">June 25, 2018</span></span>

<span data-ttu-id="8b368-1876">Версия 2.0.39</span><span class="sxs-lookup"><span data-stu-id="8b368-1876">Version 2.0.39</span></span>

### <a name="cli"></a><span data-ttu-id="8b368-1877">CLI</span><span class="sxs-lookup"><span data-stu-id="8b368-1877">CLI</span></span>

* <span data-ttu-id="8b368-1878">В установщике MSI обновлена обрезка файлов, чтобы устранить проблему с установкой расширений.</span><span class="sxs-lookup"><span data-stu-id="8b368-1878">Updated file trimming in MSI installer to fix extension installation issue</span></span>

## <a name="june-19-2018"></a><span data-ttu-id="8b368-1879">19 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1879">June 19, 2018</span></span>

<span data-ttu-id="8b368-1880">Версия 2.0.38</span><span class="sxs-lookup"><span data-stu-id="8b368-1880">Version 2.0.38</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1881">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1881">Core</span></span>

* <span data-ttu-id="8b368-1882">Добавлена глобальная поддержка параметра `--subscription` в большинстве команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-1882">Added global support for `--subscription` to most commands</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1883">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1883">ACR</span></span>

* <span data-ttu-id="8b368-1884">Добавлена зависимость `azure-storage-blob`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1884">Added `azure-storage-blob` as dependency</span></span>
* <span data-ttu-id="8b368-1885">Изменена конфигурация ЦП по умолчанию с `acr build-task create`: теперь используется 2 ядра.</span><span class="sxs-lookup"><span data-stu-id="8b368-1885">Changed default CPU configuration with `acr build-task create` to use 2 cores</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1886">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1886">ACS</span></span>

* <span data-ttu-id="8b368-1887">Обновлены параметры команды `aks use-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1887">Updated options of `aks use-dev-spaces` command.</span></span> <span data-ttu-id="8b368-1888">Добавлена поддержка параметра `--update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1888">Added `--update` support</span></span>
* <span data-ttu-id="8b368-1889">Изменена команда `aks get-credentials --admin`, чтобы не заменять контекст пользователя в `$HOME/.kube/config`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1889">Changed `aks get-credentials --admin` to not eplace the user context in `$HOME/.kube/config`</span></span>
* <span data-ttu-id="8b368-1890">В управляемых кластерах предоставляется доступное только для чтения свойство `nodeResourceGroup`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1890">Exposed read-only `nodeResourceGroup` property on managed clusters</span></span>
* <span data-ttu-id="8b368-1891">Исправлена ошибка в команде `acs browse`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1891">Fixed `acs browse` command error</span></span>
* <span data-ttu-id="8b368-1892">Параметр `--connector-name` стал необязательным для `aks install-connector`, `aks upgrade-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1892">Made `--connector-name` optional for `aks install-connector`, `aks upgrade-connector` and `aks remove-connector`</span></span>
* <span data-ttu-id="8b368-1893">Добавлены новые регионы экземпляров контейнеров Azure для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1893">Added new Azure Container Instance regions for `aks install-connector`</span></span>
* <span data-ttu-id="8b368-1894">В имя выпуска и имя узла Helm добавлено нормализованное расположение для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1894">Added the normalized location into the helm release name and node name to `aks install-connector`</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1895">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-1895">AppService</span></span>

* <span data-ttu-id="8b368-1896">Добавлена поддержка новых версий urllib.</span><span class="sxs-lookup"><span data-stu-id="8b368-1896">Added support for newer versions of urllib</span></span>
* <span data-ttu-id="8b368-1897">Добавлена поддержка `functionapp create`, что позволяет использовать план службы приложений из внешних групп ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1897">Added support to `functionapp create` to use appservice plan from external resource groups</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-1898">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-1898">Batch</span></span>

* <span data-ttu-id="8b368-1899">Удалена зависимость `azure-batch-extensions`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1899">Removed `azure-batch-extensions` dependency</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8b368-1900">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8b368-1900">Batch AI</span></span>

* <span data-ttu-id="8b368-1901">Добавлена поддержка рабочих областей.</span><span class="sxs-lookup"><span data-stu-id="8b368-1901">Added support for workspaces.</span></span> <span data-ttu-id="8b368-1902">Рабочие области позволяют объединять кластеры, файловые серверы и эксперименты в группы без ограничений по количеству созданных ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1902">Workspaces allow to group clusters, file-servers and experiments in groups removing limitation on number of resources can be created</span></span>
* <span data-ttu-id="8b368-1903">Добавлена поддержка экспериментов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1903">Added support for experiments.</span></span> <span data-ttu-id="8b368-1904">Эксперименты позволяют объединять задания в коллекции без ограничений по количеству созданных заданий.</span><span class="sxs-lookup"><span data-stu-id="8b368-1904">Experiments allow to group jobs in collections removing limitation on number of created jobs</span></span>
* <span data-ttu-id="8b368-1905">Добавлена поддержка настройки `/dev/shm` для заданий, выполняющихся в контейнере Docker.</span><span class="sxs-lookup"><span data-stu-id="8b368-1905">Added support to configure `/dev/shm` for jobs running in a docker container</span></span>
* <span data-ttu-id="8b368-1906">Добавлены команды `batchai cluster node exec` и `batchai job node exec`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1906">Added `batchai cluster node exec` and `batchai job node exec` commands.</span></span> <span data-ttu-id="8b368-1907">Эти команды позволяют выполнять любые команды непосредственно на узлах и предоставляют функциональные возможности для перенаправления портов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1907">These commands allow to execute any commands directly on nodes and provide functionality for port forwarding.</span></span>
* <span data-ttu-id="8b368-1908">Добавлена поддержка параметра `--ids` в командах `batchai`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1908">Added support for `--ids` to `batchai` commands</span></span>
* <span data-ttu-id="8b368-1909">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Все кластеры и файловые серверы необходимо создавать в рабочих областях.</span><span class="sxs-lookup"><span data-stu-id="8b368-1909">[BREAKING CHANGE] All clusters and fileservers must be created under workspaces</span></span>
* <span data-ttu-id="8b368-1910">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Задания необходимо создавать в рамках экспериментов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1910">[BREAKING CHANGE] Jobs must be created under experiments</span></span>
* <span data-ttu-id="8b368-1911">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--nfs-resource-group` из команд `cluster create` и `job create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1911">[BREAKING CHANGE] Removed `--nfs-resource-group` from `cluster create` and `job create` commands.</span></span> <span data-ttu-id="8b368-1912">Для подключения NFS из другой рабочей области или группы ресурсов следует указать идентификатор ARM файлового сервера с помощью параметра `--nfs`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1912">To mount an NFS belonging to a different workspace/resource group provide file server's ARM ID via `--nfs` option</span></span>
* <span data-ttu-id="8b368-1913">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--cluster-resource-group` из команды `job create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1913">[BREAKING CHANGE] Removed `--cluster-resource-group` from `job create` command.</span></span> <span data-ttu-id="8b368-1914">Для отправки задания в кластере, относящемся к другой рабочей области или группе ресурсов, следует указать идентификатор ARM кластера с помощью параметра `--cluster`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1914">To submit a job on a cluster belonging to a different workspace/resource group provide cluster's ARM ID via `--cluster` option</span></span>
* <span data-ttu-id="8b368-1915">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален атрибут `location` для заданий, кластера и файловых серверов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1915">[BREAKING CHANGE] Removed `location` attribute from jobs, cluster and file servers.</span></span> <span data-ttu-id="8b368-1916">Расположение теперь указывается как атрибут рабочей области.</span><span class="sxs-lookup"><span data-stu-id="8b368-1916">Location now is an attribute of a workspace.</span></span>
* <span data-ttu-id="8b368-1917">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--location` из команд `job create`, `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1917">[BREAKING CHANGE] Removed `--location` from `job create`, `cluster create` and `file-server create` commands</span></span>
* <span data-ttu-id="8b368-1918">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены имена коротких параметров, чтобы обеспечить согласованность интерфейса:</span><span class="sxs-lookup"><span data-stu-id="8b368-1918">[BREAKING CHANGE] Changed names of short options to make interface more consistent:</span></span>
  - <span data-ttu-id="8b368-1919">[`--config`, `-c`] переименовано в [`--config-file`, `-f`].</span><span class="sxs-lookup"><span data-stu-id="8b368-1919">Renamed [`--config`, `-c`] to [`--config-file`, `-f`]</span></span>
  - <span data-ttu-id="8b368-1920">[`--cluster`, `-r`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="8b368-1920">Renamed [`--cluster`, `-r`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="8b368-1921">[`--cluster`, `-n`] переименовано в [`--cluster`, `-c`].</span><span class="sxs-lookup"><span data-stu-id="8b368-1921">Renamed [`--cluster`, `-n`] to [`--cluster`, `-c`]</span></span>
  - <span data-ttu-id="8b368-1922">[`--job`, `-n`] переименовано в [`--job`, `-j`].</span><span class="sxs-lookup"><span data-stu-id="8b368-1922">Renamed [`--job`, `-n`] to [`--job`, `-j`]</span></span>

### <a name="maps"></a><span data-ttu-id="8b368-1923">Maps</span><span class="sxs-lookup"><span data-stu-id="8b368-1923">Maps</span></span>

* <span data-ttu-id="8b368-1924">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Внесены изменения в `maps account create`. Теперь необходимо принимать условия использования — либо с помощью интерактивной командной строки, либо с помощью флага `--accept-tos`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1924">[BREAKING CHANGE] Changed `maps account create` to require accepting Terms of Service either by interactive prompt or `--accept-tos` flag</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1925">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1925">Network</span></span>

* <span data-ttu-id="8b368-1926">Добавлена поддержка `https` в `network lb probe create` ([№ 6571](https://github.com/Azure/azure-cli/issues/6571)).</span><span class="sxs-lookup"><span data-stu-id="8b368-1926">Added support for `https` to `network lb probe create` [#6571](https://github.com/Azure/azure-cli/issues/6571)</span></span>
* <span data-ttu-id="8b368-1927">Исправлена проблема, из-за которой в параметре `--endpoint-status` учитывался регистр.</span><span class="sxs-lookup"><span data-stu-id="8b368-1927">Fixed issue where `--endpoint-status` was case sensitive.</span></span> [<span data-ttu-id="8b368-1928">#6502</span><span class="sxs-lookup"><span data-stu-id="8b368-1928">#6502</span></span>](https://github.com/Azure/azure-cli/issues/6502)

### <a name="reservations"></a><span data-ttu-id="8b368-1929">Резервирование</span><span class="sxs-lookup"><span data-stu-id="8b368-1929">Reservations</span></span>

* <span data-ttu-id="8b368-1930">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Добавлен обязательный параметр `ReservedResourceType` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1930">[BREAKING CHANGE] Added required parameter `ReservedResourceType` to `reservations catalog show`</span></span>
* <span data-ttu-id="8b368-1931">Добавлен параметр `Location` для команды `reservations catalog show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1931">Added parameter `Location`to `reservations catalog show`</span></span>
* <span data-ttu-id="8b368-1932">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `kind` из команды `ReservationProperties`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1932">[BREAKING CHANGE] Removed `kind` from `ReservationProperties`</span></span>
* <span data-ttu-id="8b368-1933">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `capabilities` в команде `Catalog` переименован в `sku_properties`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1933">[BREAKING CHANGE] Renamed `capabilities` to `sku_properties` in `Catalog`</span></span>
* <span data-ttu-id="8b368-1934">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены свойства `size` и `tier` из команды `Catalog`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1934">[BREAKING CHANGE] Removed `size` and `tier` properties from `Catalog`</span></span>
* <span data-ttu-id="8b368-1935">Добавлен параметр `InstanceFlexibility` для команды `reservations reservation update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1935">Added parameter `InstanceFlexibility` to `reservations reservation update`</span></span>

### <a name="role"></a><span data-ttu-id="8b368-1936">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-1936">Role</span></span>

* <span data-ttu-id="8b368-1937">Улучшена обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="8b368-1937">Improved error handling</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-1938">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-1938">SQL</span></span>

* <span data-ttu-id="8b368-1939">Исправлена вносившая путаницу ошибка, которая возникала при выполнении команды `az sql db list-editions` для расположения, недоступного для указанной подписки.</span><span class="sxs-lookup"><span data-stu-id="8b368-1939">Fixed confusing error when running `az sql db list-editions` for a location that is not available to your subscription</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-1940">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1940">Storage</span></span>

* <span data-ttu-id="8b368-1941">Выходные данные таблицы для `storage blob download` изменены на более удобочитаемые.</span><span class="sxs-lookup"><span data-stu-id="8b368-1941">Changed table output for `storage blob download` to be more readable</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1942">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1942">VM</span></span>

* <span data-ttu-id="8b368-1943">Улучшено уточнение размера виртуальной машины для поддержки ускоренной сети в `vm create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1943">Improved refine vm size check for accelerated networking support in `vm create`</span></span>
* <span data-ttu-id="8b368-1944">Для `vmss create` добавлено предупреждение о том, что стандартный размер виртуальной машины будет изменен с `Standard_D1_v2` на `Standard_DS1_v2`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1944">Added warning for `vmss create` that the default vm size will be switched from `Standard_D1_v2` to `Standard_DS1_v2`</span></span>
* <span data-ttu-id="8b368-1945">Добавлен параметр `--force-update` для команды `[vm|vmss] extension set`, что позволяет обновлять расширение, даже если конфигурация не изменялась.</span><span class="sxs-lookup"><span data-stu-id="8b368-1945">Added `--force-update` to `[vm|vmss] extension set` to update the extension even when the configuration has not changed</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="8b368-1946">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1946">June 13, 2018</span></span>

<span data-ttu-id="8b368-1947">Версия 2.0.37</span><span class="sxs-lookup"><span data-stu-id="8b368-1947">Version 2.0.37</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1948">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1948">Core</span></span>

* <span data-ttu-id="8b368-1949">Улучшена интерактивная телеметрия.</span><span class="sxs-lookup"><span data-stu-id="8b368-1949">Improved interactive telemetry</span></span>

## <a name="june-13-2018"></a><span data-ttu-id="8b368-1950">13 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1950">June 13, 2018</span></span>

<span data-ttu-id="8b368-1951">Версия 2.0.36</span><span class="sxs-lookup"><span data-stu-id="8b368-1951">Version 2.0.36</span></span>

### <a name="aks"></a><span data-ttu-id="8b368-1952">AKS</span><span class="sxs-lookup"><span data-stu-id="8b368-1952">AKS</span></span>

* <span data-ttu-id="8b368-1953">В `aks create` добавлены дополнительные сетевые параметры.</span><span class="sxs-lookup"><span data-stu-id="8b368-1953">Added advanced networking options to `aks create`</span></span>
* <span data-ttu-id="8b368-1954">В `aks create` добавлены аргументы для наблюдения и маршрутизации HTTP-трафика.</span><span class="sxs-lookup"><span data-stu-id="8b368-1954">Added arguments to `aks create` to enable monitoring and HTTP routing</span></span>
* <span data-ttu-id="8b368-1955">Добавлен аргумент `--no-ssh-key` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="8b368-1955">Added `--no-ssh-key` argument to `aks create`</span></span>
* <span data-ttu-id="8b368-1956">Добавлен аргумент `--enable-rbac` для команды `aks create`</span><span class="sxs-lookup"><span data-stu-id="8b368-1956">Added `--enable-rbac` argument to `aks create`</span></span>
* <span data-ttu-id="8b368-1957">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] В `aks create` добавлена поддержка аутентификации Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8b368-1957">[PREVIEW] Added support for Azure Active Directory authentication to `aks create`</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-1958">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-1958">AppService</span></span>

* <span data-ttu-id="8b368-1959">Устранена проблема с несовместимыми версиями urllib.</span><span class="sxs-lookup"><span data-stu-id="8b368-1959">Fixed an issue with incompatible urllib versions</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="8b368-1960">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1960">June 5, 2018</span></span>

<span data-ttu-id="8b368-1961">Версия 2.0.35</span><span class="sxs-lookup"><span data-stu-id="8b368-1961">Version 2.0.35</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-1962">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-1962">Interactive</span></span>

* <span data-ttu-id="8b368-1963">Добавлены ограничения в зависимости интерактивного режима.</span><span class="sxs-lookup"><span data-stu-id="8b368-1963">Added limits to the dependencies of interactive mode</span></span>

## <a name="june-5-2018"></a><span data-ttu-id="8b368-1964">5 июня 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1964">June 5, 2018</span></span>

<span data-ttu-id="8b368-1965">Версия 2.0.34</span><span class="sxs-lookup"><span data-stu-id="8b368-1965">Version 2.0.34</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1966">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1966">Core</span></span>

* <span data-ttu-id="8b368-1967">Добавлена поддержка перекрестных ссылок на ресурсы клиента.</span><span class="sxs-lookup"><span data-stu-id="8b368-1967">Added support for cross tenant resource referencing</span></span>
* <span data-ttu-id="8b368-1968">Улучшена надежность при передаче данных телеметрии.</span><span class="sxs-lookup"><span data-stu-id="8b368-1968">Improved telemetry upload reliability</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-1969">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-1969">ACR</span></span>

* <span data-ttu-id="8b368-1970">Добавлена поддержка VSTS в качестве расположения удаленного источника.</span><span class="sxs-lookup"><span data-stu-id="8b368-1970">Added support for VSTS as a remote source location</span></span>
* <span data-ttu-id="8b368-1971">Добавлена команда `acr import`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1971">Added `acr import` command</span></span>

### <a name="aks"></a><span data-ttu-id="8b368-1972">AKS</span><span class="sxs-lookup"><span data-stu-id="8b368-1972">AKS</span></span>

* <span data-ttu-id="8b368-1973">Изменена команда `aks get-credentials` для создания файла конфигурации kube с более надежными разрешениями файловой системы.</span><span class="sxs-lookup"><span data-stu-id="8b368-1973">Changed `aks get-credentials` to create the kube config file with more secure filesystem permissions</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-1974">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-1974">Batch</span></span>

* <span data-ttu-id="8b368-1975">Исправлена ошибка, связанная с форматированием таблиц при выполнении команды pool list. [[Ошибка #4378](https://github.com/Azure/azure-cli/issues/4378)]</span><span class="sxs-lookup"><span data-stu-id="8b368-1975">Fixed bug in Pool list table formatting [[Issue #4378](https://github.com/Azure/azure-cli/issues/4378)]</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-1976">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-1976">IOT</span></span>

* <span data-ttu-id="8b368-1977">Добавлена возможность создания Центров Интернета вещей категории "Базовый".</span><span class="sxs-lookup"><span data-stu-id="8b368-1977">Added support for creating Basic Tier IoT Hubs</span></span>

### <a name="network"></a><span data-ttu-id="8b368-1978">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-1978">Network</span></span>

* <span data-ttu-id="8b368-1979">Улучшена команда `network vnet peering`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1979">Improved `network vnet peering`</span></span>

### <a name="policy-insights"></a><span data-ttu-id="8b368-1980">Анализ политик</span><span class="sxs-lookup"><span data-stu-id="8b368-1980">Policy Insights</span></span>

* <span data-ttu-id="8b368-1981">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="8b368-1981">Initial Release</span></span>

### <a name="arm"></a><span data-ttu-id="8b368-1982">ARM</span><span class="sxs-lookup"><span data-stu-id="8b368-1982">ARM</span></span>

* <span data-ttu-id="8b368-1983">Добавлены команды `account management-group`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1983">Added `account management-group` commands.</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-1984">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-1984">SQL</span></span>

* <span data-ttu-id="8b368-1985">Добавлены новые команды для управляемого экземпляра:</span><span class="sxs-lookup"><span data-stu-id="8b368-1985">Added new managed instance commands:</span></span>
  * `sql mi create`
  * `sql mi show`
  * `sql mi list`
  * `sql mi update`
  * `sql mi delete`
* <span data-ttu-id="8b368-1986">Добавлены новые команды для управляемой базы данных:</span><span class="sxs-lookup"><span data-stu-id="8b368-1986">Added new managed database commands:</span></span>
  * `sql midb create`
  * `sql midb show`
  * `sql midb list`
  * `sql midb restore`
  * `sql midb delete`

### <a name="storage"></a><span data-ttu-id="8b368-1987">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-1987">Storage</span></span>

* <span data-ttu-id="8b368-1988">Добавлены типы MIME для JSON и JavaScript, выводимые из расширений файлов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1988">Added extra mimetypes for json and javascript to be inferred from file extensions</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-1989">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-1989">VM</span></span>

* <span data-ttu-id="8b368-1990">Изменена команда `vm list-skus` для использования фиксированных столбцов, а также добавлено предупреждение об удалении `Tier` и `Size`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1990">Changed `vm list-skus` to use fixed columns and add warning that `Tier` and `Size` will be removed</span></span>
* <span data-ttu-id="8b368-1991">Добавлен параметр `--accelerated-networking` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1991">Added `--accelerated-networking` option to `vm create`</span></span>
* <span data-ttu-id="8b368-1992">Добавлен параметр `--tags` для команды `identity create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1992">Added `--tags` to `identity create`</span></span>

## <a name="may-22-2018"></a><span data-ttu-id="8b368-1993">22 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-1993">May 22, 2018</span></span>

<span data-ttu-id="8b368-1994">Версия 2.0.33</span><span class="sxs-lookup"><span data-stu-id="8b368-1994">Version 2.0.33</span></span>

### <a name="core"></a><span data-ttu-id="8b368-1995">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-1995">Core</span></span>

* <span data-ttu-id="8b368-1996">Добавлена возможность включения символа `@` в имена файлов.</span><span class="sxs-lookup"><span data-stu-id="8b368-1996">Added support for expanding `@` in file names</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-1997">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-1997">ACS</span></span>

* <span data-ttu-id="8b368-1998">Добавлены новые команды для Dev Spaces: `aks use-dev-spaces` и `aks remove-dev-spaces`.</span><span class="sxs-lookup"><span data-stu-id="8b368-1998">Added new Dev-Spaces commands `aks use-dev-spaces` and `aks remove-dev-spaces`</span></span>
* <span data-ttu-id="8b368-1999">Исправлена опечатка в справочном сообщении.</span><span class="sxs-lookup"><span data-stu-id="8b368-1999">Fixed typo in help message</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2000">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-2000">AppService</span></span>

* <span data-ttu-id="8b368-2001">Улучшены команды общего обновления.</span><span class="sxs-lookup"><span data-stu-id="8b368-2001">Improved generic update commands</span></span>
* <span data-ttu-id="8b368-2002">Добавлена поддержка асинхронного выполнения для `webapp deployment source config-zip`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2002">Added async support for `webapp deployment source config-zip`</span></span>

### <a name="container"></a><span data-ttu-id="8b368-2003">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-2003">Container</span></span>

* <span data-ttu-id="8b368-2004">Добавлена возможность экспорта группы контейнеров в формате YAML.</span><span class="sxs-lookup"><span data-stu-id="8b368-2004">Added support for exporting a container group in yaml format</span></span>
* <span data-ttu-id="8b368-2005">Добавлена возможность использования файла YAML для создания или обновления группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2005">Added support for using a yaml file to create / update a container group</span></span>

### <a name="extension"></a><span data-ttu-id="8b368-2006">Расширение</span><span class="sxs-lookup"><span data-stu-id="8b368-2006">Extension</span></span>

* <span data-ttu-id="8b368-2007">Улучшена операция удаления расширений.</span><span class="sxs-lookup"><span data-stu-id="8b368-2007">Improved removal of extensions</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-2008">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-2008">Interactive</span></span>

* <span data-ttu-id="8b368-2009">Изменены параметры ведения журнала для отключения средства синтаксического анализа для завершенных операций.</span><span class="sxs-lookup"><span data-stu-id="8b368-2009">Changed logging to mute parser for completions</span></span>
* <span data-ttu-id="8b368-2010">Улучшена обработка поврежденных кэшей справки.</span><span class="sxs-lookup"><span data-stu-id="8b368-2010">Improved handling of bad help caches</span></span>

### <a name="keyvault"></a><span data-ttu-id="8b368-2011">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8b368-2011">KeyVault</span></span>

* <span data-ttu-id="8b368-2012">Исправлены команды хранилища ключей для работы с удостоверениями в Cloud Shell или виртуальных машинах.</span><span class="sxs-lookup"><span data-stu-id="8b368-2012">Fixed keyvault commands to work in cloud shell or VMs with identity</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2013">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2013">Network</span></span>

* <span data-ttu-id="8b368-2014">Исправлена проблема, при которой `network watcher show-topology` не будет выполняться, если виртуальной сети или подсети присвоить имя. [#6326](https://github.com/Azure/azure-cli/issues/6326)</span><span class="sxs-lookup"><span data-stu-id="8b368-2014">Fix issue where `network watcher show-topology` would not work with vnet and/or subnet name [#6326](https://github.com/Azure/azure-cli/issues/6326)</span></span>
* <span data-ttu-id="8b368-2015">Исправлена проблема, при которой некоторые команды `network watcher` выдают ошибку, что Наблюдатель за сетями не включен в определенных регионах. [#6264](https://github.com/Azure/azure-cli/issues/6264)</span><span class="sxs-lookup"><span data-stu-id="8b368-2015">Fix issue where some `network watcher` commands would claim Network Watcher is not enabled for regions when it actually is [#6264](https://github.com/Azure/azure-cli/issues/6264)</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-2016">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-2016">SQL</span></span>

* <span data-ttu-id="8b368-2017">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменены объекты ответа, возвращаемые в результатах команд `db` и `dw`:</span><span class="sxs-lookup"><span data-stu-id="8b368-2017">[BREAKING CHANGE] Changed response objects returned from `db` and `dw` commands:</span></span>
    * <span data-ttu-id="8b368-2018">Свойство `serviceLevelObjective` переименовано на `currentServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2018">Renamed `serviceLevelObjective` property to `currentServiceObjectiveName`</span></span>
    * <span data-ttu-id="8b368-2019">Удалены свойства `currentServiceObjectiveId` и `requestedServiceObjectiveId`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2019">Removed `currentServiceObjectiveId` and `requestedServiceObjectiveId` properties</span></span>
    * <span data-ttu-id="8b368-2020">Тип свойства `maxSizeBytes` изменен со строкового на целое число.</span><span class="sxs-lookup"><span data-stu-id="8b368-2020">Changed `maxSizeBytes` property to be an integer value instead of a string</span></span>
* <span data-ttu-id="8b368-2021">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `db` и `dw` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="8b368-2021">[BREAKING CHANGE] Changed the following `db` and `dw` properties to be read-only:</span></span>
    * <span data-ttu-id="8b368-2022">`requestedServiceObjectiveName`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2022">`requestedServiceObjectiveName`.</span></span>  <span data-ttu-id="8b368-2023">Для обновления используйте параметр `--service-objective` или задайте свойство `sku.name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2023">To update, use the `--service-objective` parameter or set the `sku.name` property</span></span>
    * <span data-ttu-id="8b368-2024">`edition`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2024">`edition`.</span></span> <span data-ttu-id="8b368-2025">Для обновления используйте параметр `--edition` или задайте свойство `sku.tier`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2025">To update, use the `--edition` parameter or set the `sku.tier` property</span></span>
    * <span data-ttu-id="8b368-2026">`elasticPoolName`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2026">`elasticPoolName`.</span></span> <span data-ttu-id="8b368-2027">Для обновления используйте параметр `--elastic-pool` или задайте свойство `elasticPoolId`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2027">To update, use the `--elastic-pool` parameter or set the `elasticPoolId` property</span></span>
* <span data-ttu-id="8b368-2028">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Теперь следующие свойства `elastic-pool` доступны только для чтения:</span><span class="sxs-lookup"><span data-stu-id="8b368-2028">[BREAKING CHANGE] Changed the following `elastic-pool` properties to be read-only:</span></span>
    * <span data-ttu-id="8b368-2029">`edition`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2029">`edition`.</span></span> <span data-ttu-id="8b368-2030">Для обновления используйте параметр `--edition`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2030">To update, use the `--edition` parameter</span></span>
    * <span data-ttu-id="8b368-2031">`dtu`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2031">`dtu`.</span></span> <span data-ttu-id="8b368-2032">Для обновления используйте параметр `--capacity`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2032">To update, use the `--capacity` parameter</span></span>
    *  <span data-ttu-id="8b368-2033">`databaseDtuMin`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2033">`databaseDtuMin`.</span></span> <span data-ttu-id="8b368-2034">Для обновления используйте параметр `--db-min-capacity`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2034">To update, use the `--db-min-capacity` parameter</span></span>
    *  <span data-ttu-id="8b368-2035">`databaseDtuMax`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2035">`databaseDtuMax`.</span></span> <span data-ttu-id="8b368-2036">Для обновления используйте параметр `--db-max-capacity`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2036">To update, use the `--db-max-capacity` parameter</span></span>
* <span data-ttu-id="8b368-2037">Добавлены параметры `--family` и `--capacity` для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2037">Added `--family` and `--capacity` parameters to `db`, `dw`, and `elastic-pool` commands.</span></span>
* <span data-ttu-id="8b368-2038">Добавлены модули форматирования таблиц для команд `db`, `dw` и `elastic-pool`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2038">Added table formatters to `db`, `dw`, and `elastic-pool` commands.</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2039">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2039">Storage</span></span>

* <span data-ttu-id="8b368-2040">Добавлено средство заполнения для аргумента `--account-name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2040">Added completer for `--account-name` argument</span></span>
* <span data-ttu-id="8b368-2041">Устранена проблема, связанная с командой `storage entity query`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2041">Fixed problem with `storage entity query`</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2042">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2042">VM</span></span>

* <span data-ttu-id="8b368-2043">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--write-accelerator` из команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2043">[BREAKING CHANGE] Removed `--write-accelerator` from `vm create`.</span></span> <span data-ttu-id="8b368-2044">Такие же возможности предоставляет команда `vm update` или `vm disk attach`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2044">The same support can be accessed through `vm update` or `vm disk attach`</span></span>
* <span data-ttu-id="8b368-2045">Устранена проблема с сопоставлением образов расширения в команде `[vm|vmss] extension`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2045">Fixed extension image matching in `[vm|vmss] extension`</span></span>
* <span data-ttu-id="8b368-2046">Добавлен параметр `--boot-diagnostics-storage` для команды `vm create` для записи журнала загрузки.</span><span class="sxs-lookup"><span data-stu-id="8b368-2046">Added `--boot-diagnostics-storage` to `vm create` to capture boot log</span></span>
* <span data-ttu-id="8b368-2047">Добавлен параметр `--license-type` для команды `[vm|vmss] update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2047">Added `--license-type` to `[vm|vmss] update`</span></span>

## <a name="may-7-2018"></a><span data-ttu-id="8b368-2048">7 мая 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2048">May 7, 2018</span></span>

<span data-ttu-id="8b368-2049">Версия 2.0.32</span><span class="sxs-lookup"><span data-stu-id="8b368-2049">Version 2.0.32</span></span>

### <a name="core"></a><span data-ttu-id="8b368-2050">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-2050">Core</span></span>

* <span data-ttu-id="8b368-2051">Исправлено необработанное исключение при получении секретов из основной учетной записи службы с сертификатом.</span><span class="sxs-lookup"><span data-stu-id="8b368-2051">Fixed an unhandled exception when retrieving secrets from a service principal account with cert</span></span>
* <span data-ttu-id="8b368-2052">Добавлена ограниченная поддержка для позиционных аргументов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2052">Added limited support for positional arguments</span></span>
* <span data-ttu-id="8b368-2053">Исправлена проблема, когда `--query` нельзя использовать с `--ids`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2053">Fix issue where `--query` could not be used with `--ids`.</span></span> [<span data-ttu-id="8b368-2054">#5591</span><span class="sxs-lookup"><span data-stu-id="8b368-2054">#5591</span></span>](https://github.com/Azure/azure-cli/issues/5591)
* <span data-ttu-id="8b368-2055">Улучшены сценарии конвейерной передачи от команд при использовании `--ids`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2055">Improved piping scenarios from commands when using `--ids`.</span></span> <span data-ttu-id="8b368-2056">Добавлена поддержка `-o tsv` с указанием запроса или `-o json` без указания запроса.</span><span class="sxs-lookup"><span data-stu-id="8b368-2056">Supports `-o tsv` with a query specified or `-o json` without specifying a query</span></span>
* <span data-ttu-id="8b368-2057">Добавлена команда предложения в случае ошибки, если пользователи вводят команды с опечаткой.</span><span class="sxs-lookup"><span data-stu-id="8b368-2057">Added command suggestions on error if users have typo in their commands</span></span>
* <span data-ttu-id="8b368-2058">Исправлена ошибка, когда пользователи вводят `az ''`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2058">Improved error when users type `az ''`</span></span>
* <span data-ttu-id="8b368-2059">Добавлена поддержка настраиваемого ресурса для командных модулей и расширений.</span><span class="sxs-lookup"><span data-stu-id="8b368-2059">Added support custom resource types for command modules and extensions</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-2060">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-2060">ACR</span></span>

* <span data-ttu-id="8b368-2061">Добавлены команды сборки ACR.</span><span class="sxs-lookup"><span data-stu-id="8b368-2061">Added ACR Build commands</span></span>
* <span data-ttu-id="8b368-2062">Исправлена ошибка о не найденных сообщениях об ошибках.</span><span class="sxs-lookup"><span data-stu-id="8b368-2062">Improved resource not found error messages</span></span>
* <span data-ttu-id="8b368-2063">Оптимизированы производительность создания ресурсов и обработка ошибок.</span><span class="sxs-lookup"><span data-stu-id="8b368-2063">Improved resource creation performance and error handling</span></span>
* <span data-ttu-id="8b368-2064">Улучшены возможности входа ACR в нестандартные консоли и WSL.</span><span class="sxs-lookup"><span data-stu-id="8b368-2064">Improved acr login in non-standard consoles and WSL</span></span>
* <span data-ttu-id="8b368-2065">Улучшены сообщения об ошибках команд репозитория.</span><span class="sxs-lookup"><span data-stu-id="8b368-2065">Improved repository commands error messages</span></span>
* <span data-ttu-id="8b368-2066">Обновлены столбцы таблиц и порядок их расположения.</span><span class="sxs-lookup"><span data-stu-id="8b368-2066">Updated table columns and ordering</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2067">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2067">ACS</span></span>

* <span data-ttu-id="8b368-2068">Добавлено предупреждение о том, что `az aks` — это предварительная версия службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-2068">Added warning that `az aks` is a preview service</span></span>
* <span data-ttu-id="8b368-2069">Исправлена проблема с разрешением в `aks install-connector`, когда `--aci-resource-group` не указывается.</span><span class="sxs-lookup"><span data-stu-id="8b368-2069">Fixed the permission issue in `aks install-connector` when `--aci-resource-group` is not specified</span></span>

### <a name="ams"></a><span data-ttu-id="8b368-2070">AMS</span><span class="sxs-lookup"><span data-stu-id="8b368-2070">AMS</span></span>

* <span data-ttu-id="8b368-2071">Первоначальный выпуск. Управление ресурсами Служб мультимедиа Azure.</span><span class="sxs-lookup"><span data-stu-id="8b368-2071">Initial release - Manage Azure Media Services resources</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2072">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2072">Appservice</span></span>

* <span data-ttu-id="8b368-2073">Исправлена ошибка в `webapp delete`, когда `--slot` предоставляется.</span><span class="sxs-lookup"><span data-stu-id="8b368-2073">Fixed a bug in `webapp delete` when `--slot` is provided</span></span>
* <span data-ttu-id="8b368-2074">Удалено `--runtime-version` из `webapp auth update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2074">Removed `--runtime-version` from `webapp auth update`</span></span>
* <span data-ttu-id="8b368-2075">Добавлена поддержка min\_tls\_version и https2.0.</span><span class="sxs-lookup"><span data-stu-id="8b368-2075">Added support for min\_tls\_version & https2.0</span></span>
* <span data-ttu-id="8b368-2076">Добавлена поддержка нескольких контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2076">Added support for multicontainers</span></span>

### <a name="batch-ai"></a><span data-ttu-id="8b368-2077">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8b368-2077">Batch AI</span></span>

* <span data-ttu-id="8b368-2078">Изменено `batchai create cluster` с учетом приоритета виртуальной машины при настройке в файле конфигурации кластера.</span><span class="sxs-lookup"><span data-stu-id="8b368-2078">Changed `batchai create cluster` to respect vm priority configured in the cluster's configuration file</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8b368-2079">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="8b368-2079">Cognitive Services</span></span>

* <span data-ttu-id="8b368-2080">Исправлена опечатка в примере для `cognitiveservices account create` ([№ 5603](https://github.com/Azure/azure-cli/issues/5603)).</span><span class="sxs-lookup"><span data-stu-id="8b368-2080">Fixed typo in example for `cognitiveservices account create` [#5603](https://github.com/Azure/azure-cli/issues/5603)</span></span>

### <a name="consumption"></a><span data-ttu-id="8b368-2081">Потребление</span><span class="sxs-lookup"><span data-stu-id="8b368-2081">Consumption</span></span>

* <span data-ttu-id="8b368-2082">Добавлены новые команды в API для управления бюджетом.</span><span class="sxs-lookup"><span data-stu-id="8b368-2082">Added new commands for budget API</span></span>

### <a name="container"></a><span data-ttu-id="8b368-2083">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-2083">Container</span></span>

* <span data-ttu-id="8b368-2084">Удалено требование `--registry-server` для `container create`, когда сервер реестра включен в имя образа.</span><span class="sxs-lookup"><span data-stu-id="8b368-2084">Removed requirement for `--registry-server` for `container create` when a registry server is included in the image name</span></span>

### <a name="cosmos-db"></a><span data-ttu-id="8b368-2085">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-2085">Cosmos DB</span></span>

* <span data-ttu-id="8b368-2086">Добавлена поддержка VNET для Azure CLI в Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-2086">Introducing VNET support for Azure CLI - Cosmos DB</span></span>

### <a name="dms"></a><span data-ttu-id="8b368-2087">DMS</span><span class="sxs-lookup"><span data-stu-id="8b368-2087">DMS</span></span>

* <span data-ttu-id="8b368-2088">Исходный выпуск. Добавлена поддержка сценария миграции SQL — Azure SQL.</span><span class="sxs-lookup"><span data-stu-id="8b368-2088">Initial release - Adds support for the SQL to Azure SQL migration scenario</span></span>

### <a name="extension"></a><span data-ttu-id="8b368-2089">Расширение</span><span class="sxs-lookup"><span data-stu-id="8b368-2089">Extension</span></span>

* <span data-ttu-id="8b368-2090">Исправлена ошибка, когда метаданные остановленного расширения отображались.</span><span class="sxs-lookup"><span data-stu-id="8b368-2090">Fixed bug where extension metadata stopped being shown</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-2091">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-2091">Interactive</span></span>

* <span data-ttu-id="8b368-2092">Разрешена работа интерактивных средств завершения с позиционными аргументами.</span><span class="sxs-lookup"><span data-stu-id="8b368-2092">Allow interactive completers to function with positional arguments</span></span>
* <span data-ttu-id="8b368-2093">Добавлены более понятные выходные данные, когда пользователи вводят \'.</span><span class="sxs-lookup"><span data-stu-id="8b368-2093">More user-friendly output when users type '\'</span></span>
* <span data-ttu-id="8b368-2094">Исправлены завершения для параметров без справки.</span><span class="sxs-lookup"><span data-stu-id="8b368-2094">Fixed completions for parameters with no help</span></span>
* <span data-ttu-id="8b368-2095">Исправлены описания для групп команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-2095">Fixed descriptions for command-groups</span></span>

### <a name="lab"></a><span data-ttu-id="8b368-2096">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="8b368-2096">Lab</span></span>

* <span data-ttu-id="8b368-2097">Исправлены регрессии из преобразования Knack.</span><span class="sxs-lookup"><span data-stu-id="8b368-2097">Fixed regressions from knack conversion</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2098">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2098">Network</span></span>

* <span data-ttu-id="8b368-2099">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--ids` для:</span><span class="sxs-lookup"><span data-stu-id="8b368-2099">[BREAKING CHANGE] Removed the `--ids` parameter for:</span></span>
  * `express-route auth list`
  * `express-route peering list`
  * `nic ip-config list`
  * `nsg rule list`
  * `route-filter rule list`
  * `route-table route list`
  * `traffic-manager endpoint list`

### <a name="profile"></a><span data-ttu-id="8b368-2100">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-2100">Profile</span></span>

* <span data-ttu-id="8b368-2101">Исправлено определение источника `disk create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2101">Fixed `disk create` source detection</span></span>
* <span data-ttu-id="8b368-2102">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--msi-port` и `--identity-port`, так как они больше не используются.</span><span class="sxs-lookup"><span data-stu-id="8b368-2102">[BREAKING CHANGE] Removed `--msi-port` and `--identity-port` as they are no longer used</span></span>
* <span data-ttu-id="8b368-2103">Исправлена опечатка в кратком описании `account get-access-token`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2103">Fixed typo in `account get-access-token` short summary</span></span>

### <a name="redis"></a><span data-ttu-id="8b368-2104">Redis</span><span class="sxs-lookup"><span data-stu-id="8b368-2104">Redis</span></span>

* <span data-ttu-id="8b368-2105">Вместо `redis patch-schedule patch-schedule show` теперь используется `redis patch-schedule show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2105">Deprecated `redis patch-schedule patch-schedule show` in favor of `redis patch-schedule show`</span></span>
* <span data-ttu-id="8b368-2106">`redis list-all` теперь не используется.</span><span class="sxs-lookup"><span data-stu-id="8b368-2106">Deprecated `redis list-all`.</span></span> <span data-ttu-id="8b368-2107">Эта функция включена в `redis list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2107">This functionality has been folded into `redis list`</span></span>
* <span data-ttu-id="8b368-2108">Вместо `redis import-method` теперь используется `redis import`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2108">Deprecated `redis import-method` in favor of `redis import`</span></span>
* <span data-ttu-id="8b368-2109">Добавлена поддержка `--ids` для разных команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-2109">Added support for `--ids` to various commands</span></span>

### <a name="role"></a><span data-ttu-id="8b368-2110">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-2110">Role</span></span>

* <span data-ttu-id="8b368-2111">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `ad sp reset-credentials` по причине устаревания.</span><span class="sxs-lookup"><span data-stu-id="8b368-2111">[BREAKING CHANGE] Removed deprecated `ad sp reset-credentials`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2112">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2112">Storage</span></span>

* <span data-ttu-id="8b368-2113">Разрешено применение SAS-токенов назначения к источнику для копирования BLOB-объектов, если SAS источника и ключ учетной записи не указаны.</span><span class="sxs-lookup"><span data-stu-id="8b368-2113">Allow destination sas-token to apply to source for blob copy if source sas and account key are unspecified</span></span>
* <span data-ttu-id="8b368-2114">Добавлено отображение времени ожидания сокета для отправки и скачивания большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="8b368-2114">Exposed --socket-timeout for blob uploads and downloads</span></span>
* <span data-ttu-id="8b368-2115">Добавлена обработка имен больших двоичных объектов, которые начинаются с разделителей пути, как относительных путей.</span><span class="sxs-lookup"><span data-stu-id="8b368-2115">Treat blob names that start with path separators as relative paths</span></span>
* <span data-ttu-id="8b368-2116">Разрешено использовать `storage blob copy --source-sas` с начальным символом запроса "?".</span><span class="sxs-lookup"><span data-stu-id="8b368-2116">Allow `storage blob copy --source-sas` with starting query char, '?'</span></span>
* <span data-ttu-id="8b368-2117">Исправлено `storage entity query --marker` для принятия списка пар "ключ-значение".</span><span class="sxs-lookup"><span data-stu-id="8b368-2117">Fixed `storage entity query --marker` to accept list of key=values</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2118">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2118">VM</span></span>

* <span data-ttu-id="8b368-2119">Исправлена недопустимая логика обнаружения в URI неуправляемого BLOB-объекта.</span><span class="sxs-lookup"><span data-stu-id="8b368-2119">Fixed an invalid detection logic on unmanaged blob uri</span></span>
* <span data-ttu-id="8b368-2120">Добавлена поддержка шифрования диска без предоставления пользователем субъектов-служб.</span><span class="sxs-lookup"><span data-stu-id="8b368-2120">Added support disk encryption w/o user provided service principals</span></span>
* <span data-ttu-id="8b368-2121">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Не используйте ManagedIdentityExtension виртуальной машины для включения поддержки MSI.</span><span class="sxs-lookup"><span data-stu-id="8b368-2121">[BREAKING CHANGE] Do not use VM 'ManagedIdentityExtension' for MSI support</span></span>
* <span data-ttu-id="8b368-2122">Добавлена поддержка политики вытеснения для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2122">Added support for eviction policy to `vmss`</span></span>
* <span data-ttu-id="8b368-2123">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалено `--ids` из:</span><span class="sxs-lookup"><span data-stu-id="8b368-2123">[BREAKING CHANGE] Removed `--ids` from:</span></span>
  * `vm extension list`
  * `vm secret list`
  * `vm unmanaged-disk list`
  * `vmss nic list`
* <span data-ttu-id="8b368-2124">Добавлена поддержка ускорителя записи.</span><span class="sxs-lookup"><span data-stu-id="8b368-2124">Added write accelerator support</span></span>
* <span data-ttu-id="8b368-2125">Добавлена команда `vmss perform-maintenance`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2125">Added `vmss perform-maintenance`</span></span>
* <span data-ttu-id="8b368-2126">Исправлено `vm diagnostics set` для надежного определения типа ОС виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="8b368-2126">Fixed `vm diagnostics set` to detect VM's OS type reliably</span></span>
* <span data-ttu-id="8b368-2127">Изменено `vm resize` для проверки того, отличается ли запрошенный размер от установленного (с обновлением только при изменении).</span><span class="sxs-lookup"><span data-stu-id="8b368-2127">Changed `vm resize` to check if the requested size is different than currently set and update only on change</span></span>


## <a name="april-10-2018"></a><span data-ttu-id="8b368-2128">10 апреля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2128">April 10, 2018</span></span>

<span data-ttu-id="8b368-2129">Версия 2.0.31</span><span class="sxs-lookup"><span data-stu-id="8b368-2129">Version 2.0.31</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-2130">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-2130">ACR</span></span>

* <span data-ttu-id="8b368-2131">Улучшена обработка ошибок при откате wincred.</span><span class="sxs-lookup"><span data-stu-id="8b368-2131">Improved error handling of wincred fallback</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2132">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2132">ACS</span></span>

* <span data-ttu-id="8b368-2133">Срок действия имен субъектов-служб, созданных службой контейнеров Azure, изменен до 5 лет.</span><span class="sxs-lookup"><span data-stu-id="8b368-2133">Changed aks created SPNs to be valid for 5 years</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2134">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2134">Appservice</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `assign-identity`
[BREAKING CHANGE]: Removed `assign-identity`
* <span data-ttu-id="8b368-2136">Исправлено неперехватываемое исключение для несуществующих планов веб-приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-2136">Fixed uncaught exception for nonexistant webapp plans</span></span>

### <a name="batchai"></a><span data-ttu-id="8b368-2137">Batch AI</span><span class="sxs-lookup"><span data-stu-id="8b368-2137">BatchAI</span></span>

* <span data-ttu-id="8b368-2138">Добавлена поддержка API 2018-03-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-2138">Added support for 2018-03-01 API</span></span>

  - <span data-ttu-id="8b368-2139">Подключение на уровне задания.</span><span class="sxs-lookup"><span data-stu-id="8b368-2139">Job level mounting</span></span>
  - <span data-ttu-id="8b368-2140">Переменные среды со значениями секретов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2140">Environment variables with secret values</span></span>
  - <span data-ttu-id="8b368-2141">Параметры счетчиков производительности</span><span class="sxs-lookup"><span data-stu-id="8b368-2141">Performance counters settings</span></span>
  - <span data-ttu-id="8b368-2142">Предоставление информации о сегменте пути конкретного задания.</span><span class="sxs-lookup"><span data-stu-id="8b368-2142">Reporting of job specific path segment</span></span>
  - <span data-ttu-id="8b368-2143">Поддержка вложенных папок в API списка файлов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2143">Support for subfolders in list files api</span></span>
  - <span data-ttu-id="8b368-2144">Предоставление информации об использовании и ограничениях.</span><span class="sxs-lookup"><span data-stu-id="8b368-2144">Usage and limits reporting</span></span>
  - <span data-ttu-id="8b368-2145">Возможность указать тип кэширования для NFS-серверов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2145">Allow to specify caching type for NFS servers</span></span>
  - <span data-ttu-id="8b368-2146">Поддержка пользовательских образов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2146">Support for custom images</span></span>
  - <span data-ttu-id="8b368-2147">Добавлена поддержка инструментария pyTorch.</span><span class="sxs-lookup"><span data-stu-id="8b368-2147">Added pyTorch toolkit support</span></span>

* <span data-ttu-id="8b368-2148">Добавлена команда `job wait`, позволяющая дождаться завершения задания и сообщить код выхода задания.</span><span class="sxs-lookup"><span data-stu-id="8b368-2148">Added `job wait` command which allows to wait for the job completion and reports job exit code</span></span>
* <span data-ttu-id="8b368-2149">Добавлена команда `usage show`, позволяющая получить актуальные сведения об использовании и ограничениях ресурсов Batch AI для различных регионов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2149">Added `usage show` command to list current Batch AI resources usage and limits for different regions</span></span>
* <span data-ttu-id="8b368-2150">Поддержка национальных облаков.</span><span class="sxs-lookup"><span data-stu-id="8b368-2150">National clouds are supported</span></span>
* <span data-ttu-id="8b368-2151">Для заданий добавлены аргументы командной строки, которые позволяют подключать файловые системы на уровне заданий. Эти же действия можно выполнять в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="8b368-2151">Added job command line arguments to mount filesystems on the job level in addition to config files</span></span>
* <span data-ttu-id="8b368-2152">Добавлены дополнительные параметры для настройки кластеров: приоритет виртуальной машины, подсеть, исходное число узлов для кластеров с автоматическим масштабированием, выбор пользовательского образа.</span><span class="sxs-lookup"><span data-stu-id="8b368-2152">Added more options to customize clusters - vm priority, subnet, initial nodes count for auto-scale clusters, specifying custom image</span></span>
* <span data-ttu-id="8b368-2153">Добавлен параметр командной строки, который позволяет указать тип кэширования для управляемой файловой системы NFS службы Batch AI.</span><span class="sxs-lookup"><span data-stu-id="8b368-2153">Added command line option to specify caching type for Batch AI managed NFS</span></span>
* <span data-ttu-id="8b368-2154">Упрощена процедура выбора подключаемой файловой системы в файлах конфигурации.</span><span class="sxs-lookup"><span data-stu-id="8b368-2154">Simplified specifying mount filesystem in config files.</span></span> <span data-ttu-id="8b368-2155">Теперь учетные данные для общего файлового ресурса Azure и контейнеров BLOB-объектов Azure указывать не нужно: CLI получит отсутствующие учетные данные с помощью ключа учетной записи хранения, указанного в параметрах командной строки, или переменной среды либо запросит ключ из службы хранилища Azure (если учетная запись хранения относится к текущей подписке).</span><span class="sxs-lookup"><span data-stu-id="8b368-2155">Now you can omit credentials for Azure File Share and Azure Blob Containers - CLI will populate missing credentials using storage account key provided via command line parameters or specified via environment variable or will query the key from Azure Storage (if the storage account belongs to the current subscription)</span></span>
* <span data-ttu-id="8b368-2156">Команда задания потоковой передачи файлов теперь автоматически завершается при завершении задания (успешное выполнение, сбой, прерывание или удаление).</span><span class="sxs-lookup"><span data-stu-id="8b368-2156">Job file stream command now auto-completes when the job is completed (succeeded, failed, terminated or deleted)</span></span>
* <span data-ttu-id="8b368-2157">Улучшены выходные данные `table` для операций `show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2157">Improved `table` output for `show` operations</span></span>
* <span data-ttu-id="8b368-2158">Добавлен параметр `--use-auto-storage` для создания кластера.</span><span class="sxs-lookup"><span data-stu-id="8b368-2158">Added `--use-auto-storage` option for cluster creation.</span></span> <span data-ttu-id="8b368-2159">Этот параметр упрощает управление учетными записями хранения, а также подключение общего файлового ресурса Azure и контейнеров BLOB-объектов Azure к кластеру.</span><span class="sxs-lookup"><span data-stu-id="8b368-2159">This option make it simpler to manage storage accounts and mount Azure File Share and Azure Blob Containers to clusters</span></span>
* <span data-ttu-id="8b368-2160">Добавлен параметр `--generate-ssh-keys` для команд `cluster create` и `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2160">Added `--generate-ssh-keys` option to `cluster create` and `file-server create`</span></span>
* <span data-ttu-id="8b368-2161">Добавлена возможность запустить задачу настройки узла через командную строку.</span><span class="sxs-lookup"><span data-stu-id="8b368-2161">Added ability to provide node setup task via command line</span></span>
* <span data-ttu-id="8b368-2162">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `job stream-file` и `job list-files` перемещены в группу `job file`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2162">[BREAKING CHANGE] Moved `job stream-file` and `job list-files` commands under `job file` group</span></span>
* <span data-ttu-id="8b368-2163">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В команде `file-server create` параметр `--admin-user-name` переименован в `--user-name` для согласованности с командой `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2163">[BREAKING CHANGE] Renamed `--admin-user-name` to `--user-name` in `file-server create` command to be consistent with `cluster create` command</span></span>

### <a name="billing"></a><span data-ttu-id="8b368-2164">Выставление счетов</span><span class="sxs-lookup"><span data-stu-id="8b368-2164">Billing</span></span>

* <span data-ttu-id="8b368-2165">Добавлены команды для учетной записи регистрации.</span><span class="sxs-lookup"><span data-stu-id="8b368-2165">Added enrollment account commands</span></span>

### <a name="consumption"></a><span data-ttu-id="8b368-2166">Потребление</span><span class="sxs-lookup"><span data-stu-id="8b368-2166">Consumption</span></span>

* <span data-ttu-id="8b368-2167">Добавлены команды `marketplace`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2167">Added `marketplace` commands</span></span>
* <span data-ttu-id="8b368-2168">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations summaries` переименована в `reservation summary`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2168">[BREAKING CHANGE] Renamed `reservations summaries` to `reservation summary`</span></span>
* <span data-ttu-id="8b368-2169">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `reservations details` переименована в `reservation detail`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2169">[BREAKING CHANGE] Renamed `reservations details` to `reservation detail`</span></span>
* <span data-ttu-id="8b368-2170">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation` удалены короткие параметры `--reservation-order-id` и `--reservation-id`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2170">[BREAKING CHANGE] Removed `--reservation-order-id` and `--reservation-id` short options for `reservation` commands</span></span>
* <span data-ttu-id="8b368-2171">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `reservation summary` удалены короткие параметры `--grain`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2171">[BREAKING CHANGE] Removed `--grain` short options for `reservation summary` commands</span></span>
* <span data-ttu-id="8b368-2172">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] В командах `pricesheet` удалены короткие параметры `--include-meter-details`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2172">[BREAKING CHANGE] Removed `--include-meter-details` short options for `pricesheet` commands</span></span>

### <a name="container"></a><span data-ttu-id="8b368-2173">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-2173">Container</span></span>

* <span data-ttu-id="8b368-2174">Добавлены параметры подключения тома репозитория Git: `--gitrepo-url`, `--gitrepo-dir`, `--gitrepo-revision` и `--gitrepo-mount-path`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2174">Added git repo volume mount parameters `--gitrepo-url` `--gitrepo-dir` `--gitrepo-revision` and `--gitrepo-mount-path`</span></span>
* <span data-ttu-id="8b368-2175">Исправлена ошибка [#5926](https://github.com/Azure/azure-cli/issues/5926): команда `az container exec` возвращает ошибку, когда указан параметр --container-name.</span><span class="sxs-lookup"><span data-stu-id="8b368-2175">Fixed [#5926](https://github.com/Azure/azure-cli/issues/5926): `az container exec` failing when --container-name specified</span></span>

### <a name="extension"></a><span data-ttu-id="8b368-2176">Расширение</span><span class="sxs-lookup"><span data-stu-id="8b368-2176">Extension</span></span>

* <span data-ttu-id="8b368-2177">Сообщение о проверке распространения перенесено на уровень отладки.</span><span class="sxs-lookup"><span data-stu-id="8b368-2177">Changed distribution check message to be debug-level</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-2178">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-2178">Interactive</span></span>

* <span data-ttu-id="8b368-2179">Если команда не распознана, выполнение прерывается.</span><span class="sxs-lookup"><span data-stu-id="8b368-2179">Changed to stop completions upon unrecognized commands</span></span>
* <span data-ttu-id="8b368-2180">Добавлены перехватчики событий, которые используются до и после создания поддерева команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-2180">Added event hooks before and after command subtree is created</span></span>
* <span data-ttu-id="8b368-2181">Добавлены сведения о выполнении для параметров `--ids`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2181">Added completion for `--ids` parameters</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2182">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2182">Network</span></span>

* <span data-ttu-id="8b368-2183">Исправлена ошибка [#5936](https://github.com/Azure/azure-cli/issues/5936): не задаются теги `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2183">Fixed [#5936](https://github.com/Azure/azure-cli/issues/5936): `application-gateway create` tags could not bet set</span></span>
* <span data-ttu-id="8b368-2184">Добавлен аргумент `--auth-certs`, который позволяет подключать сертификаты аутентификации для `application-gateway http-settings [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2184">Added argument `--auth-certs` to attach authentication certificates for `application-gateway http-settings [create|update]`.</span></span> <span data-ttu-id="8b368-2185">[#4910](https://github.com/Azure/azure-cli/issues/4910).</span><span class="sxs-lookup"><span data-stu-id="8b368-2185">[#4910](https://github.com/Azure/azure-cli/issues/4910)</span></span>
* <span data-ttu-id="8b368-2186">Добавлены команды `ddos-protection` для создания планов защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="8b368-2186">Added `ddos-protection` commands to create DDoS protection plans</span></span>
* <span data-ttu-id="8b368-2187">В команду `vnet [create|update]` добавлена поддержка `--ddos-protection-plan` для связи виртуальной сети с планом защиты от атак DDoS.</span><span class="sxs-lookup"><span data-stu-id="8b368-2187">Added support for `--ddos-protection-plan` to `vnet [create|update]` to associate a VNet to a DDoS protection plan</span></span>
* <span data-ttu-id="8b368-2188">Исправлена ошибка с флагом `--disable-bgp-route-propagation` в команде `network route-table [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2188">Fixed issue with `--disable-bgp-route-propagation` flag in `network route-table [create|update]`</span></span>
* <span data-ttu-id="8b368-2189">Удалены фиктивные аргументы `--public-ip-address-type` и `--subnet-type` для команды `network lb [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2189">Removed dummy arguments `--public-ip-address-type` and `--subnet-type` for `network lb [create|update]`</span></span>
* <span data-ttu-id="8b368-2190">В `network dns zone [import|export]` и `network dns record-set txt add-record` добавлена поддержка записей типа TXT с escape-последовательностями RFC 1035.</span><span class="sxs-lookup"><span data-stu-id="8b368-2190">Added support for TXT records with RFC 1035 escape sequences to `network dns zone [import|export]` and `network dns record-set txt add-record`</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-2191">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-2191">Profile</span></span>

* <span data-ttu-id="8b368-2192">Добавлена поддержка классических учетных записей Azure для команды `account list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2192">Added support for Azure Classic accounts in `account list`</span></span>
* <span data-ttu-id="8b368-2193">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалены аргументы `--msi` & `--msi-port`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2193">[BREAKING CHANGE] Removed `--msi` & `--msi-port` arguments</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-2194">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="8b368-2194">RDBMS</span></span>

* <span data-ttu-id="8b368-2195">Добавлена команда `georestore`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2195">Added `georestore` command</span></span>
* <span data-ttu-id="8b368-2196">Из команды `create` исключено ограничение на размер хранилища.</span><span class="sxs-lookup"><span data-stu-id="8b368-2196">Removed storage size restriction from `create` command</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-2197">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-2197">Resource</span></span>

* <span data-ttu-id="8b368-2198">Добавлена поддержка параметра `--metadata` в команде `policy definition create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2198">Added support for `--metadata` to `policy definition create`</span></span>
* <span data-ttu-id="8b368-2199">Добавлена поддержка `--metadata`, `--set`, `--add` и `--remove` для команды `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2199">Added support for `--metadata`, `--set`, `--add`, `--remove` to `policy definition update`</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-2200">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-2200">SQL</span></span>

* <span data-ttu-id="8b368-2201">Добавлены команды `sql elastic-pool op list` и `sql elastic-pool op cancel`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2201">Added `sql elastic-pool op list` and `sql elastic-pool op cancel`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2202">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2202">Storage</span></span>

* <span data-ttu-id="8b368-2203">Улучшены сообщения об ошибках для строк подключения, имеющих неправильный формат.</span><span class="sxs-lookup"><span data-stu-id="8b368-2203">Improved error messages for malformed connection strings</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2204">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2204">VM</span></span>

* <span data-ttu-id="8b368-2205">В команде `vmss create` добавлена возможность настроить для платформы количество доменов сбоя.</span><span class="sxs-lookup"><span data-stu-id="8b368-2205">Added support to configure platform fault domain count to `vmss create`</span></span>
* <span data-ttu-id="8b368-2206">Команда `vmss create` теперь по умолчанию использует стандартную балансировку нагрузки для зональных и больших масштабируемых наборов, а также масштабируемых наборов, в которых отключена одна группа размещения.</span><span class="sxs-lookup"><span data-stu-id="8b368-2206">Changed `vmss create` to default to Standard LB for zonal, large or single-placement-group disabled scale-set</span></span>
* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
[BREAKING CHANGE]: Removed `vm assign-identity`, `vm remove-identity and `vm format-secret\`
* <span data-ttu-id="8b368-2208">Добавлена поддержка SKU общедоступного IP-адреса для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2208">Added support for Public-IP SKU to `vm create`</span></span>
* <span data-ttu-id="8b368-2209">В команду `vm secret format` добавлены аргументы `--keyvault` и `--resource-group` для тех случаев, когда команда не может разрешить идентификатор хранилища.</span><span class="sxs-lookup"><span data-stu-id="8b368-2209">Added `--keyvault` and `--resource-group` arguments to `vm secret format` to support scenarios where the command is unable to resolve the vault ID.</span></span> <span data-ttu-id="8b368-2210">[#5718](https://github.com/Azure/azure-cli/issues/5718).</span><span class="sxs-lookup"><span data-stu-id="8b368-2210">[#5718](https://github.com/Azure/azure-cli/issues/5718)</span></span>
* <span data-ttu-id="8b368-2211">Улучшены сообщения об ошибках для команды `[vm|vmss create]`, когда расположение группы ресурсов не поддерживает зоны.</span><span class="sxs-lookup"><span data-stu-id="8b368-2211">Better errors for `[vm|vmss create]` when a resource group's location has no zone support</span></span>


## <a name="march-27-2018"></a><span data-ttu-id="8b368-2212">27 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2212">March 27, 2018</span></span>

<span data-ttu-id="8b368-2213">Версия 2.0.30</span><span class="sxs-lookup"><span data-stu-id="8b368-2213">Version 2.0.30</span></span>

### <a name="core"></a><span data-ttu-id="8b368-2214">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-2214">Core</span></span>

* <span data-ttu-id="8b368-2215">Отображение сообщения для расширений, которые отмечены в справке как предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="8b368-2215">Show message for extensions marked as preview in help</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2216">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2216">ACS</span></span>

* <span data-ttu-id="8b368-2217">Устранена ошибка с проверкой SSL-сертификата для `aks install-cli` в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="8b368-2217">Fix SSL certificate verification error for `aks install-cli` in Cloud Shell</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2218">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2218">Appservice</span></span>

* <span data-ttu-id="8b368-2219">Добавлена поддержка только протокола HTTPS для `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2219">Added HTTPS-only support to `webapp update`</span></span>
* <span data-ttu-id="8b368-2220">Добавлена поддержка слотов для `az webapp identity [assign|show]` и `az functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2220">Added support for slots to `az webapp identity [assign|show]` and `az functionapp identity [assign|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="8b368-2221">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="8b368-2221">Backup</span></span>

* <span data-ttu-id="8b368-2222">Добавлена новая команда `az backup protection isenabled-for-vm`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2222">Added new command `az backup protection isenabled-for-vm`.</span></span> <span data-ttu-id="8b368-2223">Эта команда используется для проверки резервного копирования виртуальной машины в любое хранилище в подписке.</span><span class="sxs-lookup"><span data-stu-id="8b368-2223">This command can be used to check if a VM is backed up by any vault in the subscription</span></span>
* <span data-ttu-id="8b368-2224">Включены идентификаторы объектов Azure для параметров `--resource-group` и `--vault-name` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="8b368-2224">Enabled Azure object IDs for `--resource-group` and `--vault-name` parameters for the following commands:</span></span>
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
* <span data-ttu-id="8b368-2225">Изменены параметры `--name` для поддержки формата вывода команд `backup ... show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2225">Changed `--name` parameters to accept the output format from `backup ... show` commands</span></span>

### <a name="container"></a><span data-ttu-id="8b368-2226">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-2226">Container</span></span>

* <span data-ttu-id="8b368-2227">Добавлена команда `container exec`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2227">Added `container exec` command.</span></span> <span data-ttu-id="8b368-2228">Выполнение команды в контейнере для выполняющейся группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2228">Executes commands in a container for a running container group</span></span>
* <span data-ttu-id="8b368-2229">Разрешение выходной таблице создавать и обновлять группу контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2229">Allow table output for creating and updating a container group</span></span>

### <a name="extension"></a><span data-ttu-id="8b368-2230">Расширение</span><span class="sxs-lookup"><span data-stu-id="8b368-2230">Extension</span></span>

* <span data-ttu-id="8b368-2231">Добавлено сообщение для `extension add`, если расширение доступно в режиме предварительной версии.</span><span class="sxs-lookup"><span data-stu-id="8b368-2231">Added message for `extension add` if extension is in preview</span></span>
* <span data-ttu-id="8b368-2232">Изменен параметр `extension list-available` для отображения всех данных расширения с использованием `--show-details`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2232">Changed `extension list-available` to show full extension data with `--show-details`</span></span>
* <span data-ttu-id="8b368-2233">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменена команда `extension list-available` для отображения упрощенных данных расширения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-2233">[BREAKING CHANGE] Changed `extension list-available` to show simplified extension data by default</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-2234">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-2234">Interactive</span></span>

* <span data-ttu-id="8b368-2235">Изменены операции завершения, активируемые сразу после завершения загрузки таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-2235">Changed completions to activate as soon as command table loading is done</span></span>
* <span data-ttu-id="8b368-2236">Исправлена ошибка с использованием параметра `--style`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2236">Fixed bug with using `--style` parameter</span></span>
* <span data-ttu-id="8b368-2237">Отсутствующий интерактивный лексический анализатор создается после дампа таблицы команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-2237">Interactive lexer instantiated after command table dump if missing</span></span>
* <span data-ttu-id="8b368-2238">Улучшена поддержка средства заполнения.</span><span class="sxs-lookup"><span data-stu-id="8b368-2238">Improved completer support</span></span>

### <a name="lab"></a><span data-ttu-id="8b368-2239">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="8b368-2239">Lab</span></span>

* <span data-ttu-id="8b368-2240">Исправлены ошибки с командой `create environment`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2240">Fixed bugs with `create environment` command</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-2241">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-2241">Monitor</span></span>

* <span data-ttu-id="8b368-2242">Добавлена поддержка аргументов `--top`, `--orderby` и `--namespace` для `metrics list` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="8b368-2242">Added support for `--top`, `--orderby` and `--namespace` to `metrics list` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>
* <span data-ttu-id="8b368-2243">Исправлена ошибка [#4529](https://github.com/Azure/azure-cli/issues/5785). Команда `metrics list` принимает разделенный пробелами список метрик для извлечения.</span><span class="sxs-lookup"><span data-stu-id="8b368-2243">Fixed [#4529](https://github.com/Azure/azure-cli/issues/5785): `metrics list` Accepts a space-separated list of metrics to retrieve</span></span>
* <span data-ttu-id="8b368-2244">Добавлена поддержка `--namespace` для `metrics list-definitions` ([№ 5785](https://github.com/Azure/azure-cli/issues/5785)).</span><span class="sxs-lookup"><span data-stu-id="8b368-2244">Added support for `--namespace` to `metrics list-definitions` [#5785](https://github.com/Azure/azure-cli/issues/5785)</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2245">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2245">Network</span></span>

* <span data-ttu-id="8b368-2246">Добавлена поддержка Частных зон DNS.</span><span class="sxs-lookup"><span data-stu-id="8b368-2246">Added support for Private DNS zones</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-2247">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-2247">Profile</span></span>

* <span data-ttu-id="8b368-2248">Добавлено предупреждение для `--identity-port` и `--msi-port` в `login`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2248">Added warning for `--identity-port` and `--msi-port` to `login`</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-2249">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="8b368-2249">RDBMS</span></span>

* <span data-ttu-id="8b368-2250">Добавлена общедоступная версия 2017-12-01 бизнес-модели API.</span><span class="sxs-lookup"><span data-stu-id="8b368-2250">Added business model GA API version 2017-12-01</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-2251">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-2251">Resource</span></span>

* [КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]: Changed `provider operation [list|show]` to not require `--api-version`
[BREAKING CHANGE]: Changed `provider operation [list|show]` to not require `--api-version`

### <a name="role"></a><span data-ttu-id="8b368-2253">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-2253">Role</span></span>

* <span data-ttu-id="8b368-2254">Добавлена поддержка конфигурации требуемого уровня доступа и собственных клиентов для `az ad app create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2254">Added support for required access configurations and native clients to `az ad app create`</span></span>
* <span data-ttu-id="8b368-2255">Изменены команды `rbac`, чтобы возвращать не более 1000 идентификаторов в разрешении объекта.</span><span class="sxs-lookup"><span data-stu-id="8b368-2255">Changed `rbac` commands to return less than 1000 IDs on object resolution</span></span>
* <span data-ttu-id="8b368-2256">Добавлены команды `ad sp credential [reset|list|delete]` для управления учетными данными.</span><span class="sxs-lookup"><span data-stu-id="8b368-2256">Added credential management commands `ad sp credential [reset|list|delete]`</span></span>
* <span data-ttu-id="8b368-2257">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр properties из выходных данных `az role assignment [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2257">[BREAKING CHANGE] Removed 'properties' from `az role assignment [list|show]` output</span></span>
* <span data-ttu-id="8b368-2258">Добавлена поддержка разрешений `dataActions` и `notDataActions` для `role definition`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2258">Added support for `dataActions` and `notDataActions` permissions to `role definition`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2259">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2259">Storage</span></span>

* <span data-ttu-id="8b368-2260">Исправлена проблема с отправкой файла размером от 195 до 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="8b368-2260">Fixed issue when uploading file with size between 195GB and 200GB</span></span>
* <span data-ttu-id="8b368-2261">Исправлена ошибка [#4049](https://github.com/Azure/azure-cli/issues/4049). Проблемы игнорирования параметров условия при отправке добавочного большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="8b368-2261">Fixed [#4049](https://github.com/Azure/azure-cli/issues/4049): Problems with append blob uploads ignoring condition parameters</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2262">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2262">VM</span></span>

* <span data-ttu-id="8b368-2263">Добавлено предупреждение `vmss create` для предстоящих критически важных изменений для наборов из 100 и более экземпляров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2263">Added warning to `vmss create` for upcoming breaking changes for sets with 100+ instances</span></span>
* <span data-ttu-id="8b368-2264">Добавлена поддержка устойчивости зон для `vm [snapshot|image]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2264">Added zone resilient support to `vm [snapshot|image]`</span></span>
* <span data-ttu-id="8b368-2265">Изменено представление экземпляра диска для улучшения отчета о состоянии шифрования.</span><span class="sxs-lookup"><span data-stu-id="8b368-2265">Changed disk instance view to report better encryption status</span></span>
* <span data-ttu-id="8b368-2266">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.]`vm extension delete` Изменена команда, которая больше не возвращает выходные данные.</span><span class="sxs-lookup"><span data-stu-id="8b368-2266">[BREAKING CHANGE] Changed `vm extension delete` to no longer return output</span></span>

## <a name="march-13-2018"></a><span data-ttu-id="8b368-2267">13 марта 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2267">March 13, 2018</span></span>

<span data-ttu-id="8b368-2268">Версия 2.0.29</span><span class="sxs-lookup"><span data-stu-id="8b368-2268">Version 2.0.29</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-2269">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-2269">ACR</span></span>

* <span data-ttu-id="8b368-2270">Добавлена поддержка параметра `--image` для `repository delete`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2270">Added support for `--image` parameter to `repository delete`</span></span>
* <span data-ttu-id="8b368-2271">Параметры `--manifest` и `--tag` команды `repository delete` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="8b368-2271">Deprecated `--manifest` and `--tag` parameters of the `repository delete` command</span></span>
* <span data-ttu-id="8b368-2272">Добавлена команда `repository untag` для удаления тега без удаления данных.</span><span class="sxs-lookup"><span data-stu-id="8b368-2272">Added `repository untag` command to remove a tag without deleting data</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2273">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2273">ACS</span></span>

* <span data-ttu-id="8b368-2274">Добавлена команда `aks upgrade-connector` для обновления существующего соединителя.</span><span class="sxs-lookup"><span data-stu-id="8b368-2274">Added `aks upgrade-connector` command to upgrade an existing connector</span></span>
* <span data-ttu-id="8b368-2275">Изменены файлы конфигурации `kubectl`. Теперь используется более разборчивый стиль YAML с разбивкой на блоки.</span><span class="sxs-lookup"><span data-stu-id="8b368-2275">Changed `kubectl` config files to use a more readable block-style YAML</span></span>

### <a name="advisor"></a><span data-ttu-id="8b368-2276">Помощник</span><span class="sxs-lookup"><span data-stu-id="8b368-2276">Advisor</span></span>

* <span data-ttu-id="8b368-2277">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration get` переименована в `advisor configuration list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2277">[BREAKING CHANGE] Renamed `advisor configuration get` to `advisor configuration list`</span></span>
* <span data-ttu-id="8b368-2278">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `advisor configuration set` переименована в `advisor configuration update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2278">[BREAKING CHANGE] Renamed `advisor configuration set` to `advisor configuration update`</span></span>
* <span data-ttu-id="8b368-2279">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `advisor recommendation generate`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2279">[BREAKING CHANGE] Removed `advisor recommendation generate`</span></span>
* <span data-ttu-id="8b368-2280">Добавлен параметр `--refresh` для команды `advisor recommendation list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2280">Added `--refresh` parameter to `advisor recommendation list`</span></span>
* <span data-ttu-id="8b368-2281">Добавлена команда `advisor recommendation show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2281">Added `advisor recommendation show` command</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2282">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2282">Appservice</span></span>

* <span data-ttu-id="8b368-2283">Команда `[webapp|functionapp] assign-identity` отмечена как нерекомендуемая.</span><span class="sxs-lookup"><span data-stu-id="8b368-2283">Deprecated `[webapp|functionapp] assign-identity`</span></span>
* <span data-ttu-id="8b368-2284">Добавлены команды управляемого удостоверения `webapp identity [assign|show]` и `functionapp identity [assign|show]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2284">Added managed identity commands `webapp identity [assign|show]` and `functionapp identity [assign|show]`</span></span>

### <a name="eventhubs"></a><span data-ttu-id="8b368-2285">Концентраторы событий</span><span class="sxs-lookup"><span data-stu-id="8b368-2285">Eventhubs</span></span>

* <span data-ttu-id="8b368-2286">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="8b368-2286">Initial release</span></span>

### <a name="extension"></a><span data-ttu-id="8b368-2287">Расширение</span><span class="sxs-lookup"><span data-stu-id="8b368-2287">Extension</span></span>

* <span data-ttu-id="8b368-2288">Добавлена проверка, позволяющая предупредить пользователя, если используемый дистрибутив отличается от хранящегося в исходном файле пакета, так как это может привести к возникновению ошибок.</span><span class="sxs-lookup"><span data-stu-id="8b368-2288">Added check to warn user if used distro is different then the one stored in package source file, as this may lead into errors</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-2289">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-2289">Interactive</span></span>

* <span data-ttu-id="8b368-2290">Исправлена ошибка [#5625](https://github.com/Azure/azure-cli/issues/5625). Теперь записи журнала сохраняются в разных сеансах.</span><span class="sxs-lookup"><span data-stu-id="8b368-2290">Fixed [#5625](https://github.com/Azure/azure-cli/issues/5625): Persist history across different sessions</span></span>
* <span data-ttu-id="8b368-2291">Исправлена ошибка [#3016](https://github.com/Azure/azure-cli/issues/3016). При использовании области не создавались записи журнала.</span><span class="sxs-lookup"><span data-stu-id="8b368-2291">Fixed [#3016](https://github.com/Azure/azure-cli/issues/3016): History not recorded while in scope</span></span>
* <span data-ttu-id="8b368-2292">Исправлена ошибка [#5688](https://github.com/Azure/azure-cli/issues/5688). Если при загрузке таблицы команд возникало исключение, варианты автозаполнения не отображались.</span><span class="sxs-lookup"><span data-stu-id="8b368-2292">Fixed [#5688](https://github.com/Azure/azure-cli/issues/5688): Completions did not appear if command table loading encountered an exception</span></span>
* <span data-ttu-id="8b368-2293">Исправлен индикатор хода выполнения для длительных операций.</span><span class="sxs-lookup"><span data-stu-id="8b368-2293">Fixed progress meter for long running operations</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-2294">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-2294">Monitor</span></span>

* <span data-ttu-id="8b368-2295">Команды `monitor autoscale-settings` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="8b368-2295">Deprecated the `monitor autoscale-settings` commands</span></span>
* <span data-ttu-id="8b368-2296">Добавлены команды `monitor autoscale`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2296">Added `monitor autoscale` commands</span></span>
* <span data-ttu-id="8b368-2297">Добавлены команды `monitor autoscale profile`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2297">Added `monitor autoscale profile` commands</span></span>
* <span data-ttu-id="8b368-2298">Добавлены команды `monitor autoscale rule`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2298">Added `monitor autoscale rule` commands</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2299">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2299">Network</span></span>

* <span data-ttu-id="8b368-2300">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удален параметр `--tags` из `route-filter rule create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2300">[BREAKING CHANGE] Removed `--tags` parameter from  `route-filter rule create`</span></span>
* <span data-ttu-id="8b368-2301">Удалены некоторые ошибочные значения по умолчанию для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="8b368-2301">Removed some erroneous default values for the following commands:</span></span>
  * `network express-route update`
  * `network nsg rule update`
  * `network public-ip update`
  * `traffic-manager profile update`
  * `network vnet-gateway update`
* <span data-ttu-id="8b368-2302">Добавлены команды `network watcher connection-monitor`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2302">Added `network watcher connection-monitor` commands\`</span></span>
* <span data-ttu-id="8b368-2303">Добавлены параметры `--vnet` и `--subnet` для `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2303">Added `--vnet` and `--subnet` parameters to `network watcher show-topology`</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-2304">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-2304">Profile</span></span>

* <span data-ttu-id="8b368-2305">Параметр `--msi` для `az login` отмечен как нерекомендуемый.</span><span class="sxs-lookup"><span data-stu-id="8b368-2305">Deprecated `--msi` parameter for `az login`</span></span>
* <span data-ttu-id="8b368-2306">Добавлен параметр `--identity` для `az login`. Он заменяет `--msi`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2306">Added `--identity` parameter for `az login` to replace `--msi`</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-2307">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="8b368-2307">RDBMS</span></span>

* <span data-ttu-id="8b368-2308">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Внесены изменения для использования предварительной версии API 2017-12-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-2308">[PREVIEW] Changed to use the API 2017-12-01-preview</span></span>

### <a name="service-bus"></a><span data-ttu-id="8b368-2309">Служебная шина</span><span class="sxs-lookup"><span data-stu-id="8b368-2309">Service Bus</span></span>

* <span data-ttu-id="8b368-2310">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="8b368-2310">Initial release</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2311">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2311">Storage</span></span>

* <span data-ttu-id="8b368-2312">Исправлена ошибка [#4971](https://github.com/Azure/azure-cli/issues/4971): теперь `storage blob copy` поддерживает другие облака Azure.</span><span class="sxs-lookup"><span data-stu-id="8b368-2312">Fixed [#4971](https://github.com/Azure/azure-cli/issues/4971): `storage blob copy` now supports other Azure clouds</span></span>
* <span data-ttu-id="8b368-2313">Исправлена ошибка [#5286](https://github.com/Azure/azure-cli/issues/5286). При пакетном выполнении команд `storage blob [delete-batch|download-batch|upload-batch]` больше не отображается сообщение об ошибке в предусловии.</span><span class="sxs-lookup"><span data-stu-id="8b368-2313">Fixed [#5286](https://github.com/Azure/azure-cli/issues/5286): Batch commands `storage blob [delete-batch|download-batch|upload-batch]` no longer throw an error upon precondition failures</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2314">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2314">VM</span></span>

* <span data-ttu-id="8b368-2315">В `[vm|vmss] create` добавлена поддержка присоединения неуправляемых дисков данных и настройки кэширования.</span><span class="sxs-lookup"><span data-stu-id="8b368-2315">Added support to `[vm|vmss] create` to attach unmanaged data disks and configure caching</span></span>
* <span data-ttu-id="8b368-2316">`[vm|vmss] assign-identity` и `[vm|vmss] remove-identity` отмечены как нерекомендуемые.</span><span class="sxs-lookup"><span data-stu-id="8b368-2316">Deprecated `[vm|vmss] assign-identity` and `[vm|vmss] remove-identity`</span></span>
* <span data-ttu-id="8b368-2317">Вместо нерекомендуемых команд добавлены команды `vm identity [assign|remove|show]` и `vmss identity [assign|remove|show]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2317">Added `vm identity [assign|remove|show]` and `vmss identity [assign|remove|show]` commands to replace deprecated commands</span></span>
* <span data-ttu-id="8b368-2318">Для приоритета `vmss create` по умолчанию установлено значение None.</span><span class="sxs-lookup"><span data-stu-id="8b368-2318">Changed default priority in `vmss create` to None</span></span>

## <a name="february-27-2018"></a><span data-ttu-id="8b368-2319">27 февраля 2018 г</span><span class="sxs-lookup"><span data-stu-id="8b368-2319">February 27, 2018</span></span>

<span data-ttu-id="8b368-2320">Версия 2.0.28</span><span class="sxs-lookup"><span data-stu-id="8b368-2320">Version 2.0.28</span></span>

### <a name="core"></a><span data-ttu-id="8b368-2321">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-2321">Core</span></span>

* <span data-ttu-id="8b368-2322">Исправлена ошибка [#5184](https://github.com/Azure/azure-cli/issues/5184). Проблема с установкой Homebrew.</span><span class="sxs-lookup"><span data-stu-id="8b368-2322">Fixed [#5184](https://github.com/Azure/azure-cli/issues/5184): Homebrew install issue</span></span>
* <span data-ttu-id="8b368-2323">Добавлена поддержка телеметрии расширения с применением пользовательских ключей.</span><span class="sxs-lookup"><span data-stu-id="8b368-2323">Added support for extension telemetry with custom keys</span></span>
* <span data-ttu-id="8b368-2324">Добавлена функция ведения журнала HTTP в `--debug`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2324">Added HTTP logging to `--debug`</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2325">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2325">ACS</span></span>

* <span data-ttu-id="8b368-2326">Изменено для использования диаграмм Helm `virtual-kubelet-for-aks` для `aks install-connector` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-2326">Changed to use the the `virtual-kubelet-for-aks` Helm chart for `aks install-connector` by default</span></span>
* <span data-ttu-id="8b368-2327">Исправлена ошибка с недостаточными разрешениями субъектов-служб на создание групп контейнеров ACI.</span><span class="sxs-lookup"><span data-stu-id="8b368-2327">Fixed issue: Insuffient permission for service principals to create ACI container group issue</span></span>
* <span data-ttu-id="8b368-2328">Добавлены параметры `--aci-container-group`, `--location` и `--image-tag` для `aks install-connector`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2328">Added `--aci-container-group`, `--location`, and `--image-tag` parameters to `aks install-connector`</span></span>
* <span data-ttu-id="8b368-2329">Удалено уведомление об устаревании из `aks get-versions`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2329">Removed deprecation notice from `aks get-versions`</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2330">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2330">Appservice</span></span>

* <span data-ttu-id="8b368-2331">Обновления для новой версии пакета SDK (azure-mgmt-web 0.35.0)</span><span class="sxs-lookup"><span data-stu-id="8b368-2331">Updates for new SDK version (azure-mgmt-web 0.35.0)</span></span>
* <span data-ttu-id="8b368-2332">Исправлена ошибка [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` указывалось как недопустимый номер SKU.</span><span class="sxs-lookup"><span data-stu-id="8b368-2332">Fixed [#5538](https://github.com/Azure/azure-cli/issues/5538): `Free` reported as invalid SKU</span></span>

### <a name="cognitive-services"></a><span data-ttu-id="8b368-2333">Cognitive Services</span><span class="sxs-lookup"><span data-stu-id="8b368-2333">Cognitive Services</span></span>

* <span data-ttu-id="8b368-2334">Обновлено уведомление при создании новой учетной записи Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="8b368-2334">Updated the 'notice' when creating a new Cognitive Services account</span></span>

### <a name="consumption"></a><span data-ttu-id="8b368-2335">Потребление</span><span class="sxs-lookup"><span data-stu-id="8b368-2335">Consumption</span></span>

* <span data-ttu-id="8b368-2336">Добавлены новые команды для резервирования API прейскуранта.</span><span class="sxs-lookup"><span data-stu-id="8b368-2336">Added new commands for pricesheet API</span></span>
* <span data-ttu-id="8b368-2337">Обновлены существующие форматы сведений об использовании и резервировании.</span><span class="sxs-lookup"><span data-stu-id="8b368-2337">Updated the existing Usage Details and Reservation Details formats</span></span>

### <a name="container"></a><span data-ttu-id="8b368-2338">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-2338">Container</span></span>

* <span data-ttu-id="8b368-2339">Добавлены аргументы `--secrets` и `--secrets-mount-path` в командах `container create` для использования секретов в ACI.</span><span class="sxs-lookup"><span data-stu-id="8b368-2339">Added `--secrets` and `--secrets-mount-path` arguments to `container create` to use secrets in ACI</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2340">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2340">Network</span></span>

* <span data-ttu-id="8b368-2341">Исправлена ошибка [#5559](https://github.com/Azure/azure-cli/issues/5559). Отсутствующий клиент в `network vnet-gateway vpn-client generate`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2341">Fixed [#5559](https://github.com/Azure/azure-cli/issues/5559): Missing client in `network vnet-gateway vpn-client generate`</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-2342">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-2342">Resource</span></span>

* <span data-ttu-id="8b368-2343">Изменено `group deployment export` для отображения частичного шаблона и ошибок при сбое.</span><span class="sxs-lookup"><span data-stu-id="8b368-2343">Changed `group deployment export` to display a partial template and errors on failure</span></span>

### <a name="role"></a><span data-ttu-id="8b368-2344">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-2344">Role</span></span>

* <span data-ttu-id="8b368-2345">Добавлено `role assignment list-changelogs` для включения аудита ролей субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-2345">Added `role assignment list-changelogs` to allow auditing of service principal roles</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-2346">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-2346">SQL</span></span>

* <span data-ttu-id="8b368-2347">Добавлена поддержка избыточности зон для создания и обновления баз данных и эластичных пулов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2347">Added zone redundancy support for databases and elastic pools on creation and update</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2348">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2348">Storage</span></span>

* <span data-ttu-id="8b368-2349">Включено определение пути назначения и префикса для `storage blob [upload-batch|download-batch]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2349">Enabled specifying destination-path/prefix for `storage blob [upload-batch|download-batch]`</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2350">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2350">VM</span></span>

* <span data-ttu-id="8b368-2351">Добавлена поддержка присоединения и отсоединения дисков на одном экземпляре VMSS.</span><span class="sxs-lookup"><span data-stu-id="8b368-2351">Added suport for attaching/detatching disks on a single VMSS instance</span></span>


## <a name="february-13-2018"></a><span data-ttu-id="8b368-2352">13 февраля 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2352">February 13, 2018</span></span>

<span data-ttu-id="8b368-2353">Версия 2.0.27</span><span class="sxs-lookup"><span data-stu-id="8b368-2353">Version 2.0.27</span></span>

### <a name="core"></a><span data-ttu-id="8b368-2354">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-2354">Core</span></span>

* <span data-ttu-id="8b368-2355">Изменен способ аутентификации при входе с помощью MSI: применяется ключ при использовании идентификатора подписки и имени.</span><span class="sxs-lookup"><span data-stu-id="8b368-2355">Changed authentication to key on both subscription ID and name on MSI login</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2356">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2356">ACS</span></span>

* <span data-ttu-id="8b368-2357">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Переименовано `aks get-versions` на `aks get-upgrades` для точности.</span><span class="sxs-lookup"><span data-stu-id="8b368-2357">[BREAKING CHANGE] Renamed `aks get-versions` to `aks get-upgrades` in the interest of accuracy</span></span>
* <span data-ttu-id="8b368-2358">Изменено `aks get-versions` для отображения версий Kubernetes, доступных для `aks create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2358">Changed `aks get-versions` to show Kubernetes versions available for `aks create`</span></span>
* <span data-ttu-id="8b368-2359">Изменены значения по умолчанию `aks create`, чтобы разрешить серверу выбирать версию Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="8b368-2359">Changed `aks create` defaults to letting the server choose the version of Kubernetes</span></span>
* <span data-ttu-id="8b368-2360">Обновлены справочные сообщения, связанные с субъектом-службой и создаваемые AKS.</span><span class="sxs-lookup"><span data-stu-id="8b368-2360">Updated help messages referring to the service principal generated by AKS</span></span>
* <span data-ttu-id="8b368-2361">Изменены стандартные размеры узла для `aks create` с уровня Standard\_D1\_v2 на уровень Standard\_DS1\_v2.</span><span class="sxs-lookup"><span data-stu-id="8b368-2361">Changed default node sizes for `aks create` from "Standard\_D1\_v2" to "Standard\_DS1\_v2"</span></span>
* <span data-ttu-id="8b368-2362">Улучшена надежность при поиске панели мониторинга для группы pod для `az aks browse`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2362">Improved reliability when locating the dashboard pod for `az aks browse`</span></span>
* <span data-ttu-id="8b368-2363">Исправлена команда `aks get-credentials` для обработки ошибок Юникода при загрузке файлов конфигурации Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="8b368-2363">Fixed `aks get-credentials` to handle Unicode errors when loading Kubernetes configuration files</span></span>
* <span data-ttu-id="8b368-2364">Добавлено сообщение в `az aks install-cli`, чтобы помочь получить `kubectl` в `$PATH`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2364">Added a message to `az aks install-cli` to help get `kubectl` in `$PATH`</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2365">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2365">Appservice</span></span>

* <span data-ttu-id="8b368-2366">Исправлена проблема со сбоем `webapp [backup|restore]` из-за пустой ссылки.</span><span class="sxs-lookup"><span data-stu-id="8b368-2366">Fixed issue where `webapp [backup|restore]` failed because of a null reference</span></span>
* <span data-ttu-id="8b368-2367">Добавлена поддержка стандартных планов службы приложений с помощью `az configure --defaults appserviceplan=my-asp`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2367">Added support for default app service plans through `az configure --defaults appserviceplan=my-asp`</span></span>

### <a name="cdn"></a><span data-ttu-id="8b368-2368">CDN</span><span class="sxs-lookup"><span data-stu-id="8b368-2368">CDN</span></span>

* <span data-ttu-id="8b368-2369">Добавлены команды `cdn custom-domain [enable-https|disable-https]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2369">Added `cdn custom-domain [enable-https|disable-https]` commands</span></span>

### <a name="container"></a><span data-ttu-id="8b368-2370">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-2370">Container</span></span>

* <span data-ttu-id="8b368-2371">Добавлен параметр `--follow` для `az container logs` для журналов потоковой передачи.</span><span class="sxs-lookup"><span data-stu-id="8b368-2371">Added `--follow` option to `az container logs` for streaming logs</span></span>
* <span data-ttu-id="8b368-2372">Добавлена команда `container attach`, которая добавляет локальный стандартный поток вывода и поток вывода сообщений об ошибках к контейнеру в группе контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2372">Added `container attach` command that attaches local standard output and error streams to a container in a container group</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8b368-2373">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-2373">CosmosDB</span></span>

* <span data-ttu-id="8b368-2374">Добавлена поддержка настройки параметров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2374">Added support for setting capabilities</span></span>

### <a name="extension"></a><span data-ttu-id="8b368-2375">Расширение</span><span class="sxs-lookup"><span data-stu-id="8b368-2375">Extension</span></span>

* <span data-ttu-id="8b368-2376">Добавлена поддержка параметра `--pip-proxy` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2376">Added support for `--pip-proxy` parameter to `az extension [add|update]` commands</span></span>
* <span data-ttu-id="8b368-2377">Добавлена поддержка аргумента `--pip-extra-index-urls` для команд `az extension [add|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2377">Added support for `--pip-extra-index-urls` argument to `az extension [add|update]` commands</span></span>

### <a name="feedback"></a><span data-ttu-id="8b368-2378">Отзывы</span><span class="sxs-lookup"><span data-stu-id="8b368-2378">Feedback</span></span>

* <span data-ttu-id="8b368-2379">Добавлены сведения о расширении к данным телеметрии.</span><span class="sxs-lookup"><span data-stu-id="8b368-2379">Added extension information to telemetry data</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-2380">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-2380">Interactive</span></span>

* <span data-ttu-id="8b368-2381">Исправлена проблема, когда пользователю предлагалось войти в интерактивном режиме в Cloud Shell.</span><span class="sxs-lookup"><span data-stu-id="8b368-2381">Fixed issue where user is prompted to login when using interactive mode in Cloud Shell</span></span>
* <span data-ttu-id="8b368-2382">Исправлена регрессия с отсутствующей функцией заполнения параметров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2382">Fixed regression with missing parameter completions</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-2383">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-2383">IoT</span></span>

* <span data-ttu-id="8b368-2384">Исправлена проблема, когда `iot dps access policy [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="8b368-2384">Fixed issue where `iot dps access policy [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="8b368-2385">Исправлена проблема, когда `iot dps linked-hub [create|update]` в случае успешного выполнения возвращает сообщение об ошибке "Не найдено".</span><span class="sxs-lookup"><span data-stu-id="8b368-2385">Fixed issue where `iot dps linked-hub [create|update]` would return a 'not found' error on success</span></span>
* <span data-ttu-id="8b368-2386">Добавлена поддержка параметра `--no-wait` для `iot dps access policy [create|update]` и `iot dps linked-hub [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2386">Added `--no-wait` support to `iot dps access policy [create|update]` and `iot dps linked-hub [create|update]`</span></span>
* <span data-ttu-id="8b368-2387">Изменена команда `iot hub create` для указания числа секций.</span><span class="sxs-lookup"><span data-stu-id="8b368-2387">Changed `iot hub create` to allow specifying the number of partitions</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-2388">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-2388">Monitor</span></span>

* <span data-ttu-id="8b368-2389">Исправлена команда `az monitor log-profiles create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2389">Fixed `az monitor log-profiles create` command</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2390">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2390">Network</span></span>

* <span data-ttu-id="8b368-2391">Исправлен параметр `--tags` для следующих команд:</span><span class="sxs-lookup"><span data-stu-id="8b368-2391">Fixed the `--tags` option for the following commands:</span></span>
  * `network public-ip create`
  * `network lb create`
  * `network local-gateway create`
  * `network nic create`
  * `network vnet-gateway create`
  * `network vpn-connection create`

### <a name="profile"></a><span data-ttu-id="8b368-2392">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-2392">Profile</span></span>

* <span data-ttu-id="8b368-2393">Включена команда `az login` для использования в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="8b368-2393">Enabled `az login` in from interactive mode</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-2394">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-2394">Resource</span></span>

* <span data-ttu-id="8b368-2395">Снова добавлена команда `feature show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2395">Added back `feature show`</span></span>

### <a name="role"></a><span data-ttu-id="8b368-2396">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-2396">Role</span></span>

* <span data-ttu-id="8b368-2397">Добавлен аргумент `--available-to-other-tenants` для команды `ad app update`</span><span class="sxs-lookup"><span data-stu-id="8b368-2397">Added `--available-to-other-tenants` argument to `ad app update`</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-2398">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-2398">SQL</span></span>

* <span data-ttu-id="8b368-2399">Добавлены команды `sql server dns-alias`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2399">Added `sql server dns-alias` commands</span></span>
* <span data-ttu-id="8b368-2400">Добавлена команда `sql db rename`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2400">Added `sql db rename`</span></span>
* <span data-ttu-id="8b368-2401">Добавлена поддержка аргумента `--ids` для команд SQL.</span><span class="sxs-lookup"><span data-stu-id="8b368-2401">Added support for the `--ids` argument to all sql commands</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2402">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2402">Storage</span></span>

* <span data-ttu-id="8b368-2403">Добавлены команды `storage blob service-properties delete-policy` и `storage blob undelete` для включения обратимого удаления.</span><span class="sxs-lookup"><span data-stu-id="8b368-2403">Added `storage blob service-properties delete-policy` and `storage blob undelete` commands to enable soft-delete</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2404">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2404">VM</span></span>

* <span data-ttu-id="8b368-2405">Исправлена ошибка, когда шифрование виртуальной машины инициализировалось не полностью.</span><span class="sxs-lookup"><span data-stu-id="8b368-2405">Fixed a crash when VM encryption may not be fully initialized</span></span>
* <span data-ttu-id="8b368-2406">Добавлены выходные данные идентификатора субъекта для включения MSI.</span><span class="sxs-lookup"><span data-stu-id="8b368-2406">Added principal ID output on enabling MSI</span></span>
* <span data-ttu-id="8b368-2407">Фиксированное значение `vm boot-diagnostics get-boot-log`</span><span class="sxs-lookup"><span data-stu-id="8b368-2407">Fixed `vm boot-diagnostics get-boot-log`</span></span>


## <a name="january-31-2018"></a><span data-ttu-id="8b368-2408">31 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2408">January 31, 2018</span></span>

<span data-ttu-id="8b368-2409">Версия 2.0.26</span><span class="sxs-lookup"><span data-stu-id="8b368-2409">Version 2.0.26</span></span>

### <a name="core"></a><span data-ttu-id="8b368-2410">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-2410">Core</span></span>

* <span data-ttu-id="8b368-2411">Добавлена поддержка получения необработанного маркера в контексте MSI.</span><span class="sxs-lookup"><span data-stu-id="8b368-2411">Added support raw token retrival in MSI context</span></span>
* <span data-ttu-id="8b368-2412">Удалена строка индикатора опроса после завершения LRO при выполнении cmd.exe в Windows.</span><span class="sxs-lookup"><span data-stu-id="8b368-2412">Removed polling indicator string after finishing LRO on Windows cmd.exe</span></span>
* <span data-ttu-id="8b368-2413">Добавлено предупреждение, которое появляется при использовании настроенных по умолчанию параметров, измененных на запись уровня INFO.</span><span class="sxs-lookup"><span data-stu-id="8b368-2413">Added a warning that appears when using a configured default has been changed to an INFO level entry.</span></span> <span data-ttu-id="8b368-2414">Используйте `--verbose` для просмотра.</span><span class="sxs-lookup"><span data-stu-id="8b368-2414">Use `--verbose` to see</span></span>
* <span data-ttu-id="8b368-2415">Добавьте индикатор хода выполнения для ожидания команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-2415">Add a progress indicator for wait commands</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2416">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2416">ACS</span></span>

* <span data-ttu-id="8b368-2417">Добавлено описание аргумента `--disable-browser`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2417">Clarified `--disable-browser` argument</span></span>
* <span data-ttu-id="8b368-2418">Улучшено заполнение нажатием клавиши TAB для аргументов `--vm-size`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2418">Improved tab completion for `--vm-size` arguments</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2419">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2419">Appservice</span></span>

* <span data-ttu-id="8b368-2420">Фиксированное значение `webapp log [tail|download]`</span><span class="sxs-lookup"><span data-stu-id="8b368-2420">Fixed `webapp log [tail|download]`</span></span>
* <span data-ttu-id="8b368-2421">Удалена проверка `kind` в веб-приложениях и функциях.</span><span class="sxs-lookup"><span data-stu-id="8b368-2421">Removed the `kind` check on webapps and functions</span></span>

### <a name="cdn"></a><span data-ttu-id="8b368-2422">CDN</span><span class="sxs-lookup"><span data-stu-id="8b368-2422">CDN</span></span>

* <span data-ttu-id="8b368-2423">Устранена проблема с отсутствием клиента для команды `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2423">Fixed missing client issue with `cdn custom-domain create`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8b368-2424">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-2424">CosmosDB</span></span>

* <span data-ttu-id="8b368-2425">Исправлено описание параметров для политик отработки отказа.</span><span class="sxs-lookup"><span data-stu-id="8b368-2425">Fixed parameter description for failover policies</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-2426">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-2426">Interactive</span></span>

* <span data-ttu-id="8b368-2427">Исправлена проблема, когда заполнение параметров команд больше не выполнялось.</span><span class="sxs-lookup"><span data-stu-id="8b368-2427">Fixed issue where command option completions no longer appeared</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2428">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2428">Network</span></span>

* <span data-ttu-id="8b368-2429">Добавлена защита `--cert-password` для `application-gateway create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2429">Added protection for `--cert-password` to `application-gateway create`</span></span>
* <span data-ttu-id="8b368-2430">Исправлена проблема с `application-gateway update`, когда команда `--sku` ошибочно применяла значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-2430">Fixed issue with `application-gateway update` where `--sku` erroneously applied a default value</span></span>
* <span data-ttu-id="8b368-2431">Добавлена защита `--shared-key` и `--authorization-key` для `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2431">Added protection for `--shared-key` and `--authorization-key` to `vpn-connection create`</span></span>
* <span data-ttu-id="8b368-2432">Устранена проблема с отсутствием клиента для команды `asg create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2432">Fixed missing client issue with `asg create`</span></span>
* <span data-ttu-id="8b368-2433">Добавлен параметр `--file-name / -f` для экспортируемых имен в `dns zone export`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2433">Added `--file-name / -f` parameter for exported names to `dns zone export`</span></span>
* <span data-ttu-id="8b368-2434">Исправлены следующие ошибки для `dns zone export`:</span><span class="sxs-lookup"><span data-stu-id="8b368-2434">Fixed the following issues with `dns zone export`:</span></span>
  * <span data-ttu-id="8b368-2435">Исправлена проблема, когда длинные записи ТХТ неправильно экспортировались.</span><span class="sxs-lookup"><span data-stu-id="8b368-2435">Fixed issue where long TXT records were incorrectly exported</span></span>
  * <span data-ttu-id="8b368-2436">Исправлена проблема, когда записи ТХТ в кавычках неправильно экспортировались без символов экранирования.</span><span class="sxs-lookup"><span data-stu-id="8b368-2436">Fixed issue where quoted TXT records were incorrectly exported without escaped quotes</span></span>
* <span data-ttu-id="8b368-2437">Исправлена проблема, когда некоторые записи импортировались дважды с помощью `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2437">Fixed issue where certain records were imported twice with `dns zone import`</span></span>
* <span data-ttu-id="8b368-2438">Восстановлены команды `vnet-gateway root-cert` и `vnet-gateway revoked-cert`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2438">Restored `vnet-gateway root-cert` and `vnet-gateway revoked-cert` commands</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-2439">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-2439">Profile</span></span>

* <span data-ttu-id="8b368-2440">Исправлена команда `get-access-token` для работы в виртуальной машине с идентификатором.</span><span class="sxs-lookup"><span data-stu-id="8b368-2440">Fixed `get-access-token` to work inside a VM with identity</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-2441">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-2441">Resource</span></span>

* <span data-ttu-id="8b368-2442">Исправлена ошибка с `deployment [create|validate]`, когда предупреждение неправильно отображалось, если поле type шаблона содержало значения в верхнем регистре.</span><span class="sxs-lookup"><span data-stu-id="8b368-2442">Fixed bug with `deployment [create|validate]` where warning was incorrectly displayed when a template 'type' field contained uppercase values</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2443">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2443">Storage</span></span>

* <span data-ttu-id="8b368-2444">Исправлена проблема с переносом учетных записей хранения из версии 1 в версию 2.</span><span class="sxs-lookup"><span data-stu-id="8b368-2444">Fixed issue with migrating Storage V1 accounts to Storage V2</span></span>
* <span data-ttu-id="8b368-2445">Добавлены отчеты о ходе выполнения всех команд отправки или скачивания.</span><span class="sxs-lookup"><span data-stu-id="8b368-2445">Added progress reporting for all upload/download commands</span></span>
* <span data-ttu-id="8b368-2446">Исправлена ошибка, которая препятствовала использованию параметра аргумента -n с `storage account check-name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2446">Fixed bug preventing "-n" arg option with `storage account check-name`</span></span>
* <span data-ttu-id="8b368-2447">Добавлен столбец snapshot в табличные выходные данные для `blob [list|show]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2447">Added 'snapshot' column to table output for `blob [list|show]`</span></span>
* <span data-ttu-id="8b368-2448">Исправлены ошибки с разными параметрами, которые должны были анализироваться как целые числа.</span><span class="sxs-lookup"><span data-stu-id="8b368-2448">Fixed bugs with various parameters that needed to be parsed as ints</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2449">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2449">VM</span></span>

* <span data-ttu-id="8b368-2450">Добавлена команда `vm image accept-terms` для разрешения создания виртуальных машин из образов с дополнительными расходами.</span><span class="sxs-lookup"><span data-stu-id="8b368-2450">Added `vm image accept-terms` command to allow creating VMs from images with additional charges</span></span>
* <span data-ttu-id="8b368-2451">Исправлена команда `[vm|vmss create]` для выполнения команд с прокси-сервера с помощью неподписанных сертификатов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2451">Fixed `[vm|vmss create]` to ensure commands can run under proxy with unsigned certificates</span></span>
* <span data-ttu-id="8b368-2452">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка режима низкого приоритета для VMSS.</span><span class="sxs-lookup"><span data-stu-id="8b368-2452">[PREVIEW] Added support for "low" priority to VMSS</span></span>
* <span data-ttu-id="8b368-2453">Добавлена защита `--admin-password` для `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2453">Added protection for `--admin-password` to `[vm|vmss] create`</span></span>


## <a name="january-17-2018"></a><span data-ttu-id="8b368-2454">17 января 2018 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2454">January 17, 2018</span></span>

<span data-ttu-id="8b368-2455">Версия 2.0.25</span><span class="sxs-lookup"><span data-stu-id="8b368-2455">Version 2.0.25</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-2456">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-2456">ACR</span></span>

* <span data-ttu-id="8b368-2457">Добавлена возможность отката входа ACR при ошибках учетных данных в Windows.</span><span class="sxs-lookup"><span data-stu-id="8b368-2457">Added acr login fallback on Windows credential errors</span></span>
* <span data-ttu-id="8b368-2458">Включены журналы реестра.</span><span class="sxs-lookup"><span data-stu-id="8b368-2458">Enabled registry logs</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2459">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2459">ACS</span></span>

* <span data-ttu-id="8b368-2460">Исправлена команда `get-credentials`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2460">Fixed `get-credentials` command</span></span>
* <span data-ttu-id="8b368-2461">Удалено требование роли для имени субъекта-службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-2461">Removed SPN role requirement</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2462">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2462">Appservice</span></span>

* <span data-ttu-id="8b368-2463">Исправлена ошибка с `config ssl upload`, при которой значение `hosting_environment_profile` было NULL.</span><span class="sxs-lookup"><span data-stu-id="8b368-2463">Fixed bug with `config ssl upload` where `hosting_environment_profile` was null</span></span>
* <span data-ttu-id="8b368-2464">В `browse` добавлена поддержка для пользовательских URL-адресов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2464">Added support for custom URLs to `browse`</span></span>
* <span data-ttu-id="8b368-2465">Исправлена поддержка слотов для `log tail`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2465">Fixed slot support for `log tail`</span></span>

### <a name="backup"></a><span data-ttu-id="8b368-2466">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="8b368-2466">Backup</span></span>

* <span data-ttu-id="8b368-2467">Параметр `--container-name` для `backup item list` теперь не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="8b368-2467">Changed `--container-name` option of `backup item list` to be optional</span></span>
* <span data-ttu-id="8b368-2468">В `backup restore restore-disks` добавлены варианты учетной записи хранения.</span><span class="sxs-lookup"><span data-stu-id="8b368-2468">Added storage account options to `backup restore restore-disks`</span></span>
* <span data-ttu-id="8b368-2469">Для проверки расположения в `backup protection enable-for-vm` добавлена чувствительность к регистру.</span><span class="sxs-lookup"><span data-stu-id="8b368-2469">Fixed location check in `backup protection enable-for-vm` to be case insensitive</span></span>
* <span data-ttu-id="8b368-2470">Устранена проблема, при которой команды завершались сбоем с указанием недопустимого имени контейнера.</span><span class="sxs-lookup"><span data-stu-id="8b368-2470">Fixed issue where commands failed with an invalid container name</span></span>
* <span data-ttu-id="8b368-2471">В `backup item list` теперь по умолчанию включен параметр Health Status.</span><span class="sxs-lookup"><span data-stu-id="8b368-2471">Changed `backup item list` to include 'Health Status' by default</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-2472">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-2472">Batch</span></span>

* <span data-ttu-id="8b368-2473">`batch login` теперь возвращает сведения об аутентификации.</span><span class="sxs-lookup"><span data-stu-id="8b368-2473">Changed `batch login` to return authentication details</span></span>

### <a name="cloud"></a><span data-ttu-id="8b368-2474">Cloud</span><span class="sxs-lookup"><span data-stu-id="8b368-2474">Cloud</span></span>

* <span data-ttu-id="8b368-2475">При установке `--profile` в облаке теперь не требуется указывать конечные точки.</span><span class="sxs-lookup"><span data-stu-id="8b368-2475">Changed to not require endpoints when setting `--profile` on a cloud</span></span>

### <a name="consumption"></a><span data-ttu-id="8b368-2476">Потребление</span><span class="sxs-lookup"><span data-stu-id="8b368-2476">Consumption</span></span>

* <span data-ttu-id="8b368-2477">Добавлены новые команды для резервирования: `consumption reservations summaries` и `consumption reservations details`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2477">Added new commands for reservations: `consumption reservations summaries` and `consumption reservations details`</span></span>

### <a name="event-grid"></a><span data-ttu-id="8b368-2478">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-2478">Event Grid</span></span>

* <span data-ttu-id="8b368-2479">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid topic event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2479">[BREAKING CHANGE] Moved the `az eventgrid topic event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="8b368-2480">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команды `az eventgrid resource event-subscription` перемещены в `eventgrid event-subscription`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2480">[BREAKING CHANGE] Moved the `az eventgrid resource event-subscription` commands to `eventgrid event-subscription`</span></span>
* <span data-ttu-id="8b368-2481">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Удалена команда `eventgrid event-subscription show-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2481">[BREAKING CHANGE] Removed the `eventgrid event-subscription show-endpoint-url` command.</span></span> <span data-ttu-id="8b368-2482">Вместо нее следует использовать `eventgrid event-subscription show --include-full-endpoint-url`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2482">Use `eventgrid event-subscription show --include-full-endpoint-url` instead</span></span>
* <span data-ttu-id="8b368-2483">Добавлена команда `eventgrid topic update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2483">Added command `eventgrid topic update`</span></span>
* <span data-ttu-id="8b368-2484">Добавлена команда `eventgrid event-subscription update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2484">Added command `eventgrid event-subscription update`</span></span>
* <span data-ttu-id="8b368-2485">Добавлен параметр `--ids` для команд `eventgrid topic`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2485">Added `--ids` parameter for `eventgrid topic` commands</span></span>
* <span data-ttu-id="8b368-2486">Добавлена поддержка заполнения нажатием клавиши TAB для имен разделов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2486">Added tab completion support for topic names</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-2487">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-2487">Interactive</span></span>

* <span data-ttu-id="8b368-2488">Устранена проблема, при которой интерактивный режим не работал с Python 2.x.</span><span class="sxs-lookup"><span data-stu-id="8b368-2488">Fixed issue where interactive mode did not work with Python 2.x</span></span>
* <span data-ttu-id="8b368-2489">Исправлены ошибки при запуске.</span><span class="sxs-lookup"><span data-stu-id="8b368-2489">Fixed errors on startup</span></span>
* <span data-ttu-id="8b368-2490">Устранена проблема, при которой некоторые команды не работали в интерактивном режиме.</span><span class="sxs-lookup"><span data-stu-id="8b368-2490">Fixed issue with some commands not running in interactive mode</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-2491">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-2491">IoT</span></span>

* <span data-ttu-id="8b368-2492">Добавлена поддержка службы подготовки устройств.</span><span class="sxs-lookup"><span data-stu-id="8b368-2492">Added support for device provisioning service</span></span>
* <span data-ttu-id="8b368-2493">В команды и справочную информацию о них добавлены сообщения о нерекомендуемых версиях.</span><span class="sxs-lookup"><span data-stu-id="8b368-2493">Added deprecation messages in commands and command help</span></span>
* <span data-ttu-id="8b368-2494">Теперь при проверке Интернета вещей указывается расширение Интернета вещей.</span><span class="sxs-lookup"><span data-stu-id="8b368-2494">Added IoT check to inform users of the IoT Extension</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-2495">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-2495">Monitor</span></span>

* <span data-ttu-id="8b368-2496">Добавлена поддержка параметра нескольких диагностических операций.</span><span class="sxs-lookup"><span data-stu-id="8b368-2496">Added multi-diagnostic setting support.</span></span> <span data-ttu-id="8b368-2497">Теперь параметр `--name` является обязательным для `az monitor diagnostic-settings create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2497">The `--name` parameter is now required for `az monitor diagnostic-settings create`</span></span>
* <span data-ttu-id="8b368-2498">Добавлена команда `monitor diagnostic-settings categories` для получения категории параметров диагностики.</span><span class="sxs-lookup"><span data-stu-id="8b368-2498">Added command `monitor diagnostic-settings categories` to get diagnostic settings category</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2499">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2499">Network</span></span>

* <span data-ttu-id="8b368-2500">Устранена проблема с `vnet-gateway update` при попытке входа в активный режим и режим ожидания или выхода из них.</span><span class="sxs-lookup"><span data-stu-id="8b368-2500">Fixed issue when trying to change to/from active-standby mode with `vnet-gateway update`</span></span>
* <span data-ttu-id="8b368-2501">Для `application-gateway [create|update]` добавлена поддержка HTTP2.</span><span class="sxs-lookup"><span data-stu-id="8b368-2501">Added support for HTTP2 to `application-gateway [create|update]`</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-2502">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-2502">Profile</span></span>

* <span data-ttu-id="8b368-2503">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="8b368-2503">Added support for login with user assigned identities</span></span>

### <a name="role"></a><span data-ttu-id="8b368-2504">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-2504">Role</span></span>

* <span data-ttu-id="8b368-2505">В `role assignment create` добавлен аргумент `--assignee-object-id`, чтобы обойти запрос графов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2505">Added `--assignee-object-id` argument to `role assignment create` to bypass graph query</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8b368-2506">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8b368-2506">Service Fabric</span></span>

* <span data-ttu-id="8b368-2507">В результат проверки при создании кластера добавлены подробные сведения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="8b368-2507">Added detailed errors to validation response when creating cluster</span></span>
* <span data-ttu-id="8b368-2508">Устранена проблема отсутствия клиента при выполнении некоторых команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-2508">Fixed missing client issue with several commands</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2509">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2509">VM</span></span>

* <span data-ttu-id="8b368-2510">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Поддержка разных зон для `vmss`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2510">[PREVIEW] Cross-zone support for `vmss`</span></span>
* <span data-ttu-id="8b368-2511">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Значение по умолчанию `vmss` для одной зоны заменено данными подсистемы балансировки нагрузки уровня "Стандартный".</span><span class="sxs-lookup"><span data-stu-id="8b368-2511">[BREAKING CHANGE] Changed single-zone `vmss` default to "Standard" load balancer</span></span>
* <span data-ttu-id="8b368-2512">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Для EMSI параметр `externalIdentities` изменен на `userAssignedIdentities`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2512">[BREAKING CHANGE] Changed `externalIdentities` to `userAssignedIdentities` for EMSI</span></span>
* <span data-ttu-id="8b368-2513">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка переключения дисков ОС.</span><span class="sxs-lookup"><span data-stu-id="8b368-2513">[PREVIEW] Added support for OS disk swap</span></span>
* <span data-ttu-id="8b368-2514">Добавлена поддержка использования образов виртуальных машин из других подписок.</span><span class="sxs-lookup"><span data-stu-id="8b368-2514">Added support for using VM images from other subscriptions</span></span>
* <span data-ttu-id="8b368-2515">В `[vm|vmss] create` добавлены аргументы `--plan-name`, `--plan-product`, `--plan-promotion-code` и `--plan-publisher`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2515">Added `--plan-name`, `--plan-product`, `--plan-promotion-code` and `--plan-publisher` arguments to `[vm|vmss] create`</span></span>
* <span data-ttu-id="8b368-2516">Устранены проблемы с `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2516">Fixed error issues with `[vm|vmss] create`</span></span>
* <span data-ttu-id="8b368-2517">Устранена проблема чрезмерного использования ресурсов из-за `vm image list --all`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2517">Fixed excessive resource usage caused by `vm image list --all`</span></span>

## <a name="december-19-2017"></a><span data-ttu-id="8b368-2518">19 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2518">December 19, 2017</span></span>

<span data-ttu-id="8b368-2519">Версия 2.0.23</span><span class="sxs-lookup"><span data-stu-id="8b368-2519">Version 2.0.23</span></span>

* <span data-ttu-id="8b368-2520">Добавлена поддержка для входа с использованием назначенных пользователям удостоверений.</span><span class="sxs-lookup"><span data-stu-id="8b368-2520">Added support for login with user assigned identities</span></span>

### <a name="container"></a><span data-ttu-id="8b368-2521">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-2521">Container</span></span>

* <span data-ttu-id="8b368-2522">Исправлен неправильный порядок параметров для журналов контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2522">Fixed incorrect order of parameters for container logs</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2523">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2523">Network</span></span>

* <span data-ttu-id="8b368-2524">Добавлен аргумент `--disable-bgp-route-propagation` для команды `route-table [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8b368-2524">Added `--disable-bgp-route-propagation` argument to `route-table [create|update]`</span></span>
* <span data-ttu-id="8b368-2525">Добавлен аргумент `--ip-tags` для команды `public-ip [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8b368-2525">Added `--ip-tags` argument to `public-ip [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2526">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2526">Storage</span></span>

* <span data-ttu-id="8b368-2527">Добавлена поддержка хранилища версии 2.</span><span class="sxs-lookup"><span data-stu-id="8b368-2527">Added support for storage V2</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2528">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2528">VM</span></span>

* <span data-ttu-id="8b368-2529">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка для назначенных пользователям удостоверений для виртуальных машин и VMSS.</span><span class="sxs-lookup"><span data-stu-id="8b368-2529">[PREVIEW] Added support for user-assigned identities for VMs and VMSSes</span></span>


## <a name="december-5-2017"></a><span data-ttu-id="8b368-2530">5 декабря 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2530">December 5, 2017</span></span>

<span data-ttu-id="8b368-2531">Версия 2.0.22</span><span class="sxs-lookup"><span data-stu-id="8b368-2531">Version 2.0.22</span></span>

* <span data-ttu-id="8b368-2532">Удалена команда `az component`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2532">Removed `az component` commands.</span></span> <span data-ttu-id="8b368-2533">Вместо нее следует использовать `az extension`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2533">Use `az extension` instead</span></span>

### <a name="core"></a><span data-ttu-id="8b368-2534">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-2534">Core</span></span>
* <span data-ttu-id="8b368-2535">Конечная точка `AZURE_US_GOV_CLOUD` центра AAD изменена с login.microsoftonline.com на login.microsoftonline.us.</span><span class="sxs-lookup"><span data-stu-id="8b368-2535">Modified the `AZURE_US_GOV_CLOUD` AAD authority endpoint from login.microsoftonline.com to login.microsoftonline.us</span></span>
* <span data-ttu-id="8b368-2536">Исправлена проблема с непрерывной отправкой телеметрии.</span><span class="sxs-lookup"><span data-stu-id="8b368-2536">Fixed issue where telemetry would continuously resend</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2537">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2537">ACS</span></span>

* <span data-ttu-id="8b368-2538">Добавлены команды `aks install-connector` и `aks remove-connector`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2538">Added `aks install-connector` and `aks remove-connector` commands</span></span>
* <span data-ttu-id="8b368-2539">Улучшены сообщения об ошибках для команды `acs create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2539">Improved error reporting for `acs create`</span></span>
* <span data-ttu-id="8b368-2540">Добавлена возможность использования команды `aks get-credentials -f` без полного пути.</span><span class="sxs-lookup"><span data-stu-id="8b368-2540">Fixed usage of `aks get-credentials -f` without fully-qualified path</span></span>

### <a name="advisor"></a><span data-ttu-id="8b368-2541">Помощник</span><span class="sxs-lookup"><span data-stu-id="8b368-2541">Advisor</span></span>

* <span data-ttu-id="8b368-2542">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="8b368-2542">Initial release</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2543">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2543">Appservice</span></span>

* <span data-ttu-id="8b368-2544">Добавлена возможность создания имени сертификата с помощью команды `webapp config ssl upload`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2544">Fixed cert name generation with `webapp config ssl upload`</span></span>
* <span data-ttu-id="8b368-2545">Исправлены команды `webapp [list|show]` и `functionapp [list|show]` для отображения правильных приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-2545">Fixed `webapp [list|show]` and `functionapp [list|show]` to display correct apps</span></span>
* <span data-ttu-id="8b368-2546">Добавлено стандартное значение для переменной `WEBSITE_NODE_DEFAULT_VERSION`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2546">Added default value for `WEBSITE_NODE_DEFAULT_VERSION`</span></span>

### <a name="consumption"></a><span data-ttu-id="8b368-2547">Потребление</span><span class="sxs-lookup"><span data-stu-id="8b368-2547">Consumption</span></span>

* <span data-ttu-id="8b368-2548">Добавлена поддержка API версии 2017-11-30.</span><span class="sxs-lookup"><span data-stu-id="8b368-2548">Aded support for API version 2017-11-30</span></span>

### <a name="container"></a><span data-ttu-id="8b368-2549">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-2549">Container</span></span>

* <span data-ttu-id="8b368-2550">Исправлены стандартные порты регрессии.</span><span class="sxs-lookup"><span data-stu-id="8b368-2550">Fixed default ports regression</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-2551">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-2551">Monitor</span></span>

* <span data-ttu-id="8b368-2552">Добавлена поддержка нескольких измерений для команд метрик.</span><span class="sxs-lookup"><span data-stu-id="8b368-2552">Added multi-dimension support to metrics command</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-2553">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-2553">Resource</span></span>

* <span data-ttu-id="8b368-2554">Добавлен аргумент `--include-response-body` для команды `resource show`</span><span class="sxs-lookup"><span data-stu-id="8b368-2554">Added `--include-response-body` argument to `resource show`</span></span>

### <a name="role"></a><span data-ttu-id="8b368-2555">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-2555">Role</span></span>

* <span data-ttu-id="8b368-2556">Добавлено отображение стандартных назначений "классических" администраторов для команды `role assignment list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2556">Added display of default assignments for "classic" administraors to `role assignment list`</span></span>
* <span data-ttu-id="8b368-2557">Добавлена поддержка команды `ad sp reset-credentials` для добавления учетных данных вместо перезаписи.</span><span class="sxs-lookup"><span data-stu-id="8b368-2557">Added suport to `ad sp reset-credentials` for adding credentials instead of overwriting</span></span>
* <span data-ttu-id="8b368-2558">Улучшены сообщения об ошибках для команды `ad sp create-for-rbac`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2558">Improved error reporting for `ad sp create-for-rbac`</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-2559">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-2559">SQL</span></span>

* <span data-ttu-id="8b368-2560">Добавлены команды `sql db list-usages` и `sql db show-usage`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2560">Added `sql db list-usages` and `sql db show-usage` commands</span></span>
* <span data-ttu-id="8b368-2561">Добавлены команды `sql server conn-policy show` и `sql server conn-policy update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2561">Added `sql server conn-policy show` and `sql server conn-policy update` commands</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2562">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2562">VM</span></span>

* <span data-ttu-id="8b368-2563">Добавлены сведения о зонах для команды `az vm list-skus`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2563">Added zone information to `az vm list-skus`</span></span>


## <a name="november-14-2017"></a><span data-ttu-id="8b368-2564">14 ноября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2564">November 14, 2017</span></span>

<span data-ttu-id="8b368-2565">Версия 2.0.21</span><span class="sxs-lookup"><span data-stu-id="8b368-2565">Version 2.0.21</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-2566">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-2566">ACR</span></span>

* <span data-ttu-id="8b368-2567">Добавлена поддержка создания веб-перехватчиков в регионах репликации.</span><span class="sxs-lookup"><span data-stu-id="8b368-2567">Added support for creating webhooks in replication regions</span></span>


### <a name="acs"></a><span data-ttu-id="8b368-2568">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2568">ACS</span></span>

* <span data-ttu-id="8b368-2569">В AKS агент теперь называется узлом.</span><span class="sxs-lookup"><span data-stu-id="8b368-2569">Changed all wording of "agent" to "node" in AKS</span></span>
* <span data-ttu-id="8b368-2570">Параметр `--orchestrator-release` для командлета `acs create` не рекомендуется использовать.</span><span class="sxs-lookup"><span data-stu-id="8b368-2570">Deprecated `--orchestrator-release` option for `acs create`</span></span>
* <span data-ttu-id="8b368-2571">Изменен размер виртуальной машины для AKS по умолчанию на `Standard_D1_v2`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2571">Changed default VM size for AKS to `Standard_D1_v2`</span></span>
* <span data-ttu-id="8b368-2572">Исправлена команда `az aks browse` для Windows.</span><span class="sxs-lookup"><span data-stu-id="8b368-2572">Fixed `az aks browse` on Windows</span></span>
* <span data-ttu-id="8b368-2573">Исправлена команда `az aks get-credentials` для Windows.</span><span class="sxs-lookup"><span data-stu-id="8b368-2573">Fixed `az aks get-credentials` on Windows</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2574">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2574">Appservice</span></span>

* <span data-ttu-id="8b368-2575">Добавлен источник развертывания `config-zip` для веб-приложений и приложений-функций.</span><span class="sxs-lookup"><span data-stu-id="8b368-2575">Added deployment source `config-zip` for webapps and function apps</span></span>
* <span data-ttu-id="8b368-2576">Добавлен параметр `--docker-container-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2576">Added `--docker-container-logging` option to `az webapp log config`</span></span>
* <span data-ttu-id="8b368-2577">Удален параметр `storage` из параметра `--web-server-logging` для команды `az webapp log config`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2577">Removed the `storage` option from the parameter `--web-server-logging` of `az webapp log config`</span></span>
* <span data-ttu-id="8b368-2578">Улучшены сообщения об ошибках для команды `deployment user set`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2578">Improved error messages for `deployment user set`</span></span>
* <span data-ttu-id="8b368-2579">Добавлена поддержка создания приложений-функций Linux</span><span class="sxs-lookup"><span data-stu-id="8b368-2579">Added support for creating Linux function apps</span></span>
* <span data-ttu-id="8b368-2580">Фиксированное значение `list-locations`</span><span class="sxs-lookup"><span data-stu-id="8b368-2580">Fixed `list-locations`</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-2581">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-2581">Batch</span></span>

* <span data-ttu-id="8b368-2582">Исправлена ошибка в команде создания пула, когда идентификатор ресурса использовался с флагом `--image`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2582">Fixed bug in pool create command when a resource ID was used with the `--image` flag</span></span>

### <a name="batchai"></a><span data-ttu-id="8b368-2583">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="8b368-2583">Batchai</span></span>

* <span data-ttu-id="8b368-2584">Добавлен короткий параметр `-s` для параметра `--vm-size` при указании размера виртуальной машины в команде `file-server create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2584">Added short option, `-s`, for `--vm-size` when providing VM size in `file-server create` command</span></span>
* <span data-ttu-id="8b368-2585">Добавлены аргументы ключа и имени учетной записи хранения в параметры команды `cluster create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2585">Added storage account name and key arguments to `cluster create` parameters</span></span>
* <span data-ttu-id="8b368-2586">Исправлена документация по командам `job list-files` и `job stream-file`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2586">Fixed documentation for `job list-files` and `job stream-file`</span></span>
* <span data-ttu-id="8b368-2587">Добавлен короткий параметр `-r` для параметра `--cluster-name` при указании имени кластера в команде `job create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2587">Added short option, `-r`, for `--cluster-name` when providing cluster name in `job create` command</span></span>

### <a name="cloud"></a><span data-ttu-id="8b368-2588">Cloud</span><span class="sxs-lookup"><span data-stu-id="8b368-2588">Cloud</span></span>

* <span data-ttu-id="8b368-2589">Изменена команда `cloud [register|update]` для предотвращения регистрации облаков, для которых отсутствуют необходимые конечные точки.</span><span class="sxs-lookup"><span data-stu-id="8b368-2589">Changed `cloud [register|update]` to prevent registering clouds that have missing required endpoints</span></span>

### <a name="container"></a><span data-ttu-id="8b368-2590">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-2590">Container</span></span>

* <span data-ttu-id="8b368-2591">Добавлена поддержка открытия нескольких портов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2591">Added support to open multiple ports</span></span>
* <span data-ttu-id="8b368-2592">Добавлена политика перезапуска группы контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2592">Added container group restart policy</span></span>
* <span data-ttu-id="8b368-2593">Добавлена поддержка подключения файлового ресурса Azure в качестве тома.</span><span class="sxs-lookup"><span data-stu-id="8b368-2593">Added support to mount Azure File share as a volume</span></span>
* <span data-ttu-id="8b368-2594">Обновлена вспомогательная документация.</span><span class="sxs-lookup"><span data-stu-id="8b368-2594">Updated helper docs</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8b368-2595">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8b368-2595">Data Lake Analytics</span></span>

* <span data-ttu-id="8b368-2596">Изменена команда `[job|account] list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="8b368-2596">Changed `[job|account] list` to return more concise information</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8b368-2597">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="8b368-2597">Data Lake Store</span></span>

* <span data-ttu-id="8b368-2598">Изменена команда `account list` для возврата более кратких сведений.</span><span class="sxs-lookup"><span data-stu-id="8b368-2598">Changed `account list` to return more concise information</span></span>

### <a name="extension"></a><span data-ttu-id="8b368-2599">Расширение</span><span class="sxs-lookup"><span data-stu-id="8b368-2599">Extension</span></span>

* <span data-ttu-id="8b368-2600">Добавлена команда `extension list-available` для отображения официальных расширений Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="8b368-2600">Added `extension list-available` to allow listing official Microsoft extensions</span></span>
* <span data-ttu-id="8b368-2601">Добавлен параметр `--name` для команды `extension [add|update]` для установки расширений по имени.</span><span class="sxs-lookup"><span data-stu-id="8b368-2601">Added `--name` to `extension [add|update]` to allow installing extensions by name</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-2602">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-2602">IoT</span></span>

* <span data-ttu-id="8b368-2603">Добавлена поддержка центров сертификации (ЦС) и цепочек сертификатов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2603">Added support for certificate authorities (CA) and certificate chains</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-2604">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-2604">Monitor</span></span>

* <span data-ttu-id="8b368-2605">Добавлены команды `activity-log alert`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2605">Added `activity-log alert` commands</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2606">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2606">Network</span></span>

* <span data-ttu-id="8b368-2607">Добавлена поддержка DNS-записей типа CAA.</span><span class="sxs-lookup"><span data-stu-id="8b368-2607">Added support for CAA DNS records</span></span>
* <span data-ttu-id="8b368-2608">Исправлена проблема, когда конечные точки могли не обновляться с помощью команды `traffic-manager profile update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2608">Fixed issue where endpoints could not be updated with `traffic-manager profile update`</span></span>
* <span data-ttu-id="8b368-2609">Исправлена проблема, когда команда `vnet update --dns-servers` не работала в зависимости от способа создания виртуальной сети.</span><span class="sxs-lookup"><span data-stu-id="8b368-2609">Fixed issue where `vnet update --dns-servers` didn't work depending on how the VNET was created</span></span>
* <span data-ttu-id="8b368-2610">Исправлена проблема, когда относительные DNS-имена неправильно импортировались с помощью команды `dns zone import`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2610">Fixed issue where relative DNS names were incorrectly imported by `dns zone import`</span></span>

### <a name="reservations"></a><span data-ttu-id="8b368-2611">Резервирование</span><span class="sxs-lookup"><span data-stu-id="8b368-2611">Reservations</span></span>

* <span data-ttu-id="8b368-2612">Первоначальный выпуск предварительной версии</span><span class="sxs-lookup"><span data-stu-id="8b368-2612">Initial preview release</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-2613">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-2613">Resource</span></span>

* <span data-ttu-id="8b368-2614">Добавлена поддержка идентификаторов ресурсов для блокировок на уровне ресурсов и параметра `--resource`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2614">Added support for resource IDs to `--resource` parameter and resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-2615">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-2615">SQL</span></span>

* <span data-ttu-id="8b368-2616">Добавлен параметр `--ignore-missing-vnet-service-endpoint` для команды `sql server vnet-rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2616">Added `--ignore-missing-vnet-service-endpoint` parameter to `sql server vnet-rule [create|update]`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2617">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2617">Storage</span></span>

* <span data-ttu-id="8b368-2618">Изменена команда `storage account create` для использования номера SKU `Standard_RAGRS` по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-2618">Changed `storage account create` to use SKU `Standard_RAGRS` as default</span></span>
* <span data-ttu-id="8b368-2619">Исправлены ошибки при обработке имени файла или большого двоичного объекта, содержащего символы, отличные от ASCII.</span><span class="sxs-lookup"><span data-stu-id="8b368-2619">Fixed bugs when dealing with file/blob names that include non-ascii chars</span></span>
* <span data-ttu-id="8b368-2620">Исправлена ошибка, препятствующая использованию параметра `--source-uri` с командой `storage [blob|file] copy start-batch`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2620">Fixed bug that prevented using `--source-uri` with `storage [blob|file] copy start-batch`</span></span>
* <span data-ttu-id="8b368-2621">Добавлены команды для удаления нескольких объектов с помощью команды `storage [blob|file] delete-batch`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2621">Added commands to glob and delete multiple objects with `storage [blob|file] delete-batch`</span></span>
* <span data-ttu-id="8b368-2622">Исправлена проблема с включением метрик с помощью команды `storage metrics update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2622">Fixed issue when enabling metrics with `storage metrics update`</span></span>
* <span data-ttu-id="8b368-2623">Исправлена проблема с файлами более 200 ГБ при использовании команды `storage blob upload-batch`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2623">Fixed issue with files over 200GB when using `storage blob upload-batch`</span></span>
* <span data-ttu-id="8b368-2624">Исправлена проблема, когда параметры `--bypass` и `--default-action` игнорировались командой `storage account [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2624">Fixed issue where `--bypass` and `--default-action` were ignored by `storage account [create|update]`</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2625">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2625">VM</span></span>

* <span data-ttu-id="8b368-2626">Исправлена ошибка с командой `vmss create`, препятствующая использованию уровня `Basic`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2626">Fixed a bug with `vmss create` that prevented using the `Basic` size tier</span></span>
* <span data-ttu-id="8b368-2627">Добавлены аргументы `--plan` для команды `[vm|vmss] create` для пользовательских образов с информацией о выставлении счетов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2627">Added `--plan` arguments to `[vm|vmss] create` for custom images with billing information</span></span>
* <span data-ttu-id="8b368-2628">Добавлены команды `vm secret `[add|remove|list]\`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2628">Added `vm secret `[add|remove|list]\` commands</span></span>
* <span data-ttu-id="8b368-2629">Переименование `vm format-secret` в `vm secret format`</span><span class="sxs-lookup"><span data-stu-id="8b368-2629">Renamed `vm format-secret` to `vm secret format`</span></span>
* <span data-ttu-id="8b368-2630">Добавлен аргумент `--encrypt format` для команды `vm encryption enable`</span><span class="sxs-lookup"><span data-stu-id="8b368-2630">Added `--encrypt format` argument to `vm encryption enable`</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="8b368-2631">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2631">October 24, 2017</span></span>

<span data-ttu-id="8b368-2632">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="8b368-2632">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="8b368-2633">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-2633">Core</span></span>

* <span data-ttu-id="8b368-2634">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="8b368-2634">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-2635">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-2635">ACR</span></span>

* <span data-ttu-id="8b368-2636">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="8b368-2636">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="8b368-2637">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="8b368-2637">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="8b368-2638">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="8b368-2638">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2639">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2639">ACS</span></span>

* <span data-ttu-id="8b368-2640">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="8b368-2640">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="8b368-2641">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="8b368-2641">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2642">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2642">Appservice</span></span>

* <span data-ttu-id="8b368-2643">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="8b368-2643">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="8b368-2644">Компонент</span><span class="sxs-lookup"><span data-stu-id="8b368-2644">Component</span></span>

* <span data-ttu-id="8b368-2645">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="8b368-2645">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-2646">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-2646">Monitor</span></span>

* <span data-ttu-id="8b368-2647">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2647">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-2648">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-2648">Resource</span></span>

* <span data-ttu-id="8b368-2649">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="8b368-2649">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="8b368-2650">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="8b368-2650">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2651">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2651">VM</span></span>

* <span data-ttu-id="8b368-2652">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="8b368-2652">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="8b368-2653">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2653">October 9, 2017</span></span>

<span data-ttu-id="8b368-2654">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="8b368-2654">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="8b368-2655">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-2655">Core</span></span>

* <span data-ttu-id="8b368-2656">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="8b368-2656">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2657">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2657">Appservice</span></span>

* <span data-ttu-id="8b368-2658">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2658">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-2659">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-2659">Batch</span></span>

* <span data-ttu-id="8b368-2660">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="8b368-2660">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="8b368-2661">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="8b368-2661">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="8b368-2662">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-2662">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="8b368-2663">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2663">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="8b368-2664">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="8b368-2664">Batchai</span></span>

* <span data-ttu-id="8b368-2665">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="8b368-2665">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="8b368-2666">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8b368-2666">Keyvault</span></span>

* <span data-ttu-id="8b368-2667">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8b368-2667">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="8b368-2668">(#4448)</span><span class="sxs-lookup"><span data-stu-id="8b368-2668">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="8b368-2669">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2669">Network</span></span>

* <span data-ttu-id="8b368-2670">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="8b368-2670">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="8b368-2671">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="8b368-2671">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-2672">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-2672">Resource</span></span>

* <span data-ttu-id="8b368-2673">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2673">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="8b368-2674">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="8b368-2674">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="8b368-2675">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="8b368-2675">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="8b368-2676">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="8b368-2676">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-2677">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-2677">Sql</span></span>

* <span data-ttu-id="8b368-2678">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="8b368-2678">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="8b368-2679">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="8b368-2679">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="8b368-2680">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="8b368-2680">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2681">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2681">Storage</span></span>

* <span data-ttu-id="8b368-2682">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2682">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2683">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="8b368-2683">Vm</span></span>

* <span data-ttu-id="8b368-2684">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2684">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="8b368-2685">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2685">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="8b368-2686">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2686">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="8b368-2687">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2687">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="8b368-2688">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="8b368-2688">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="8b368-2689">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2689">September 22, 2017</span></span>

<span data-ttu-id="8b368-2690">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="8b368-2690">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-2691">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-2691">Resource</span></span>

* <span data-ttu-id="8b368-2692">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="8b368-2692">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="8b368-2693">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="8b368-2693">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="8b368-2694">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="8b368-2694">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="8b368-2695">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2695">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2696">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2696">Network</span></span>

* <span data-ttu-id="8b368-2697">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="8b368-2697">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="8b368-2698">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="8b368-2698">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="8b368-2699">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="8b368-2699">Added `asg` application security group commands</span></span>
* <span data-ttu-id="8b368-2700">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="8b368-2700">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="8b368-2701">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8b368-2701">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="8b368-2702">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8b368-2702">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="8b368-2703">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2703">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2704">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2704">Storage</span></span>

* <span data-ttu-id="8b368-2705">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="8b368-2705">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="8b368-2706">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="8b368-2706">Eventgrid</span></span>

* <span data-ttu-id="8b368-2707">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="8b368-2707">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-2708">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-2708">SQL</span></span>

* <span data-ttu-id="8b368-2709">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="8b368-2709">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="8b368-2710">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="8b368-2710">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="8b368-2711">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="8b368-2711">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="8b368-2712">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8b368-2712">Keyvault</span></span>

* <span data-ttu-id="8b368-2713">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="8b368-2713">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2714">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2714">VM</span></span>

* <span data-ttu-id="8b368-2715">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="8b368-2715">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="8b368-2716">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="8b368-2716">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="8b368-2717">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="8b368-2717">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="8b368-2718">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="8b368-2718">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="8b368-2719">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="8b368-2719">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="8b368-2720">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="8b368-2720">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2721">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2721">ACS</span></span>

* <span data-ttu-id="8b368-2722">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="8b368-2722">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2723">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2723">Appservice</span></span>

* <span data-ttu-id="8b368-2724">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="8b368-2724">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="8b368-2725">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="8b368-2725">Backup</span></span>

* <span data-ttu-id="8b368-2726">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="8b368-2726">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="8b368-2727">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2727">September 11, 2017</span></span>

<span data-ttu-id="8b368-2728">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="8b368-2728">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="8b368-2729">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-2729">Core</span></span>

* <span data-ttu-id="8b368-2730">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="8b368-2730">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="8b368-2731">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="8b368-2731">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2732">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2732">Acs</span></span>

* <span data-ttu-id="8b368-2733">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2733">Added `acs list-locations` command</span></span>
* <span data-ttu-id="8b368-2734">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-2734">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2735">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2735">Appservice</span></span>

* <span data-ttu-id="8b368-2736">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="8b368-2736">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="8b368-2737">CDN</span><span class="sxs-lookup"><span data-stu-id="8b368-2737">CDN</span></span>

* <span data-ttu-id="8b368-2738">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2738">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`</span></span>

### <a name="extension"></a><span data-ttu-id="8b368-2739">Расширение</span><span class="sxs-lookup"><span data-stu-id="8b368-2739">Extension</span></span>

* <span data-ttu-id="8b368-2740">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="8b368-2740">Initial Release</span></span>

### <a name="keyvault"></a><span data-ttu-id="8b368-2741">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8b368-2741">Keyvault</span></span>

* <span data-ttu-id="8b368-2742">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2742">Fixed issue where permissions were case sensitive for `keyvault set-policy`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2743">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2743">Network</span></span>

* <span data-ttu-id="8b368-2744">Переименование `vnet list-private-access-services` в `vnet list-endpoint-services`</span><span class="sxs-lookup"><span data-stu-id="8b368-2744">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="8b368-2745">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2745">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="8b368-2746">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2746">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="8b368-2747">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2747">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="8b368-2748">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2748">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-2749">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-2749">Resource</span></span>

* <span data-ttu-id="8b368-2750">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2750">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="8b368-2751">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2751">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="8b368-2752">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2752">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="8b368-2753">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="8b368-2753">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-2754">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-2754">SQL</span></span>

* <span data-ttu-id="8b368-2755">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2755">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2756">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2756">VM</span></span>

* <span data-ttu-id="8b368-2757">Исправлено: Не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="8b368-2757">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="8b368-2758">Исправлено: Использовать те же расширения имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="8b368-2758">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="8b368-2759">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2759">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="8b368-2760">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="8b368-2760">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="8b368-2761">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="8b368-2761">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="8b368-2762">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2762">August 31, 2017</span></span>

<span data-ttu-id="8b368-2763">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="8b368-2763">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="8b368-2764">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8b368-2764">Keyvault</span></span>

* <span data-ttu-id="8b368-2765">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2765">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="8b368-2766">Sf</span><span class="sxs-lookup"><span data-stu-id="8b368-2766">Sf</span></span>

* <span data-ttu-id="8b368-2767">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="8b368-2767">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2768">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2768">Storage</span></span>

* <span data-ttu-id="8b368-2769">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="8b368-2769">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="8b368-2770">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="8b368-2770">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="8b368-2771">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2771">August 28, 2017</span></span>

<span data-ttu-id="8b368-2772">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="8b368-2772">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="8b368-2773">CLI</span><span class="sxs-lookup"><span data-stu-id="8b368-2773">CLI</span></span>

* <span data-ttu-id="8b368-2774">Для `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="8b368-2774">Added legal note to `--version`</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2775">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2775">ACS</span></span>

* <span data-ttu-id="8b368-2776">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="8b368-2776">Corrected preview regions</span></span>
* <span data-ttu-id="8b368-2777">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2777">Formatted default `dns_name_prefix` properly</span></span>
* <span data-ttu-id="8b368-2778">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="8b368-2778">Optimized acs command output</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2779">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2779">Appservice</span></span>

* <span data-ttu-id="8b368-2780">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2780">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="8b368-2781">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2781">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="8b368-2782">Предоставлен параметр `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2782">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="8b368-2783">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="8b368-2783">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="8b368-2784">Исправлено: Правильно определять параметры слота.</span><span class="sxs-lookup"><span data-stu-id="8b368-2784">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-2785">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-2785">IoT</span></span>

* <span data-ttu-id="8b368-2786">Исправлена ошибка #3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="8b368-2786">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2787">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2787">Network</span></span>

* <span data-ttu-id="8b368-2788">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2788">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="8b368-2789">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2789">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="8b368-2790">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2790">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="8b368-2791">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2791">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="8b368-2792">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2792">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-2793">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-2793">Profile</span></span>

* <span data-ttu-id="8b368-2794">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="8b368-2794">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8b368-2795">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8b368-2795">Service Fabric</span></span>

* <span data-ttu-id="8b368-2796">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="8b368-2796">Preview release</span></span>
* <span data-ttu-id="8b368-2797">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="8b368-2797">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="8b368-2798">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="8b368-2798">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="8b368-2799">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2799">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2800">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2800">Storage</span></span>

* <span data-ttu-id="8b368-2801">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="8b368-2801">Enabled setting blob tier</span></span>
* <span data-ttu-id="8b368-2802">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-2802">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="8b368-2803">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2803">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>
* <span data-ttu-id="8b368-2804">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="8b368-2804">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="8b368-2805">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2805">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="8b368-2806">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2806">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2807">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2807">VM</span></span>

* <span data-ttu-id="8b368-2808">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2808">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="8b368-2809">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2809">Added support for `--lb-sku` to `vmss create`:</span></span>
* <span data-ttu-id="8b368-2810">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="8b368-2810">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span>
* <span data-ttu-id="8b368-2811">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="8b368-2811">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="8b368-2812">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="8b368-2812">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="8b368-2813">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2813">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="8b368-2814">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2814">August 15, 2017</span></span>

<span data-ttu-id="8b368-2815">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="8b368-2815">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2816">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2816">ACS</span></span>

* <span data-ttu-id="8b368-2817">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="8b368-2817">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2818">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2818">Appservice</span></span>

* <span data-ttu-id="8b368-2819">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="8b368-2819">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="8b368-2820">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-2820">Event Grid</span></span>

* <span data-ttu-id="8b368-2821">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="8b368-2821">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="8b368-2822">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2822">August 11, 2017</span></span>

<span data-ttu-id="8b368-2823">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="8b368-2823">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2824">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2824">ACS</span></span>

* <span data-ttu-id="8b368-2825">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="8b368-2825">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-2826">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-2826">Batch</span></span>

* <span data-ttu-id="8b368-2827">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="8b368-2827">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="8b368-2828">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="8b368-2828">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="8b368-2829">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2829">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="8b368-2830">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="8b368-2830">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="8b368-2831">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="8b368-2831">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="8b368-2832">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="8b368-2832">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="8b368-2833">Компонент</span><span class="sxs-lookup"><span data-stu-id="8b368-2833">Component</span></span>

* <span data-ttu-id="8b368-2834">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="8b368-2834">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="8b368-2835">Контейнер</span><span class="sxs-lookup"><span data-stu-id="8b368-2835">Container</span></span>

* <span data-ttu-id="8b368-2836">`create`: исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="8b368-2836">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="8b368-2837">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="8b368-2837">Data Lake Store</span></span>

* <span data-ttu-id="8b368-2838">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="8b368-2838">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="8b368-2839">Сетка событий Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-2839">Event Grid</span></span>

* <span data-ttu-id="8b368-2840">Начальный выпуск</span><span class="sxs-lookup"><span data-stu-id="8b368-2840">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2841">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2841">Network</span></span>

* <span data-ttu-id="8b368-2842">`lb`: исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="8b368-2842">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="8b368-2843">`application-gateway {subresource} delete`: исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2843">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="8b368-2844">`application-gateway http-settings update`: исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2844">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="8b368-2845">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2845">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-2846">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-2846">Profile</span></span>

* <span data-ttu-id="8b368-2847">`account list`: добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="8b368-2847">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-2848">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-2848">Storage</span></span>

* <span data-ttu-id="8b368-2849">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="8b368-2849">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-2850">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-2850">VM</span></span>

* <span data-ttu-id="8b368-2851">`availability-set`: предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="8b368-2851">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="8b368-2852">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2852">Exposed `list-skus` command</span></span>
* <span data-ttu-id="8b368-2853">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="8b368-2853">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="8b368-2854">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="8b368-2854">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="8b368-2855">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="8b368-2855">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="8b368-2856">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-2856">July 28, 2017</span></span>

<span data-ttu-id="8b368-2857">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="8b368-2857">Version 2.0.12</span></span>

* <span data-ttu-id="8b368-2858">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2858">Added container commands</span></span>
* <span data-ttu-id="8b368-2859">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2859">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="8b368-2860">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-2860">Core</span></span>

* <span data-ttu-id="8b368-2861">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="8b368-2861">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="8b368-2862">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="8b368-2862">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="8b368-2863">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="8b368-2863">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="8b368-2864">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="8b368-2864">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="8b368-2865">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="8b368-2865">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="8b368-2866">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="8b368-2866">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="8b368-2867">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="8b368-2867">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="8b368-2868">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="8b368-2868">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="8b368-2869">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="8b368-2869">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="8b368-2870">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="8b368-2870">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="8b368-2871">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="8b368-2871">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="8b368-2872">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="8b368-2872">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="8b368-2873">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="8b368-2873">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="8b368-2874">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="8b368-2874">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="8b368-2875">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="8b368-2875">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="8b368-2876">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="8b368-2876">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="8b368-2877">ACR</span><span class="sxs-lookup"><span data-stu-id="8b368-2877">ACR</span></span>

* <span data-ttu-id="8b368-2878">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2878">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="8b368-2879">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="8b368-2879">Support SKU update for managed registries</span></span>
* <span data-ttu-id="8b368-2880">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="8b368-2880">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="8b368-2881">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="8b368-2881">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="8b368-2882">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="8b368-2882">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="8b368-2883">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="8b368-2883">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-2884">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-2884">ACS</span></span>

* <span data-ttu-id="8b368-2885">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="8b368-2885">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-2886">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="8b368-2886">Appservice</span></span>

* <span data-ttu-id="8b368-2887">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="8b368-2887">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="8b368-2888">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="8b368-2888">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="8b368-2889">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2889">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="8b368-2890">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="8b368-2890">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="8b368-2891">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="8b368-2891">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="8b368-2892">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="8b368-2892">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="8b368-2893">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="8b368-2893">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="8b368-2894">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="8b368-2894">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="8b368-2895">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="8b368-2895">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="8b368-2896">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2896">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="8b368-2897">Пакетная служба Azure</span><span class="sxs-lookup"><span data-stu-id="8b368-2897">Batch</span></span>

* <span data-ttu-id="8b368-2898">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="8b368-2898">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="8b368-2899">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2899">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="8b368-2900">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2900">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="8b368-2901">CDN</span><span class="sxs-lookup"><span data-stu-id="8b368-2901">CDN</span></span>

* <span data-ttu-id="8b368-2902">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="8b368-2902">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist</span></span>

### <a name="cloud"></a><span data-ttu-id="8b368-2903">Cloud</span><span class="sxs-lookup"><span data-stu-id="8b368-2903">Cloud</span></span>

* <span data-ttu-id="8b368-2904">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="8b368-2904">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="8b368-2905">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="8b368-2905">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="8b368-2906">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="8b368-2906">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="8b368-2907">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="8b368-2907">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="8b368-2908">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2908">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8b368-2909">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-2909">CosmosDB</span></span>

* <span data-ttu-id="8b368-2910">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="8b368-2910">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="8b368-2911">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="8b368-2911">Added support for collection default TTL</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8b368-2912">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8b368-2912">Data Lake Analytics</span></span>

* <span data-ttu-id="8b368-2913">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2913">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="8b368-2914">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2914">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="8b368-2915">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2915">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8b368-2916">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="8b368-2916">Data Lake Store</span></span>

* <span data-ttu-id="8b368-2917">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2917">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="8b368-2918">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="8b368-2918">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="8b368-2919">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2919">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="8b368-2920">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="8b368-2920">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="8b368-2921">Интерактивно</span><span class="sxs-lookup"><span data-stu-id="8b368-2921">Interactive</span></span>

* <span data-ttu-id="8b368-2922">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="8b368-2922">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="8b368-2923">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="8b368-2923">Increased test coverage</span></span>
* <span data-ttu-id="8b368-2924">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="8b368-2924">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="8b368-2925">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="8b368-2925">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="8b368-2926">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="8b368-2926">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="8b368-2927">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="8b368-2927">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="8b368-2928">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="8b368-2928">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="8b368-2929">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2929">Added `--progress` flag</span></span>
* <span data-ttu-id="8b368-2930">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2930">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="8b368-2931">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="8b368-2931">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="8b368-2932">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="8b368-2932">IoT</span></span>

* <span data-ttu-id="8b368-2933">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="8b368-2933">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="8b368-2934">(3934).</span><span class="sxs-lookup"><span data-stu-id="8b368-2934">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="8b368-2935">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8b368-2935">Key vault</span></span>

* <span data-ttu-id="8b368-2936">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="8b368-2936">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="8b368-2937">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2937">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="8b368-2938">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="8b368-2938">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="8b368-2939">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2939">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="8b368-2940">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2940">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="8b368-2941">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="8b368-2941">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="8b368-2942">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="8b368-2942">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="8b368-2943">(3307).</span><span class="sxs-lookup"><span data-stu-id="8b368-2943">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="8b368-2944">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="8b368-2944">Lab</span></span>

* <span data-ttu-id="8b368-2945">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2945">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="8b368-2946">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2946">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-2947">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-2947">Monitor</span></span>

* <span data-ttu-id="8b368-2948">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="8b368-2948">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="8b368-2949">Переименование `monitor alert-rule-incidents list` в `monitor alert list-incidents`</span><span class="sxs-lookup"><span data-stu-id="8b368-2949">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="8b368-2950">Переименование `monitor alert-rule-incidents show` в `monitor alert show-incident`</span><span class="sxs-lookup"><span data-stu-id="8b368-2950">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="8b368-2951">Переименование `monitor metric-defintions list` в `monitor metrics list-definitions`</span><span class="sxs-lookup"><span data-stu-id="8b368-2951">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="8b368-2952">Переименование `monitor alert-rules` в `monitor alert`</span><span class="sxs-lookup"><span data-stu-id="8b368-2952">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="8b368-2953">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="8b368-2953">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="8b368-2954">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="8b368-2954">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="8b368-2955">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="8b368-2955">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="8b368-2956">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="8b368-2956">`location` no longer required</span></span>
  * <span data-ttu-id="8b368-2957">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="8b368-2957">Add name and ID support for target</span></span>
  * <span data-ttu-id="8b368-2958">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="8b368-2958">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="8b368-2959">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="8b368-2959">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="8b368-2960">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="8b368-2960">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="8b368-2961">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="8b368-2961">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="8b368-2962">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2962">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="8b368-2963">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2963">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="8b368-2964">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-2964">Network</span></span>

* <span data-ttu-id="8b368-2965">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2965">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="8b368-2966">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2966">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="8b368-2967">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="8b368-2967">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="8b368-2968">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2968">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="8b368-2969">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2969">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="8b368-2970">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2970">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="8b368-2971">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2971">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="8b368-2972">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2972">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="8b368-2973">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2973">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="8b368-2974">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2974">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="8b368-2975">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2975">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="8b368-2976">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2976">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="8b368-2977">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2977">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="8b368-2978">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2978">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="8b368-2979">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2979">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="8b368-2980">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2980">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="8b368-2981">Добавлена поддержка аргумента `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка аргумента --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="8b368-2981">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="8b368-2982">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2982">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="8b368-2983">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2983">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="8b368-2984">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2984">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="8b368-2985">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2985">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="8b368-2986">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2986">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="8b368-2987">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="8b368-2987">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="8b368-2988">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="8b368-2988">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="8b368-2989">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="8b368-2989">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="8b368-2990">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="8b368-2990">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="8b368-2991">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="8b368-2991">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-2992">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-2992">Profile</span></span>

* <span data-ttu-id="8b368-2993">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="8b368-2993">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="8b368-2994">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="8b368-2994">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="8b368-2995">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="8b368-2995">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="8b368-2996">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="8b368-2996">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="8b368-2997">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="8b368-2997">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="8b368-2998">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="8b368-2998">RDBMS</span></span>

* <span data-ttu-id="8b368-2999">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="8b368-2999">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="8b368-3000">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="8b368-3000">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="8b368-3001">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="8b368-3001">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="8b368-3002">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="8b368-3002">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-3003">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-3003">Resource</span></span>

* <span data-ttu-id="8b368-3004">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3004">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="8b368-3005">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3005">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="8b368-3006">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3006">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="8b368-3007">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3007">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="8b368-3008">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="8b368-3008">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="8b368-3009">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3009">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="8b368-3010">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="8b368-3010">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="8b368-3011">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3011">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="8b368-3012">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-3012">Role</span></span>

* <span data-ttu-id="8b368-3013">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="8b368-3013">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="8b368-3014">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="8b368-3014">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="8b368-3015">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="8b368-3015">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="8b368-3016">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="8b368-3016">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="8b368-3017">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3017">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="8b368-3018">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="8b368-3018">Service Fabric</span></span>
* <span data-ttu-id="8b368-3019">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="8b368-3019">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="8b368-3020">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="8b368-3020">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="8b368-3021">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="8b368-3021">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-3022">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-3022">SQL</span></span>

* <span data-ttu-id="8b368-3023">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3023">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="8b368-3024">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3024">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="8b368-3025">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3025">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-3026">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-3026">Storage</span></span>

* <span data-ttu-id="8b368-3027">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="8b368-3027">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="8b368-3028">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="8b368-3028">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="8b368-3029">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="8b368-3029">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="8b368-3030">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="8b368-3030">Rephrased exception message from CORS add (#3638) (#3362)</span></span>
* <span data-ttu-id="8b368-3031">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="8b368-3031">Converted generator to a list in download batch command dry run mode (#3592)</span></span>
* <span data-ttu-id="8b368-3032">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="8b368-3032">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-3033">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-3033">VM</span></span>

* <span data-ttu-id="8b368-3034">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="8b368-3034">Support configuring nsg</span></span>
* <span data-ttu-id="8b368-3035">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="8b368-3035">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="8b368-3036">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="8b368-3036">Support managed service identities</span></span>
* <span data-ttu-id="8b368-3037">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3037">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`</span></span>
* <span data-ttu-id="8b368-3038">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="8b368-3038">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="8b368-3039">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-3039">May 10, 2017</span></span>

<span data-ttu-id="8b368-3040">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="8b368-3040">Version 2.0.6</span></span>

* <span data-ttu-id="8b368-3041">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="8b368-3041">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="8b368-3042">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="8b368-3042">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="8b368-3043">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="8b368-3043">Include Data Lake Analytics and Data Lake Store modules</span></span>
* <span data-ttu-id="8b368-3044">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="8b368-3044">Include Cognitive Services module</span></span>
* <span data-ttu-id="8b368-3045">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="8b368-3045">Include Service Fabric module</span></span>
* <span data-ttu-id="8b368-3046">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="8b368-3046">Include Interactive module (rename of az-shell)</span></span>
* <span data-ttu-id="8b368-3047">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="8b368-3047">Add support for CDN commands</span></span>
* <span data-ttu-id="8b368-3048">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="8b368-3048">Remove Container module</span></span>
* <span data-ttu-id="8b368-3049">Добавлена команда az -v для az --version ([#2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3049">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="8b368-3050">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3050">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="8b368-3051">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-3051">Core</span></span>

* <span data-ttu-id="8b368-3052">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="8b368-3052">core: capture exceptions caused by unregistered provider and auto-register it</span></span>
* <span data-ttu-id="8b368-3053">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([#2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3053">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="8b368-3054">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3054">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="8b368-3055">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([#3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3055">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="8b368-3056">Добавлено расположение Python в az -version ([#2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3056">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="8b368-3057">Вход: поддержка входа при отсутствии подписок ([#2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3057">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="8b368-3058">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([#2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3058">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="8b368-3059">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([#2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3059">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="8b368-3060">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([#2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3060">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="8b368-3061">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="8b368-3061">core: Improved performance</span></span>
* <span data-ttu-id="8b368-3062">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="8b368-3062">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="8b368-3063">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="8b368-3063">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-3064">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-3064">ACS</span></span>

* <span data-ttu-id="8b368-3065">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="8b368-3065">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="8b368-3066">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="8b368-3066">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="8b368-3067">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="8b368-3067">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="8b368-3068">Удален профиль Windows перед вызовом метода PUT для команды scale ([#2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3068">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-3069">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-3069">AppService</span></span>

* <span data-ttu-id="8b368-3070">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="8b368-3070">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="8b368-3071">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-3071">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="8b368-3072">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="8b368-3072">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="8b368-3073">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="8b368-3073">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="8b368-3074">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="8b368-3074">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="8b368-3075">Включена поддержка настройки строк подключения ([#2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3075">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="8b368-3076">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="8b368-3076">support slot swap with preview</span></span>
* <span data-ttu-id="8b368-3077">Устранены ошибки из команд службы приложений ([#2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3077">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="8b368-3078">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([#2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3078">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="8b368-3079">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="8b368-3079">CosmosDB</span></span>

* <span data-ttu-id="8b368-3080">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="8b368-3080">Rename documentdb module to cosmosdb</span></span>
* <span data-ttu-id="8b368-3081">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="8b368-3081">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="8b368-3082">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="8b368-3082">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="8b368-3083">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="8b368-3083">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="8b368-3084">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="8b368-3084">Data Lake Analytics</span></span>

* <span data-ttu-id="8b368-3085">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="8b368-3085">Fix a bug where filtering on result and state for job lists would throw an error</span></span>
* <span data-ttu-id="8b368-3086">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="8b368-3086">Add support for new catalog item type: package.</span></span> <span data-ttu-id="8b368-3087">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3087">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="8b368-3088">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="8b368-3088">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="8b368-3089">Таблица</span><span class="sxs-lookup"><span data-stu-id="8b368-3089">Table</span></span>
  * <span data-ttu-id="8b368-3090">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="8b368-3090">Table valued function</span></span>
  * <span data-ttu-id="8b368-3091">Представление</span><span class="sxs-lookup"><span data-stu-id="8b368-3091">View</span></span>
  * <span data-ttu-id="8b368-3092">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="8b368-3092">Table Statistics.</span></span> <span data-ttu-id="8b368-3093">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="8b368-3093">This can also be listed with a schema, but without specifying a table name</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="8b368-3094">Data Lake Storage</span><span class="sxs-lookup"><span data-stu-id="8b368-3094">Data Lake Store</span></span>

* <span data-ttu-id="8b368-3095">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="8b368-3095">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios</span></span>
* <span data-ttu-id="8b368-3096">Повышена производительность загрузки пакетов и выполнения команд ([#2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3096">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="8b368-3097">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="8b368-3097">missed help for access show.</span></span> <span data-ttu-id="8b368-3098">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="8b368-3098">adding it.</span></span> <span data-ttu-id="8b368-3099">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="8b368-3099">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="8b368-3100">Поиск</span><span class="sxs-lookup"><span data-stu-id="8b368-3100">Find</span></span>

* <span data-ttu-id="8b368-3101">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="8b368-3101">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="8b368-3102">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="8b368-3102">KeyVault</span></span>

* <span data-ttu-id="8b368-3103">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="8b368-3103">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="8b368-3104">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="8b368-3104">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service</span></span>
* <span data-ttu-id="8b368-3105">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="8b368-3105">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="8b368-3106">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="8b368-3106">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not</span></span>
* <span data-ttu-id="8b368-3107">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([#2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3107">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="8b368-3108">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="8b368-3108">Lab</span></span>

* <span data-ttu-id="8b368-3109">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="8b368-3109">Adding create, show, delete & list commands for environment in the lab</span></span>
* <span data-ttu-id="8b368-3110">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="8b368-3110">Adding show & list commands to view ARM templates in the lab</span></span>
* <span data-ttu-id="8b368-3111">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="8b368-3111">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab</span></span>
* <span data-ttu-id="8b368-3112">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="8b368-3112">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula</span></span>
* <span data-ttu-id="8b368-3113">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="8b368-3113">Add commands to manage secrets within a Lab</span></span>

### <a name="monitor"></a><span data-ttu-id="8b368-3114">Монитор</span><span class="sxs-lookup"><span data-stu-id="8b368-3114">Monitor</span></span>

* <span data-ttu-id="8b368-3115">Исправление ошибки. моделирование параметра `--actions` команды `az alert-rules create` для использования строки в формате JSON ([#3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3115">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="8b368-3116">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([#2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3116">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="8b368-3117">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-3117">Network</span></span>

* <span data-ttu-id="8b368-3118">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3118">Add `network watcher test-connectivity` command</span></span>
* <span data-ttu-id="8b368-3119">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3119">Add support for `--filters` parameter for `network watcher packet-capture create`</span></span>
* <span data-ttu-id="8b368-3120">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-3120">Add support for Application Gateway connection draining</span></span>
* <span data-ttu-id="8b368-3121">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="8b368-3121">Add support for Application Gateway WAF rule set configuration</span></span>
* <span data-ttu-id="8b368-3122">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="8b368-3122">Add support for ExpressRoute route filters and rules</span></span>
* <span data-ttu-id="8b368-3123">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="8b368-3123">Add support for TrafficManager geographic routing</span></span>
* <span data-ttu-id="8b368-3124">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="8b368-3124">Add support for VPN connection policy-based traffic selectors</span></span>
* <span data-ttu-id="8b368-3125">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="8b368-3125">Add support for VPN connection IPSec policies</span></span>
* <span data-ttu-id="8b368-3126">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3126">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters</span></span>
* <span data-ttu-id="8b368-3127">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="8b368-3127">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="8b368-3128">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3128">Remove nulls values from output of `network vpn-connection list/show` commands</span></span>
* <span data-ttu-id="8b368-3129">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3129">BC: Fix bug in the output of `vpn-connection create`</span></span>
* <span data-ttu-id="8b368-3130">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="8b368-3130">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly</span></span>
* <span data-ttu-id="8b368-3131">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="8b368-3131">Fix bug in `dns zone import` where records were not imported correctly</span></span>
* <span data-ttu-id="8b368-3132">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="8b368-3132">Fix bug where `traffic-manager endpoint update` did not work</span></span>
* <span data-ttu-id="8b368-3133">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="8b368-3133">Add 'network watcher' preview commands</span></span>

### <a name="profile"></a><span data-ttu-id="8b368-3134">Профиль</span><span class="sxs-lookup"><span data-stu-id="8b368-3134">Profile</span></span>

* <span data-ttu-id="8b368-3135">Включена поддержка входа при отсутствии подписок ([#2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3135">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="8b368-3136">Включена поддержка сокращенных имен параметров в команде az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3136">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="8b368-3137">Redis</span><span class="sxs-lookup"><span data-stu-id="8b368-3137">Redis</span></span>

* <span data-ttu-id="8b368-3138">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="8b368-3138">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="8b368-3139">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="8b368-3139">Deprecates the 'update-settings' command</span></span>

### <a name="resource"></a><span data-ttu-id="8b368-3140">Ресурс</span><span class="sxs-lookup"><span data-stu-id="8b368-3140">Resource</span></span>

* <span data-ttu-id="8b368-3141">Добавлены команды определения managedapp и managedapp ([#2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3141">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="8b368-3142">Включена поддержка команд provider operation ([#2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3142">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="8b368-3143">Включена поддержка создания универсального ресурса ([#2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3143">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="8b368-3144">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="8b368-3144">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="8b368-3145">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="8b368-3145">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="8b368-3146">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="8b368-3146">Add docs for az lock update.</span></span> <span data-ttu-id="8b368-3147">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="8b368-3147">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="8b368-3148">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="8b368-3148">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="8b368-3149">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="8b368-3149">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="8b368-3150">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="8b368-3150">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="8b368-3151">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="8b368-3151">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="8b368-3152">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([#2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3152">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="8b368-3153">Роль</span><span class="sxs-lookup"><span data-stu-id="8b368-3153">Role</span></span>

* <span data-ttu-id="8b368-3154">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([#2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3154">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="8b368-3155">RBAC: добавлена полная поддержка команды ad group ([#2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3155">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="8b368-3156">Роль: устранены проблемы при обновлении определения роли ([#2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3156">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="8b368-3157">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="8b368-3157">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="8b368-3158">SQL</span><span class="sxs-lookup"><span data-stu-id="8b368-3158">SQL</span></span>

* <span data-ttu-id="8b368-3159">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="8b368-3159">Added az sql server list-usages and az sql db list-usages commands</span></span>
* <span data-ttu-id="8b368-3160">SQL: добавлена возможность прямого подключения к поставщику ресурса ([#2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3160">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="8b368-3161">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-3161">Storage</span></span>

* <span data-ttu-id="8b368-3162">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3162">Default location to resource group location for `storage account create`</span></span>
* <span data-ttu-id="8b368-3163">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="8b368-3163">Add support for incremental blob copy</span></span>
* <span data-ttu-id="8b368-3164">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="8b368-3164">Add support for large block blob upload</span></span>
* <span data-ttu-id="8b368-3165">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="8b368-3165">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-3166">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-3166">VM</span></span>

* <span data-ttu-id="8b368-3167">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="8b368-3167">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="8b368-3168">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="8b368-3168">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="8b368-3169">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="8b368-3169">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="8b368-3170">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="8b368-3170">az vm/vmss disk</span></span>
  3. <span data-ttu-id="8b368-3171">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="8b368-3171">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="8b368-3172">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="8b368-3172">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="8b368-3173">vm/vmss: добавлена поддержка создания из образа Marketplace, для которого требуются сведения о плане ([#1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3173">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="8b368-3174">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-3174">April 3, 2017</span></span>

<span data-ttu-id="8b368-3175">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="8b368-3175">Version 2.0.2</span></span>

<span data-ttu-id="8b368-3176">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="8b368-3176">We released the ACR, Batch, KeyVault, and SQL components in this release</span></span>

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

### <a name="core"></a><span data-ttu-id="8b368-3177">Основные сведения</span><span class="sxs-lookup"><span data-stu-id="8b368-3177">Core</span></span>

* <span data-ttu-id="8b368-3178">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-3178">Add acr, lab, monitor, and find modules to default list</span></span>
* <span data-ttu-id="8b368-3179">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3179">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="8b368-3180">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3180">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="8b368-3181">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3181">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="8b368-3182">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3182">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="8b368-3183">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="8b368-3183">Add prompting for missing template parameters.</span></span> <span data-ttu-id="8b368-3184">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3184">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="8b368-3185">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b368-3185">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="8b368-3186">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="8b368-3186">Support login to specific tenant</span></span>

### <a name="acs"></a><span data-ttu-id="8b368-3187">ACS</span><span class="sxs-lookup"><span data-stu-id="8b368-3187">ACS</span></span>

* <span data-ttu-id="8b368-3188">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3188">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="8b368-3189">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="8b368-3189">Add support for ssh key password prompting.</span></span> <span data-ttu-id="8b368-3190">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3190">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="8b368-3191">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="8b368-3191">Add support for windows clusters.</span></span> <span data-ttu-id="8b368-3192">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3192">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="8b368-3193">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="8b368-3193">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="8b368-3194">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3194">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>

### <a name="appservice"></a><span data-ttu-id="8b368-3195">AppService</span><span class="sxs-lookup"><span data-stu-id="8b368-3195">AppService</span></span>

* <span data-ttu-id="8b368-3196">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3196">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="8b368-3197">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3197">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="8b368-3198">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3198">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="8b368-3199">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3199">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>

### <a name="datalake"></a><span data-ttu-id="8b368-3200">Data Lake</span><span class="sxs-lookup"><span data-stu-id="8b368-3200">DataLake</span></span>

* <span data-ttu-id="8b368-3201">Первый выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="8b368-3201">Initial release of Data Lake Analytics module</span></span>
* <span data-ttu-id="8b368-3202">Первый выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="8b368-3202">Initial release of Data Lake Store module</span></span>

### <a name="docuemntdb"></a><span data-ttu-id="8b368-3203">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="8b368-3203">DocuemntDB</span></span>

* <span data-ttu-id="8b368-3204">DocumentDB: добавлена возможность получить список строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3204">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="8b368-3205">ВМ</span><span class="sxs-lookup"><span data-stu-id="8b368-3205">VM</span></span>

* <span data-ttu-id="8b368-3206">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3206">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="8b368-3207">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3207">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="8b368-3208">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3208">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="8b368-3209">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3209">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="8b368-3210">Масштабируемый набор виртуальных машин: добавлена поддержка \* для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3210">Virtual machine scale set: support \* to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="8b368-3211">Добавлен параметр --secrets для виртуальной машины и масштабируемого набора виртуальных машин ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3211">Add --secrets for VM and virtual machine scale set ([#2212}(<https://github.com/Azure/azure-cli/pull/2212>))</span></span>
* <span data-ttu-id="8b368-3212">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="8b368-3212">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="8b368-3213">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="8b368-3213">February 27, 2017</span></span>

<span data-ttu-id="8b368-3214">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="8b368-3214">Version 2.0.0</span></span>

<span data-ttu-id="8b368-3215">Этот первый общедоступный выпуск Azure CLI 2.0. Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="8b368-3215">This release of Azure CLI 2.0 is the first "Generally Available" release General availability applies to these command modules:</span></span>
- <span data-ttu-id="8b368-3216">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="8b368-3216">Container Service (acs)</span></span>
- <span data-ttu-id="8b368-3217">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="8b368-3217">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="8b368-3218">Сеть</span><span class="sxs-lookup"><span data-stu-id="8b368-3218">Networking</span></span>
- <span data-ttu-id="8b368-3219">Память</span><span class="sxs-lookup"><span data-stu-id="8b368-3219">Storage</span></span>

<span data-ttu-id="8b368-3220">Эти командные модули могут использоваться в рабочих средах. Они поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания. Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/). Вы можете задавать вопросы на [сайте StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3220">These command modules can be used in production and are supported by standard Microsoft SLA You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/) You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com) You can provide feedback from the command line with the `az feedback` command</span></span>

<span data-ttu-id="8b368-3221">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="8b368-3221">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI</span></span>

<span data-ttu-id="8b368-3222">Проверить версию CLI можно с помощью команды `az --version`. В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="8b368-3222">To verify the version of the CLI, use `az --version` The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using</span></span>

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
> <span data-ttu-id="8b368-3223">Некоторые командные модули имеют постфикс b*n* или rc*n*. Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="8b368-3223">Some of the command modules have a "b*n*" or "rc*n*" postfix These command modules are still in preview and will become generally available in the future</span></span>

<span data-ttu-id="8b368-3224">У нас также есть предварительные ежедневные сборки CLI. Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="8b368-3224">We also have nightly preview builds of the CLI For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup)</span></span>

<span data-ttu-id="8b368-3225">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="8b368-3225">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="8b368-3226">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="8b368-3226">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="8b368-3227">Свяжитесь с командой разработчиков ([azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)),</span><span class="sxs-lookup"><span data-stu-id="8b368-3227">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com)</span></span>
- <span data-ttu-id="8b368-3228">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="8b368-3228">Provide feedback from the command line with the `az feedback` command</span></span>

