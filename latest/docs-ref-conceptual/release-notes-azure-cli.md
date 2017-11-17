---
title: "Заметки о выпуске Azure CLI 2.0"
description: "Узнайте о последних обновлениях в Azure CLI 2.0"
keywords: "Azure CLI 2.0, заметки о выпуске"
author: sptramer
ms.author: sttramer
manager: douge
ms.date: 04/03/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ce0428f7-0a59-4e72-9237-d907b171af51
ms.openlocfilehash: 429b099dabd27d9356e88791f955ec52acd2a5f9
ms.sourcegitcommit: 9b36c15dc0e10024e23b8018604f5ef63c025de1
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/24/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="886c3-104">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="886c3-104">Azure CLI 2.0 release notes</span></span>

## <a name="october-24-2017"></a><span data-ttu-id="886c3-105">24 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-105">October 24, 2017</span></span>

<span data-ttu-id="886c3-106">Версия 2.0.20</span><span class="sxs-lookup"><span data-stu-id="886c3-106">Version 2.0.20</span></span>

### <a name="core"></a><span data-ttu-id="886c3-107">Core</span><span class="sxs-lookup"><span data-stu-id="886c3-107">Core</span></span>

* <span data-ttu-id="886c3-108">Обновление `2017-03-09-profile` для использования API `MGMT_STORAGE` версии `2016-01-01`</span><span class="sxs-lookup"><span data-stu-id="886c3-108">Updated `2017-03-09-profile` to consume `MGMT_STORAGE` API version `2016-01-01`</span></span>

### <a name="acr"></a><span data-ttu-id="886c3-109">ACR</span><span class="sxs-lookup"><span data-stu-id="886c3-109">ACR</span></span>

* <span data-ttu-id="886c3-110">Обновление службы управления ресурсами для указания API версии `2017-10-01`</span><span class="sxs-lookup"><span data-stu-id="886c3-110">Updated resource management to point to `2017-10-01` API version</span></span>
* <span data-ttu-id="886c3-111">Изменение номера SKU BYOS-хранилища на "Классический"</span><span class="sxs-lookup"><span data-stu-id="886c3-111">Changed 'bring your own storage' SKU to Classic</span></span>
* <span data-ttu-id="886c3-112">Переименование номеров SKU реестра на "Базовый", "Стандартный" и "Премиум"</span><span class="sxs-lookup"><span data-stu-id="886c3-112">Renamed registry SKUs to Basic, Standard, and Premium</span></span>

### <a name="acs"></a><span data-ttu-id="886c3-113">ACS</span><span class="sxs-lookup"><span data-stu-id="886c3-113">ACS</span></span>

* <span data-ttu-id="886c3-114">[ПРЕДВАРИЕТЛЬНАЯ ВЕРСИЯ] Добавление команд `az aks`</span><span class="sxs-lookup"><span data-stu-id="886c3-114">[PREVIEW] Added `az aks` commands</span></span>
* <span data-ttu-id="886c3-115">Исправление Kubernetes `get-credentials`</span><span class="sxs-lookup"><span data-stu-id="886c3-115">Fixed kubernetes `get-credentials`</span></span>

### <a name="appservice"></a><span data-ttu-id="886c3-116">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="886c3-116">Appservice</span></span>

* <span data-ttu-id="886c3-117">Исправление проблемы с недопустимыми скачанными журналами `webapp`</span><span class="sxs-lookup"><span data-stu-id="886c3-117">Fixed issue where downloaded `webapp` logs may be invalid</span></span>

### <a name="component"></a><span data-ttu-id="886c3-118">Компонент</span><span class="sxs-lookup"><span data-stu-id="886c3-118">Component</span></span>

* <span data-ttu-id="886c3-119">Добавление более понятного сообщения об устаревании для всех установщиков, а также запроса на подтверждение</span><span class="sxs-lookup"><span data-stu-id="886c3-119">Added clearer deprecation message for all installers and confirmation prompt</span></span>

### <a name="monitor"></a><span data-ttu-id="886c3-120">Монитор</span><span class="sxs-lookup"><span data-stu-id="886c3-120">Monitor</span></span>

* <span data-ttu-id="886c3-121">Добавлены команды `action-group`.</span><span class="sxs-lookup"><span data-stu-id="886c3-121">Added `action-group` commands</span></span>

### <a name="resource"></a><span data-ttu-id="886c3-122">Ресурс</span><span class="sxs-lookup"><span data-stu-id="886c3-122">Resource</span></span>

* <span data-ttu-id="886c3-123">Исправление несовместимости с самой последней версии зависимости msrest в `group export`</span><span class="sxs-lookup"><span data-stu-id="886c3-123">Fixed incompatibility with most recent version of msrest dependency in `group export`</span></span>
* <span data-ttu-id="886c3-124">Исправление `policy assignment create` для работы с определениями встроенных политик и наборов политик</span><span class="sxs-lookup"><span data-stu-id="886c3-124">Fixed `policy assignment create` to work with built in policy definitions and policy set definitions</span></span>

### <a name="vm"></a><span data-ttu-id="886c3-125">ВМ</span><span class="sxs-lookup"><span data-stu-id="886c3-125">VM</span></span>

* <span data-ttu-id="886c3-126">Добавлен аргумент `--accelerated-networking` для команды `vmss create`</span><span class="sxs-lookup"><span data-stu-id="886c3-126">Added `--accelerated-networking` argument to `vmss create`</span></span>


## <a name="october-9-2017"></a><span data-ttu-id="886c3-127">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-127">October 9, 2017</span></span>

<span data-ttu-id="886c3-128">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="886c3-128">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="886c3-129">Core</span><span class="sxs-lookup"><span data-stu-id="886c3-129">Core</span></span>

* <span data-ttu-id="886c3-130">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="886c3-130">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="886c3-131">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="886c3-131">Appservice</span></span>

* <span data-ttu-id="886c3-132">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-132">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="886c3-133">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="886c3-133">Batch</span></span>

* <span data-ttu-id="886c3-134">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="886c3-134">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="886c3-135">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="886c3-135">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="886c3-136">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="886c3-136">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="886c3-137">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="886c3-137">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="886c3-138">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="886c3-138">Batchai</span></span>

* <span data-ttu-id="886c3-139">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="886c3-139">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="886c3-140">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="886c3-140">Keyvault</span></span>

* <span data-ttu-id="886c3-141">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="886c3-141">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="886c3-142">(#4448)</span><span class="sxs-lookup"><span data-stu-id="886c3-142">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="886c3-143">Сеть</span><span class="sxs-lookup"><span data-stu-id="886c3-143">Network</span></span>

* <span data-ttu-id="886c3-144">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="886c3-144">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="886c3-145">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="886c3-145">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="886c3-146">Ресурс</span><span class="sxs-lookup"><span data-stu-id="886c3-146">Resource</span></span>

* <span data-ttu-id="886c3-147">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="886c3-147">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="886c3-148">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="886c3-148">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="886c3-149">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="886c3-149">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="886c3-150">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="886c3-150">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="886c3-151">SQL</span><span class="sxs-lookup"><span data-stu-id="886c3-151">Sql</span></span>

* <span data-ttu-id="886c3-152">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="886c3-152">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="886c3-153">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="886c3-153">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="886c3-154">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="886c3-154">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="886c3-155">Хранилище</span><span class="sxs-lookup"><span data-stu-id="886c3-155">Storage</span></span>

* <span data-ttu-id="886c3-156">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="886c3-156">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="886c3-157">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="886c3-157">Vm</span></span>

* <span data-ttu-id="886c3-158">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="886c3-158">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="886c3-159">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-159">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="886c3-160">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="886c3-160">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="886c3-161">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-161">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="886c3-162">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="886c3-162">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="886c3-163">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-163">September 22, 2017</span></span>

<span data-ttu-id="886c3-164">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="886c3-164">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="886c3-165">Ресурс</span><span class="sxs-lookup"><span data-stu-id="886c3-165">Resource</span></span>

* <span data-ttu-id="886c3-166">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="886c3-166">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="886c3-167">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="886c3-167">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="886c3-168">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="886c3-168">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="886c3-169">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="886c3-169">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="886c3-170">Сеть</span><span class="sxs-lookup"><span data-stu-id="886c3-170">Network</span></span>

* <span data-ttu-id="886c3-171">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="886c3-171">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="886c3-172">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="886c3-172">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="886c3-173">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="886c3-173">Added `asg` application security group commands</span></span>
* <span data-ttu-id="886c3-174">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="886c3-174">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="886c3-175">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="886c3-175">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="886c3-176">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="886c3-176">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="886c3-177">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="886c3-177">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="886c3-178">Хранилище</span><span class="sxs-lookup"><span data-stu-id="886c3-178">Storage</span></span>

* <span data-ttu-id="886c3-179">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="886c3-179">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="886c3-180">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="886c3-180">Eventgrid</span></span>

* <span data-ttu-id="886c3-181">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="886c3-181">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="886c3-182">SQL</span><span class="sxs-lookup"><span data-stu-id="886c3-182">SQL</span></span>

* <span data-ttu-id="886c3-183">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="886c3-183">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="886c3-184">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="886c3-184">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="886c3-185">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="886c3-185">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="886c3-186">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="886c3-186">Keyvault</span></span>

* <span data-ttu-id="886c3-187">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="886c3-187">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="886c3-188">ВМ</span><span class="sxs-lookup"><span data-stu-id="886c3-188">VM</span></span>

* <span data-ttu-id="886c3-189">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="886c3-189">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="886c3-190">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="886c3-190">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="886c3-191">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="886c3-191">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="886c3-192">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="886c3-192">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="886c3-193">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="886c3-193">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="886c3-194">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="886c3-194">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="886c3-195">ACS</span><span class="sxs-lookup"><span data-stu-id="886c3-195">ACS</span></span>

* <span data-ttu-id="886c3-196">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="886c3-196">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="886c3-197">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="886c3-197">Appservice</span></span>

* <span data-ttu-id="886c3-198">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="886c3-198">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="886c3-199">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="886c3-199">Backup</span></span>

* <span data-ttu-id="886c3-200">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="886c3-200">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="886c3-201">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-201">September 11, 2017</span></span>

<span data-ttu-id="886c3-202">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="886c3-202">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="886c3-203">Core</span><span class="sxs-lookup"><span data-stu-id="886c3-203">Core</span></span>

* <span data-ttu-id="886c3-204">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="886c3-204">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="886c3-205">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="886c3-205">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="886c3-206">ACS</span><span class="sxs-lookup"><span data-stu-id="886c3-206">Acs</span></span>

* <span data-ttu-id="886c3-207">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="886c3-207">Added `acs list-locations` command</span></span>
* <span data-ttu-id="886c3-208">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="886c3-208">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="886c3-209">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="886c3-209">Appservice</span></span>

* <span data-ttu-id="886c3-210">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="886c3-210">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="886c3-211">CDN</span><span class="sxs-lookup"><span data-stu-id="886c3-211">CDN</span></span>

* <span data-ttu-id="886c3-212">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-212">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="886c3-213">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="886c3-213">Extension</span></span>

* <span data-ttu-id="886c3-214">Первый выпуск.</span><span class="sxs-lookup"><span data-stu-id="886c3-214">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="886c3-215">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="886c3-215">Keyvault</span></span>

* <span data-ttu-id="886c3-216">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="886c3-216">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="886c3-217">Сеть</span><span class="sxs-lookup"><span data-stu-id="886c3-217">Network</span></span>

* <span data-ttu-id="886c3-218">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="886c3-218">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="886c3-219">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-219">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="886c3-220">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-220">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="886c3-221">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-221">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="886c3-222">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-222">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="886c3-223">Ресурс</span><span class="sxs-lookup"><span data-stu-id="886c3-223">Resource</span></span>

* <span data-ttu-id="886c3-224">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-224">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="886c3-225">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-225">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="886c3-226">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="886c3-226">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="886c3-227">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="886c3-227">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="886c3-228">SQL</span><span class="sxs-lookup"><span data-stu-id="886c3-228">SQL</span></span>

* <span data-ttu-id="886c3-229">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="886c3-229">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="886c3-230">ВМ</span><span class="sxs-lookup"><span data-stu-id="886c3-230">VM</span></span>

* <span data-ttu-id="886c3-231">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="886c3-231">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="886c3-232">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="886c3-232">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="886c3-233">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-233">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="886c3-234">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="886c3-234">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="886c3-235">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="886c3-235">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="886c3-236">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-236">August 31, 2017</span></span>

<span data-ttu-id="886c3-237">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="886c3-237">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="886c3-238">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="886c3-238">Keyvault</span></span>

* <span data-ttu-id="886c3-239">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="886c3-239">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="886c3-240">Sf</span><span class="sxs-lookup"><span data-stu-id="886c3-240">Sf</span></span>

* <span data-ttu-id="886c3-241">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="886c3-241">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="886c3-242">Хранилище</span><span class="sxs-lookup"><span data-stu-id="886c3-242">Storage</span></span>

* <span data-ttu-id="886c3-243">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="886c3-243">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="886c3-244">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="886c3-244">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="886c3-245">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-245">August 28, 2017</span></span>

<span data-ttu-id="886c3-246">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="886c3-246">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="886c3-247">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="886c3-247">CLI</span></span>

* <span data-ttu-id="886c3-248">К параметру `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="886c3-248">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="886c3-249">ACS</span><span class="sxs-lookup"><span data-stu-id="886c3-249">ACS</span></span>

* <span data-ttu-id="886c3-250">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="886c3-250">Corrected preview regions.</span></span>
* <span data-ttu-id="886c3-251">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="886c3-251">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="886c3-252">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="886c3-252">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="886c3-253">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="886c3-253">Appservice</span></span>

* <span data-ttu-id="886c3-254">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="886c3-254">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="886c3-255">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="886c3-255">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="886c3-256">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="886c3-256">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="886c3-257">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="886c3-257">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="886c3-258">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="886c3-258">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="886c3-259">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="886c3-259">IoT</span></span>

* <span data-ttu-id="886c3-260">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="886c3-260">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="886c3-261">Сеть</span><span class="sxs-lookup"><span data-stu-id="886c3-261">Network</span></span>

* <span data-ttu-id="886c3-262">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="886c3-262">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="886c3-263">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="886c3-263">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="886c3-264">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="886c3-264">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="886c3-265">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-265">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="886c3-266">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-266">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="886c3-267">Профиль</span><span class="sxs-lookup"><span data-stu-id="886c3-267">Profile</span></span>

* <span data-ttu-id="886c3-268">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="886c3-268">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="886c3-269">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="886c3-269">Service Fabric</span></span>

* <span data-ttu-id="886c3-270">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="886c3-270">Preview release</span></span>
* <span data-ttu-id="886c3-271">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="886c3-271">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="886c3-272">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="886c3-272">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="886c3-273">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="886c3-273">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="886c3-274">Хранилище</span><span class="sxs-lookup"><span data-stu-id="886c3-274">Storage</span></span>

* <span data-ttu-id="886c3-275">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="886c3-275">Enabled setting blob tier</span></span>
* <span data-ttu-id="886c3-276">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="886c3-276">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="886c3-277">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="886c3-277">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="886c3-278">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="886c3-278">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="886c3-279">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-279">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="886c3-280">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="886c3-280">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="886c3-281">ВМ</span><span class="sxs-lookup"><span data-stu-id="886c3-281">VM</span></span>

* <span data-ttu-id="886c3-282">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="886c3-282">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="886c3-283">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-283">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="886c3-284">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="886c3-284">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="886c3-285">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="886c3-285">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="886c3-286">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="886c3-286">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="886c3-287">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-287">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="886c3-288">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-288">August 15, 2017</span></span>

<span data-ttu-id="886c3-289">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="886c3-289">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="886c3-290">ACS</span><span class="sxs-lookup"><span data-stu-id="886c3-290">ACS</span></span>

* <span data-ttu-id="886c3-291">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="886c3-291">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="886c3-292">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="886c3-292">Appservice</span></span>

* <span data-ttu-id="886c3-293">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="886c3-293">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="886c3-294">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="886c3-294">Event Grid</span></span>

* <span data-ttu-id="886c3-295">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="886c3-295">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="886c3-296">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-296">August 11, 2017</span></span>

<span data-ttu-id="886c3-297">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="886c3-297">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="886c3-298">ACS</span><span class="sxs-lookup"><span data-stu-id="886c3-298">ACS</span></span>

* <span data-ttu-id="886c3-299">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="886c3-299">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="886c3-300">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="886c3-300">Batch</span></span>

* <span data-ttu-id="886c3-301">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="886c3-301">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="886c3-302">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="886c3-302">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="886c3-303">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="886c3-303">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="886c3-304">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="886c3-304">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="886c3-305">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="886c3-305">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="886c3-306">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="886c3-306">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="886c3-307">Компонент</span><span class="sxs-lookup"><span data-stu-id="886c3-307">Component</span></span>

* <span data-ttu-id="886c3-308">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="886c3-308">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="886c3-309">Контейнер</span><span class="sxs-lookup"><span data-stu-id="886c3-309">Container</span></span>

* <span data-ttu-id="886c3-310">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="886c3-310">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="886c3-311">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="886c3-311">Data Lake Store</span></span>

* <span data-ttu-id="886c3-312">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="886c3-312">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="886c3-313">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="886c3-313">Event Grid</span></span>

* <span data-ttu-id="886c3-314">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="886c3-314">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="886c3-315">Сеть</span><span class="sxs-lookup"><span data-stu-id="886c3-315">Network</span></span>

* <span data-ttu-id="886c3-316">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="886c3-316">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="886c3-317">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="886c3-317">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="886c3-318">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="886c3-318">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="886c3-319">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="886c3-319">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="886c3-320">Профиль</span><span class="sxs-lookup"><span data-stu-id="886c3-320">Profile</span></span>

* <span data-ttu-id="886c3-321">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="886c3-321">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="886c3-322">Хранилище</span><span class="sxs-lookup"><span data-stu-id="886c3-322">Storage</span></span>

* <span data-ttu-id="886c3-323">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="886c3-323">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="886c3-324">ВМ</span><span class="sxs-lookup"><span data-stu-id="886c3-324">VM</span></span>

* <span data-ttu-id="886c3-325">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="886c3-325">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="886c3-326">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="886c3-326">Exposed `list-skus` command</span></span>
* <span data-ttu-id="886c3-327">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="886c3-327">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="886c3-328">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="886c3-328">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="886c3-329">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="886c3-329">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="886c3-330">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-330">July 28, 2017</span></span>

<span data-ttu-id="886c3-331">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="886c3-331">Version 2.0.12</span></span>

* <span data-ttu-id="886c3-332">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="886c3-332">Added container commands</span></span>
* <span data-ttu-id="886c3-333">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="886c3-333">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="886c3-334">Core</span><span class="sxs-lookup"><span data-stu-id="886c3-334">Core</span></span>

* <span data-ttu-id="886c3-335">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="886c3-335">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="886c3-336">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="886c3-336">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="886c3-337">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="886c3-337">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="886c3-338">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="886c3-338">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="886c3-339">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="886c3-339">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="886c3-340">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="886c3-340">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="886c3-341">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="886c3-341">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="886c3-342">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="886c3-342">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="886c3-343">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="886c3-343">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="886c3-344">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="886c3-344">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="886c3-345">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="886c3-345">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="886c3-346">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="886c3-346">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="886c3-347">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="886c3-347">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="886c3-348">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="886c3-348">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="886c3-349">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="886c3-349">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="886c3-350">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="886c3-350">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="886c3-351">ACR</span><span class="sxs-lookup"><span data-stu-id="886c3-351">ACR</span></span>

* <span data-ttu-id="886c3-352">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="886c3-352">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="886c3-353">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="886c3-353">Support SKU update for managed registries</span></span>
* <span data-ttu-id="886c3-354">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="886c3-354">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="886c3-355">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="886c3-355">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="886c3-356">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="886c3-356">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="886c3-357">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="886c3-357">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="886c3-358">ACS</span><span class="sxs-lookup"><span data-stu-id="886c3-358">ACS</span></span>

* <span data-ttu-id="886c3-359">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="886c3-359">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="886c3-360">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="886c3-360">Appservice</span></span>

* <span data-ttu-id="886c3-361">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="886c3-361">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="886c3-362">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="886c3-362">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="886c3-363">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="886c3-363">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="886c3-364">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="886c3-364">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="886c3-365">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="886c3-365">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="886c3-366">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="886c3-366">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="886c3-367">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="886c3-367">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="886c3-368">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="886c3-368">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="886c3-369">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="886c3-369">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="886c3-370">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="886c3-370">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="886c3-371">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="886c3-371">Batch</span></span>

* <span data-ttu-id="886c3-372">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="886c3-372">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="886c3-373">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="886c3-373">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="886c3-374">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="886c3-374">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="886c3-375">CDN</span><span class="sxs-lookup"><span data-stu-id="886c3-375">CDN</span></span>

* <span data-ttu-id="886c3-376">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="886c3-376">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="886c3-377">Облако</span><span class="sxs-lookup"><span data-stu-id="886c3-377">Cloud</span></span>

* <span data-ttu-id="886c3-378">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="886c3-378">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="886c3-379">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="886c3-379">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="886c3-380">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="886c3-380">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="886c3-381">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="886c3-381">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="886c3-382">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="886c3-382">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="886c3-383">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="886c3-383">CosmosDB</span></span>

* <span data-ttu-id="886c3-384">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="886c3-384">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="886c3-385">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="886c3-385">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="886c3-386">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="886c3-386">Data Lake Analytics</span></span>

* <span data-ttu-id="886c3-387">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="886c3-387">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="886c3-388">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="886c3-388">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="886c3-389">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="886c3-389">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="886c3-390">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="886c3-390">Data Lake Store</span></span>

* <span data-ttu-id="886c3-391">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-391">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="886c3-392">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="886c3-392">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="886c3-393">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="886c3-393">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="886c3-394">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="886c3-394">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="886c3-395">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="886c3-395">Interactive</span></span>

* <span data-ttu-id="886c3-396">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="886c3-396">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="886c3-397">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="886c3-397">Increased test coverage</span></span>
* <span data-ttu-id="886c3-398">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="886c3-398">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="886c3-399">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="886c3-399">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="886c3-400">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="886c3-400">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="886c3-401">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="886c3-401">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="886c3-402">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="886c3-402">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="886c3-403">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="886c3-403">Added `--progress` flag</span></span>
* <span data-ttu-id="886c3-404">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="886c3-404">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="886c3-405">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="886c3-405">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="886c3-406">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="886c3-406">IoT</span></span>

* <span data-ttu-id="886c3-407">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="886c3-407">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="886c3-408">(3934).</span><span class="sxs-lookup"><span data-stu-id="886c3-408">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="886c3-409">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="886c3-409">Key vault</span></span>

* <span data-ttu-id="886c3-410">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="886c3-410">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="886c3-411">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="886c3-411">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="886c3-412">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="886c3-412">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="886c3-413">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="886c3-413">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="886c3-414">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="886c3-414">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="886c3-415">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="886c3-415">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="886c3-416">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="886c3-416">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="886c3-417">(3307).</span><span class="sxs-lookup"><span data-stu-id="886c3-417">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="886c3-418">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="886c3-418">Lab</span></span>

* <span data-ttu-id="886c3-419">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="886c3-419">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="886c3-420">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="886c3-420">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="886c3-421">Монитор</span><span class="sxs-lookup"><span data-stu-id="886c3-421">Monitor</span></span>

* <span data-ttu-id="886c3-422">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="886c3-422">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="886c3-423">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="886c3-423">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="886c3-424">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="886c3-424">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="886c3-425">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="886c3-425">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="886c3-426">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="886c3-426">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="886c3-427">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="886c3-427">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="886c3-428">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="886c3-428">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="886c3-429">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="886c3-429">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="886c3-430">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="886c3-430">`location` no longer required</span></span>
  * <span data-ttu-id="886c3-431">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="886c3-431">Add name and ID support for target</span></span>
  * <span data-ttu-id="886c3-432">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="886c3-432">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="886c3-433">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="886c3-433">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="886c3-434">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="886c3-434">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="886c3-435">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="886c3-435">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="886c3-436">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="886c3-436">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="886c3-437">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-437">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="886c3-438">Сеть</span><span class="sxs-lookup"><span data-stu-id="886c3-438">Network</span></span>

* <span data-ttu-id="886c3-439">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="886c3-439">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="886c3-440">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-440">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="886c3-441">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="886c3-441">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="886c3-442">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="886c3-442">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="886c3-443">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-443">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="886c3-444">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="886c3-444">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="886c3-445">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="886c3-445">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="886c3-446">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="886c3-446">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="886c3-447">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="886c3-447">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="886c3-448">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="886c3-448">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="886c3-449">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-449">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="886c3-450">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="886c3-450">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="886c3-451">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="886c3-451">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="886c3-452">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-452">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="886c3-453">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-453">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="886c3-454">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-454">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="886c3-455">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="886c3-455">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="886c3-456">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="886c3-456">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="886c3-457">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-457">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="886c3-458">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-458">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="886c3-459">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-459">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="886c3-460">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="886c3-460">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="886c3-461">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="886c3-461">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="886c3-462">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="886c3-462">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="886c3-463">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="886c3-463">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="886c3-464">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="886c3-464">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="886c3-465">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="886c3-465">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="886c3-466">Профиль</span><span class="sxs-lookup"><span data-stu-id="886c3-466">Profile</span></span>

* <span data-ttu-id="886c3-467">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="886c3-467">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="886c3-468">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="886c3-468">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="886c3-469">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="886c3-469">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="886c3-470">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="886c3-470">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="886c3-471">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="886c3-471">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="886c3-472">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="886c3-472">RDBMS</span></span>

* <span data-ttu-id="886c3-473">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="886c3-473">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="886c3-474">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="886c3-474">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="886c3-475">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="886c3-475">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="886c3-476">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="886c3-476">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="886c3-477">Ресурс</span><span class="sxs-lookup"><span data-stu-id="886c3-477">Resource</span></span>

* <span data-ttu-id="886c3-478">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-478">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="886c3-479">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="886c3-479">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="886c3-480">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="886c3-480">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="886c3-481">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="886c3-481">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="886c3-482">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="886c3-482">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="886c3-483">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="886c3-483">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="886c3-484">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="886c3-484">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="886c3-485">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="886c3-485">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="886c3-486">Роль</span><span class="sxs-lookup"><span data-stu-id="886c3-486">Role</span></span>

* <span data-ttu-id="886c3-487">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="886c3-487">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="886c3-488">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="886c3-488">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="886c3-489">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="886c3-489">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="886c3-490">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="886c3-490">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="886c3-491">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="886c3-491">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="886c3-492">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="886c3-492">Service Fabric</span></span>
* <span data-ttu-id="886c3-493">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="886c3-493">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="886c3-494">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="886c3-494">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="886c3-495">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="886c3-495">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="886c3-496">SQL</span><span class="sxs-lookup"><span data-stu-id="886c3-496">SQL</span></span>

* <span data-ttu-id="886c3-497">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-497">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="886c3-498">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="886c3-498">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="886c3-499">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="886c3-499">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="886c3-500">Хранилище</span><span class="sxs-lookup"><span data-stu-id="886c3-500">Storage</span></span>

* <span data-ttu-id="886c3-501">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="886c3-501">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="886c3-502">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="886c3-502">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="886c3-503">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="886c3-503">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="886c3-504">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="886c3-504">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="886c3-505">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="886c3-505">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="886c3-506">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="886c3-506">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="886c3-507">ВМ</span><span class="sxs-lookup"><span data-stu-id="886c3-507">VM</span></span>

* <span data-ttu-id="886c3-508">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="886c3-508">Support configuring nsg</span></span>
* <span data-ttu-id="886c3-509">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="886c3-509">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="886c3-510">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="886c3-510">Support managed service identities</span></span>
* <span data-ttu-id="886c3-511">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="886c3-511">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="886c3-512">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="886c3-512">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="886c3-513">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-513">May 10, 2017</span></span>

<span data-ttu-id="886c3-514">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="886c3-514">Version 2.0.6</span></span>

* <span data-ttu-id="886c3-515">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="886c3-515">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="886c3-516">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="886c3-516">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="886c3-517">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="886c3-517">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="886c3-518">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="886c3-518">Include Cognitive Services module.</span></span>
* <span data-ttu-id="886c3-519">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="886c3-519">Include Service Fabric module.</span></span>
* <span data-ttu-id="886c3-520">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="886c3-520">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="886c3-521">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="886c3-521">Add support for CDN commands.</span></span>
* <span data-ttu-id="886c3-522">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="886c3-522">Remove Container module.</span></span>
* <span data-ttu-id="886c3-523">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="886c3-523">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="886c3-524">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="886c3-524">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="886c3-525">Core</span><span class="sxs-lookup"><span data-stu-id="886c3-525">Core</span></span>

* <span data-ttu-id="886c3-526">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="886c3-526">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="886c3-527">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="886c3-527">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="886c3-528">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="886c3-528">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="886c3-529">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="886c3-529">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="886c3-530">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="886c3-530">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="886c3-531">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="886c3-531">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="886c3-532">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="886c3-532">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="886c3-533">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="886c3-533">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="886c3-534">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="886c3-534">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="886c3-535">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="886c3-535">core: Improved performance</span></span>
* <span data-ttu-id="886c3-536">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="886c3-536">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="886c3-537">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="886c3-537">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="886c3-538">ACS</span><span class="sxs-lookup"><span data-stu-id="886c3-538">ACS</span></span>

* <span data-ttu-id="886c3-539">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="886c3-539">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="886c3-540">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="886c3-540">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="886c3-541">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="886c3-541">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="886c3-542">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="886c3-542">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="886c3-543">AppService</span><span class="sxs-lookup"><span data-stu-id="886c3-543">AppService</span></span>

* <span data-ttu-id="886c3-544">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="886c3-544">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="886c3-545">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="886c3-545">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="886c3-546">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="886c3-546">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="886c3-547">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="886c3-547">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="886c3-548">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="886c3-548">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="886c3-549">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="886c3-549">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="886c3-550">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="886c3-550">support slot swap with preview</span></span>
* <span data-ttu-id="886c3-551">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="886c3-551">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="886c3-552">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="886c3-552">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="886c3-553">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="886c3-553">CosmosDB</span></span>

* <span data-ttu-id="886c3-554">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="886c3-554">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="886c3-555">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="886c3-555">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="886c3-556">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="886c3-556">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="886c3-557">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="886c3-557">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="886c3-558">Аналитика озера данных</span><span class="sxs-lookup"><span data-stu-id="886c3-558">Data Lake Analytics</span></span>

* <span data-ttu-id="886c3-559">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="886c3-559">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="886c3-560">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="886c3-560">Add support for new catalog item type: package.</span></span> <span data-ttu-id="886c3-561">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="886c3-561">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="886c3-562">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="886c3-562">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="886c3-563">Таблица</span><span class="sxs-lookup"><span data-stu-id="886c3-563">Table</span></span>
  * <span data-ttu-id="886c3-564">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="886c3-564">Table valued function</span></span>
  * <span data-ttu-id="886c3-565">Просмотр</span><span class="sxs-lookup"><span data-stu-id="886c3-565">View</span></span>
  * <span data-ttu-id="886c3-566">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="886c3-566">Table Statistics.</span></span> <span data-ttu-id="886c3-567">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="886c3-567">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="886c3-568">Хранилище озера данных</span><span class="sxs-lookup"><span data-stu-id="886c3-568">Data Lake Store</span></span>

* <span data-ttu-id="886c3-569">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="886c3-569">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="886c3-570">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="886c3-570">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="886c3-571">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="886c3-571">missed help for access show.</span></span> <span data-ttu-id="886c3-572">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="886c3-572">adding it.</span></span> <span data-ttu-id="886c3-573">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="886c3-573">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="886c3-574">Поиск</span><span class="sxs-lookup"><span data-stu-id="886c3-574">Find</span></span>

* <span data-ttu-id="886c3-575">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="886c3-575">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="886c3-576">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="886c3-576">KeyVault</span></span>

* <span data-ttu-id="886c3-577">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="886c3-577">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="886c3-578">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="886c3-578">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="886c3-579">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="886c3-579">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="886c3-580">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="886c3-580">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="886c3-581">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="886c3-581">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="886c3-582">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="886c3-582">Lab</span></span>

* <span data-ttu-id="886c3-583">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="886c3-583">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="886c3-584">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="886c3-584">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="886c3-585">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="886c3-585">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="886c3-586">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="886c3-586">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="886c3-587">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="886c3-587">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="886c3-588">Монитор</span><span class="sxs-lookup"><span data-stu-id="886c3-588">Monitor</span></span>

* <span data-ttu-id="886c3-589">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="886c3-589">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="886c3-590">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="886c3-590">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="886c3-591">Сеть</span><span class="sxs-lookup"><span data-stu-id="886c3-591">Network</span></span>

* <span data-ttu-id="886c3-592">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="886c3-592">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="886c3-593">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-593">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="886c3-594">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="886c3-594">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="886c3-595">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="886c3-595">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="886c3-596">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="886c3-596">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="886c3-597">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="886c3-597">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="886c3-598">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="886c3-598">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="886c3-599">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="886c3-599">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="886c3-600">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="886c3-600">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="886c3-601">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="886c3-601">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="886c3-602">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="886c3-602">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="886c3-603">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-603">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="886c3-604">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="886c3-604">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="886c3-605">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="886c3-605">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="886c3-606">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="886c3-606">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="886c3-607">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="886c3-607">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="886c3-608">Профиль</span><span class="sxs-lookup"><span data-stu-id="886c3-608">Profile</span></span>

* <span data-ttu-id="886c3-609">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="886c3-609">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="886c3-610">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="886c3-610">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="886c3-611">Redis</span><span class="sxs-lookup"><span data-stu-id="886c3-611">Redis</span></span>

* <span data-ttu-id="886c3-612">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="886c3-612">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="886c3-613">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="886c3-613">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="886c3-614">Ресурс</span><span class="sxs-lookup"><span data-stu-id="886c3-614">Resource</span></span>

* <span data-ttu-id="886c3-615">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="886c3-615">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="886c3-616">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="886c3-616">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="886c3-617">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="886c3-617">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="886c3-618">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="886c3-618">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="886c3-619">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="886c3-619">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="886c3-620">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="886c3-620">Add docs for az lock update.</span></span> <span data-ttu-id="886c3-621">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="886c3-621">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="886c3-622">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="886c3-622">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="886c3-623">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="886c3-623">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="886c3-624">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="886c3-624">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="886c3-625">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="886c3-625">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="886c3-626">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="886c3-626">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="886c3-627">Роль</span><span class="sxs-lookup"><span data-stu-id="886c3-627">Role</span></span>

* <span data-ttu-id="886c3-628">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="886c3-628">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="886c3-629">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="886c3-629">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="886c3-630">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="886c3-630">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="886c3-631">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="886c3-631">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="886c3-632">SQL</span><span class="sxs-lookup"><span data-stu-id="886c3-632">SQL</span></span>

* <span data-ttu-id="886c3-633">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="886c3-633">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="886c3-634">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="886c3-634">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="886c3-635">Хранилище</span><span class="sxs-lookup"><span data-stu-id="886c3-635">Storage</span></span>

* <span data-ttu-id="886c3-636">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="886c3-636">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="886c3-637">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="886c3-637">Add support for incremental blob copy</span></span>
* <span data-ttu-id="886c3-638">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="886c3-638">Add support for large block blob upload</span></span>
* <span data-ttu-id="886c3-639">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="886c3-639">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="886c3-640">ВМ</span><span class="sxs-lookup"><span data-stu-id="886c3-640">VM</span></span>

* <span data-ttu-id="886c3-641">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="886c3-641">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="886c3-642">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="886c3-642">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="886c3-643">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="886c3-643">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="886c3-644">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="886c3-644">az vm/vmss disk</span></span>
  3. <span data-ttu-id="886c3-645">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="886c3-645">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="886c3-646">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="886c3-646">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="886c3-647">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="886c3-647">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="886c3-648">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-648">April 3, 2017</span></span>

<span data-ttu-id="886c3-649">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="886c3-649">Version 2.0.2</span></span>

<span data-ttu-id="886c3-650">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="886c3-650">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="886c3-651">Core</span><span class="sxs-lookup"><span data-stu-id="886c3-651">Core</span></span>

* <span data-ttu-id="886c3-652">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="886c3-652">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="886c3-653">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="886c3-653">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="886c3-654">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="886c3-654">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="886c3-655">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="886c3-655">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="886c3-656">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="886c3-656">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="886c3-657">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="886c3-657">Add prompting for missing template parameters.</span></span> <span data-ttu-id="886c3-658">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="886c3-658">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="886c3-659">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="886c3-659">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="886c3-660">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="886c3-660">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="886c3-661">ACS</span><span class="sxs-lookup"><span data-stu-id="886c3-661">ACS</span></span>

* <span data-ttu-id="886c3-662">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="886c3-662">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="886c3-663">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="886c3-663">Add support for ssh key password prompting.</span></span> <span data-ttu-id="886c3-664">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="886c3-664">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="886c3-665">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="886c3-665">Add support for windows clusters.</span></span> <span data-ttu-id="886c3-666">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="886c3-666">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="886c3-667">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="886c3-667">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="886c3-668">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="886c3-668">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="886c3-669">AppService</span><span class="sxs-lookup"><span data-stu-id="886c3-669">AppService</span></span>

* <span data-ttu-id="886c3-670">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="886c3-670">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="886c3-671">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="886c3-671">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="886c3-672">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="886c3-672">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="886c3-673">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="886c3-673">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="886c3-674">DataLake</span><span class="sxs-lookup"><span data-stu-id="886c3-674">DataLake</span></span>

* <span data-ttu-id="886c3-675">Первоначальный выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="886c3-675">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="886c3-676">Первоначальный выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="886c3-676">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="886c3-677">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="886c3-677">DocuemntDB</span></span>

* <span data-ttu-id="886c3-678">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="886c3-678">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="886c3-679">ВМ</span><span class="sxs-lookup"><span data-stu-id="886c3-679">VM</span></span>

* <span data-ttu-id="886c3-680">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="886c3-680">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="886c3-681">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="886c3-681">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="886c3-682">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="886c3-682">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="886c3-683">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="886c3-683">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="886c3-684">Масштабируемый набор виртуальных машин: добавлена поддержка * для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="886c3-684">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="886c3-685">Добавлена команда --secrets для виртуальных машин и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="886c3-685">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="886c3-686">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="886c3-686">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="886c3-687">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="886c3-687">February 27, 2017</span></span>

<span data-ttu-id="886c3-688">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="886c3-688">Version 2.0.0</span></span>

<span data-ttu-id="886c3-689">Этот первый общедоступный выпуск Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="886c3-689">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="886c3-690">Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="886c3-690">General availability applies to these command modules:</span></span>
- <span data-ttu-id="886c3-691">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="886c3-691">Container Service (acs)</span></span>
- <span data-ttu-id="886c3-692">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="886c3-692">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="886c3-693">Сеть</span><span class="sxs-lookup"><span data-stu-id="886c3-693">Networking</span></span>
- <span data-ttu-id="886c3-694">Хранилище</span><span class="sxs-lookup"><span data-stu-id="886c3-694">Storage</span></span>

<span data-ttu-id="886c3-695">Эти командные модули могут использоваться в рабочих средах и поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания.</span><span class="sxs-lookup"><span data-stu-id="886c3-695">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="886c3-696">Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="886c3-696">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="886c3-697">Вы можете задавать вопросы на сайте [StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="886c3-697">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="886c3-698">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="886c3-698">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="886c3-699">Чтобы проверить версию интерфейса командной строки, используйте `az --version`.</span><span class="sxs-lookup"><span data-stu-id="886c3-699">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="886c3-700">В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="886c3-700">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="886c3-701">Некоторые командные модули имеют постфикс b*n* или rc*n*.</span><span class="sxs-lookup"><span data-stu-id="886c3-701">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="886c3-702">Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="886c3-702">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="886c3-703">У нас также есть предварительные ежедневные сборки интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="886c3-703">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="886c3-704">Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="886c3-704">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="886c3-705">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="886c3-705">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="886c3-706">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="886c3-706">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="886c3-707">обратившись к специалистам группы разработчиков продукта по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com);</span><span class="sxs-lookup"><span data-stu-id="886c3-707">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="886c3-708">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="886c3-708">Provide feedback from the command line with the `az feedback` command.</span></span>

