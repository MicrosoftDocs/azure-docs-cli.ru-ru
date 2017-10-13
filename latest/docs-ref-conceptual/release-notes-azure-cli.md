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
ms.openlocfilehash: 2ea9daa558200204750f19b5d22685587ff097ef
ms.sourcegitcommit: 376bc0601aba890630dadd55908c1a65ddf40f5a
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/11/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="4f4a2-104">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="4f4a2-104">Azure CLI 2.0 release notes</span></span>

## <a name="october-9-2017"></a><span data-ttu-id="4f4a2-105">9 октября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-105">October 9, 2017</span></span>

<span data-ttu-id="4f4a2-106">Версия 2.0.19</span><span class="sxs-lookup"><span data-stu-id="4f4a2-106">Version 2.0.19</span></span>

### <a name="core"></a><span data-ttu-id="4f4a2-107">Core</span><span class="sxs-lookup"><span data-stu-id="4f4a2-107">Core</span></span>

* <span data-ttu-id="4f4a2-108">В Azure Stack добавлена обработка URL-адресов центра ADFS с завершающей косой чертой.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-108">Added handling of ADFS authority URLs with a trailing slash to Azure Stack</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-109">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4f4a2-109">Appservice</span></span>

* <span data-ttu-id="4f4a2-110">Добавлена возможность общего обновления с помощью новой команды `webapp update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-110">Added generic update with new command `webapp update`</span></span>

### <a name="batch"></a><span data-ttu-id="4f4a2-111">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="4f4a2-111">Batch</span></span>

* <span data-ttu-id="4f4a2-112">Обновление до пакета SDK для пакетной службы версии 4.0.0</span><span class="sxs-lookup"><span data-stu-id="4f4a2-112">Updated to Batch SDK 4.0.0</span></span>
* <span data-ttu-id="4f4a2-113">Обновлен параметр `--image` для команды VirtualMachineConfiguration, обеспечивающий поддержку ссылок на образы ARM в дополнение к publish:offer:sku:version.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-113">Updated `--image` option of VirtualMachineConfiguration to support ARM image references in addition to publish:offer:sku:version</span></span>
* <span data-ttu-id="4f4a2-114">Добавлена поддержка новой модели расширений CLI для команд расширений пакетной службы.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-114">Added support for the new CLI extension model for Batch Extensions commands</span></span>
* <span data-ttu-id="4f4a2-115">Удалена поддержка пакетной службы для модели компонентов.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-115">Removed Batch support from the component model</span></span>

### <a name="batchai"></a><span data-ttu-id="4f4a2-116">Модуль искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="4f4a2-116">Batchai</span></span>

* <span data-ttu-id="4f4a2-117">Исходный выпуск модуля искусственного интеллекта пакетной службы</span><span class="sxs-lookup"><span data-stu-id="4f4a2-117">Initial release of Batch AI module</span></span>

### <a name="keyvault"></a><span data-ttu-id="4f4a2-118">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4f4a2-118">Keyvault</span></span>

* <span data-ttu-id="4f4a2-119">Исправлена проблема с аутентификацией Key Vault при использовании ADFS в Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-119">Fixed Key Vault authentication issue when using ADFS on Azure Stack.</span></span> [<span data-ttu-id="4f4a2-120">(#4448)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-120">(#4448)</span></span>](https://github.com/Azure/azure-cli/issues/4448)

### <a name="network"></a><span data-ttu-id="4f4a2-121">Сеть</span><span class="sxs-lookup"><span data-stu-id="4f4a2-121">Network</span></span>

* <span data-ttu-id="4f4a2-122">Аргумент `--server` для `application-gateway address-pool create` изменен на необязательный (разрешено использование пустых пулов адресов).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-122">Changed `--server` argument of `application-gateway address-pool create` to be optional, allowing for empty address pools</span></span>
* <span data-ttu-id="4f4a2-123">Обновлен элемент `traffic-manager` для поддержки последних функций.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-123">Updated `traffic-manager` to support latest features</span></span>

### <a name="resource"></a><span data-ttu-id="4f4a2-124">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4f4a2-124">Resource</span></span>

* <span data-ttu-id="4f4a2-125">Добавлена поддержка параметров `--resource-group/-g` для изменения имени группы ресурсов на `group`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-125">Added support for `--resource-group/-g` options for resource group name to `group`</span></span>
* <span data-ttu-id="4f4a2-126">Добавлены команды для `account lock` для работы с блокировками на уровне подписки.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-126">Added commands for `account lock` to work with subscription-level locks</span></span>
* <span data-ttu-id="4f4a2-127">Добавлены команды для `group lock` для работы с блокировками на уровне группы.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-127">Added commands for `group lock` to work with group-level locks</span></span>
* <span data-ttu-id="4f4a2-128">Добавлены команды для `resource lock` для работы с блокировками на уровне ресурса.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-128">Added commands for `resource lock` to work with resource-level locks</span></span>

### <a name="sql"></a><span data-ttu-id="4f4a2-129">SQL</span><span class="sxs-lookup"><span data-stu-id="4f4a2-129">Sql</span></span>

* <span data-ttu-id="4f4a2-130">Добавлена поддержка SQL TDE и BYOK TDE.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-130">Added support for SQL Transparent Data Encryption (TDE) and TDE with Bring Your Own Key</span></span>
* <span data-ttu-id="4f4a2-131">Добавлена команда `db list-deleted` и параметр `db restore --deleted-time` для поиска и восстановления удаленных баз данных.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-131">Added `db list-deleted` command and `db restore --deleted-time` parameter, allowing the ability to find and restore deleted databases</span></span>
* <span data-ttu-id="4f4a2-132">Добавлено `db op list` и `db op cancel` для отображения и отмены выполняющихся операций в базе данных.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-132">Added `db op list` and `db op cancel`, allowing the ability to list and cancel in-progress operations on database</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-133">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4f4a2-133">Storage</span></span>

* <span data-ttu-id="4f4a2-134">Добавлена поддержка моментальных снимков файловых ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-134">Added support for file share snapshot</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-135">Виртуальные машины</span><span class="sxs-lookup"><span data-stu-id="4f4a2-135">Vm</span></span>

* <span data-ttu-id="4f4a2-136">Исправлена ошибка в команде `vm show`, когда использование `-d` вызывало сбой отсутствующих частных IP-адресов.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-136">Fixed a bug in `vm show` where using `-d` caused a crash on missing private ip addresses</span></span>
* <span data-ttu-id="4f4a2-137">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка последовательного обновления для команды `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-137">[PREVIEW] Added support for rolling upgrade to `vmss create`</span></span>
* <span data-ttu-id="4f4a2-138">Добавлена поддержка обновления параметров шифрования с помощью команды `vm encryption enable`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-138">Added support for updating encryption settings with `vm encryption enable`</span></span>
* <span data-ttu-id="4f4a2-139">Добавлен параметр `--os-disk-size-gb` для команды `vm create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-139">Added `--os-disk-size-gb` parameter to `vm create`</span></span>
* <span data-ttu-id="4f4a2-140">Добавлен параметр `--license-type` для команды `vmss create` (для Windows).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-140">Added `--license-type` parameter for Windows to `vmss create`</span></span>


## <a name="september-22-2017"></a><span data-ttu-id="4f4a2-141">22 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-141">September 22, 2017</span></span>

<span data-ttu-id="4f4a2-142">Версия 2.0.18</span><span class="sxs-lookup"><span data-stu-id="4f4a2-142">Version 2.0.18</span></span>

### <a name="resource"></a><span data-ttu-id="4f4a2-143">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4f4a2-143">Resource</span></span>

* <span data-ttu-id="4f4a2-144">Добавлена поддержка отображения определений встроенных политик</span><span class="sxs-lookup"><span data-stu-id="4f4a2-144">Added support for showing built-in policy definitions</span></span>
* <span data-ttu-id="4f4a2-145">Добавлена поддержка параметра mode для создания определения политик</span><span class="sxs-lookup"><span data-stu-id="4f4a2-145">Added support mode parameter for creating policy definitions</span></span>
* <span data-ttu-id="4f4a2-146">Добавлена поддержка шаблонов и определений пользовательского интерфейса для команды `managedapp definition create`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-146">Added support for UI definitions and templates to `managedapp definition create`</span></span>
* <span data-ttu-id="4f4a2-147">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ] Изменен тип ресурса `managedapp` с `appliances` на `applications` и с `applianceDefinitions` на `applicationDefinitions`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-147">[BREAKING CHANGE] Changed `managedapp` resource type from `appliances` to `applications` and `applianceDefinitions` to `applicationDefinitions`</span></span>

### <a name="network"></a><span data-ttu-id="4f4a2-148">Сеть</span><span class="sxs-lookup"><span data-stu-id="4f4a2-148">Network</span></span>

* <span data-ttu-id="4f4a2-149">Добавлена поддержка зоны доступности для подкоманд `network lb` и `network public-ip`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-149">Added support for availability zone to `network lb` and `network public-ip` subcommands</span></span>
* <span data-ttu-id="4f4a2-150">Добавлена поддержка IPv6 (пиринг Майкрософт) для `express-route`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-150">Added support for IPv6 Microsoft Peering to `express-route`</span></span>
* <span data-ttu-id="4f4a2-151">Добавлены команды группы безопасности приложения `asg`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-151">Added `asg` application security group commands</span></span>
* <span data-ttu-id="4f4a2-152">Добавлен аргумент `--application-security-groups` для команды `nic [create|ip-config create|ip-config update]`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-152">Added `--application-security-groups` argument to `nic [create|ip-config create|ip-config update]`</span></span>
* <span data-ttu-id="4f4a2-153">Добавлены аргументы `--source-asgs` и `--destination-asgs` для команды `nsg rule [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-153">Added `--source-asgs` and `--destination-asgs` arguments to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4f4a2-154">Добавлены аргументы `--ddos-protection` и `--vm-protection` для команды `vnet [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-154">Added `--ddos-protection` and `--vm-protection` arguments to `vnet [create|update]`</span></span>
* <span data-ttu-id="4f4a2-155">Добавлены команды `network [vnet-gateway|vpn-client|show-url]`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-155">Added `network [vnet-gateway|vpn-client|show-url]` commands</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-156">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4f4a2-156">Storage</span></span>

* <span data-ttu-id="4f4a2-157">Исправлена проблема, когда команды `storage account network-rule` могут не работать после обновления пакета SDK</span><span class="sxs-lookup"><span data-stu-id="4f4a2-157">Fixed issue where `storage account network-rule` commands may fail after updating the SDK</span></span>

### <a name="eventgrid"></a><span data-ttu-id="4f4a2-158">Сетка событий</span><span class="sxs-lookup"><span data-stu-id="4f4a2-158">Eventgrid</span></span>

* <span data-ttu-id="4f4a2-159">Обновлен пакет SDK Python для службы "Сетка событий Azure" для использования новой версии API 2017-09-15-preview</span><span class="sxs-lookup"><span data-stu-id="4f4a2-159">Updated Azure Event Grid Python SDK to use newer API version "2017-09-15-preview"</span></span>

### <a name="sql"></a><span data-ttu-id="4f4a2-160">SQL</span><span class="sxs-lookup"><span data-stu-id="4f4a2-160">SQL</span></span>

* <span data-ttu-id="4f4a2-161">Аргумент `--resource-group` для команды `sql server list` сделан необязательным.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-161">Changed `sql server list` argument `--resource-group` to be optional.</span></span> <span data-ttu-id="4f4a2-162">Если он не указан, возвращаются все серверы SQL Server в подписке</span><span class="sxs-lookup"><span data-stu-id="4f4a2-162">If not specified, all sql servers in the subscription will be returned</span></span>
* <span data-ttu-id="4f4a2-163">Добавлен параметр `--no-wait` для команд `db [create|copy|restore|update|replica create|create|update]` и `dw [create|update]`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-163">Added `--no-wait` param to `db [create|copy|restore|update|replica create|create|update]` and `dw [create|update]`</span></span>

### <a name="keyvault"></a><span data-ttu-id="4f4a2-164">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4f4a2-164">Keyvault</span></span>

* <span data-ttu-id="4f4a2-165">Добавлена поддержка команд хранилища ключей за прокси-сервером</span><span class="sxs-lookup"><span data-stu-id="4f4a2-165">Added support for Keyvault commands from behind a proxy</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-166">ВМ</span><span class="sxs-lookup"><span data-stu-id="4f4a2-166">VM</span></span>

* <span data-ttu-id="4f4a2-167">Добавлена поддержка зоны доступности для команды `[vm|vmss|disk] create`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-167">Added for support to availability zone to `[vm|vmss|disk] create`</span></span>
* <span data-ttu-id="4f4a2-168">Исправлена проблема, когда использование аргумента `--app-gateway ID` с командой `vmss create` приводило к сбою</span><span class="sxs-lookup"><span data-stu-id="4f4a2-168">Fixed issue where using`--app-gateway ID` with `vmss create` would cause a failure</span></span>
* <span data-ttu-id="4f4a2-169">Добавлен аргумент `--asgs` для команды `vm create`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-169">Added `--asgs` argument to `vm create`</span></span>
* <span data-ttu-id="4f4a2-170">Добавлена поддержка выполнения команд на виртуальных машинах с помощью команды `vm run-command`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-170">Added support for running commands on VMs with `vm run-command`</span></span>
* <span data-ttu-id="4f4a2-171">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлена поддержка шифрования диска VMSS с помощью команды `vmss encryption`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-171">[PREVIEW] Added support for VMSS disk encryption with `vmss encryption`</span></span>
* <span data-ttu-id="4f4a2-172">Добавлена поддержка обслуживания виртуальных машин с помощью команды `vm perform-maintenance`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-172">Added support for performing maintenance on VMs with `vm perform-maintenance`</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-173">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-173">ACS</span></span>

* <span data-ttu-id="4f4a2-174">[ПРЕДВАРИТЕЛЬНАЯ ВЕРСИЯ] Добавлен аргумент `--orchestrator-release` для команды `acs create` для регионов служб ACS (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-174">[PREVIEW] Added `--orchestrator-release` argument to `acs create` for ACS preview regions</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-175">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4f4a2-175">Appservice</span></span>

* <span data-ttu-id="4f4a2-176">Добавлена возможность обновлять и отображать параметры аутентификации с помощью команды `webapp auth [update|show]`</span><span class="sxs-lookup"><span data-stu-id="4f4a2-176">Added ability to update and show authentication settings with `webapp auth [update|show]`</span></span>

### <a name="backup"></a><span data-ttu-id="4f4a2-177">Резервное копирование</span><span class="sxs-lookup"><span data-stu-id="4f4a2-177">Backup</span></span>

* <span data-ttu-id="4f4a2-178">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-178">Preview release</span></span>


## <a name="september-11-2017"></a><span data-ttu-id="4f4a2-179">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-179">September 11, 2017</span></span>

<span data-ttu-id="4f4a2-180">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="4f4a2-180">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="4f4a2-181">Core</span><span class="sxs-lookup"><span data-stu-id="4f4a2-181">Core</span></span>

* <span data-ttu-id="4f4a2-182">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-182">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="4f4a2-183">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-183">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-184">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-184">Acs</span></span>

* <span data-ttu-id="4f4a2-185">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-185">Added `acs list-locations` command</span></span>
* <span data-ttu-id="4f4a2-186">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-186">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-187">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4f4a2-187">Appservice</span></span>

* <span data-ttu-id="4f4a2-188">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-188">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="4f4a2-189">CDN</span><span class="sxs-lookup"><span data-stu-id="4f4a2-189">CDN</span></span>

* <span data-ttu-id="4f4a2-190">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-190">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="4f4a2-191">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="4f4a2-191">Extension</span></span>

* <span data-ttu-id="4f4a2-192">Первый выпуск.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-192">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="4f4a2-193">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4f4a2-193">Keyvault</span></span>

* <span data-ttu-id="4f4a2-194">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-194">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="4f4a2-195">Сеть</span><span class="sxs-lookup"><span data-stu-id="4f4a2-195">Network</span></span>

* <span data-ttu-id="4f4a2-196">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-196">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4f4a2-197">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-197">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="4f4a2-198">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-198">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="4f4a2-199">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-199">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4f4a2-200">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-200">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="4f4a2-201">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4f4a2-201">Resource</span></span>

* <span data-ttu-id="4f4a2-202">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-202">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="4f4a2-203">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-203">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="4f4a2-204">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-204">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="4f4a2-205">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-205">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="4f4a2-206">SQL</span><span class="sxs-lookup"><span data-stu-id="4f4a2-206">SQL</span></span>

* <span data-ttu-id="4f4a2-207">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-207">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-208">ВМ</span><span class="sxs-lookup"><span data-stu-id="4f4a2-208">VM</span></span>

* <span data-ttu-id="4f4a2-209">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-209">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="4f4a2-210">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-210">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="4f4a2-211">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-211">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="4f4a2-212">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-212">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="4f4a2-213">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-213">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="4f4a2-214">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-214">August 31, 2017</span></span>

<span data-ttu-id="4f4a2-215">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="4f4a2-215">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="4f4a2-216">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4f4a2-216">Keyvault</span></span>

* <span data-ttu-id="4f4a2-217">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-217">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="4f4a2-218">Sf</span><span class="sxs-lookup"><span data-stu-id="4f4a2-218">Sf</span></span>

* <span data-ttu-id="4f4a2-219">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-219">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-220">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4f4a2-220">Storage</span></span>

* <span data-ttu-id="4f4a2-221">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-221">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="4f4a2-222">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-222">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="4f4a2-223">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-223">August 28, 2017</span></span>

<span data-ttu-id="4f4a2-224">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="4f4a2-224">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="4f4a2-225">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="4f4a2-225">CLI</span></span>

* <span data-ttu-id="4f4a2-226">К параметру `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-226">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-227">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-227">ACS</span></span>

* <span data-ttu-id="4f4a2-228">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-228">Corrected preview regions.</span></span>
* <span data-ttu-id="4f4a2-229">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-229">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="4f4a2-230">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-230">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-231">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4f4a2-231">Appservice</span></span>

* <span data-ttu-id="4f4a2-232">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-232">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="4f4a2-233">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-233">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="4f4a2-234">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-234">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="4f4a2-235">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-235">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="4f4a2-236">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-236">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="4f4a2-237">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4f4a2-237">IoT</span></span>

* <span data-ttu-id="4f4a2-238">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-238">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="4f4a2-239">Сеть</span><span class="sxs-lookup"><span data-stu-id="4f4a2-239">Network</span></span>

* <span data-ttu-id="4f4a2-240">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-240">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="4f4a2-241">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-241">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="4f4a2-242">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-242">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="4f4a2-243">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-243">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="4f4a2-244">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-244">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="4f4a2-245">Профиль</span><span class="sxs-lookup"><span data-stu-id="4f4a2-245">Profile</span></span>

* <span data-ttu-id="4f4a2-246">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-246">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4f4a2-247">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4f4a2-247">Service Fabric</span></span>

* <span data-ttu-id="4f4a2-248">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-248">Preview release</span></span>
* <span data-ttu-id="4f4a2-249">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-249">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="4f4a2-250">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-250">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="4f4a2-251">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-251">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-252">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4f4a2-252">Storage</span></span>

* <span data-ttu-id="4f4a2-253">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-253">Enabled setting blob tier</span></span>
* <span data-ttu-id="4f4a2-254">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-254">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="4f4a2-255">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-255">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="4f4a2-256">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-256">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="4f4a2-257">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-257">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="4f4a2-258">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-258">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-259">ВМ</span><span class="sxs-lookup"><span data-stu-id="4f4a2-259">VM</span></span>

* <span data-ttu-id="4f4a2-260">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-260">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="4f4a2-261">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-261">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="4f4a2-262">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-262">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="4f4a2-263">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-263">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="4f4a2-264">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-264">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="4f4a2-265">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-265">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="4f4a2-266">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-266">August 15, 2017</span></span>

<span data-ttu-id="4f4a2-267">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="4f4a2-267">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-268">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-268">ACS</span></span>

* <span data-ttu-id="4f4a2-269">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-269">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-270">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4f4a2-270">Appservice</span></span>

* <span data-ttu-id="4f4a2-271">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-271">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="4f4a2-272">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="4f4a2-272">Event Grid</span></span>

* <span data-ttu-id="4f4a2-273">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-273">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="4f4a2-274">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-274">August 11, 2017</span></span>

<span data-ttu-id="4f4a2-275">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="4f4a2-275">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-276">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-276">ACS</span></span>

* <span data-ttu-id="4f4a2-277">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-277">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="4f4a2-278">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="4f4a2-278">Batch</span></span>

* <span data-ttu-id="4f4a2-279">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-279">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="4f4a2-280">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-280">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="4f4a2-281">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-281">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="4f4a2-282">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-282">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="4f4a2-283">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-283">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="4f4a2-284">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-284">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="4f4a2-285">Компонент</span><span class="sxs-lookup"><span data-stu-id="4f4a2-285">Component</span></span>

* <span data-ttu-id="4f4a2-286">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-286">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="4f4a2-287">Контейнер</span><span class="sxs-lookup"><span data-stu-id="4f4a2-287">Container</span></span>

* <span data-ttu-id="4f4a2-288">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-288">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="4f4a2-289">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4f4a2-289">Data Lake Store</span></span>

* <span data-ttu-id="4f4a2-290">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-290">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="4f4a2-291">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="4f4a2-291">Event Grid</span></span>

* <span data-ttu-id="4f4a2-292">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="4f4a2-292">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="4f4a2-293">Сеть</span><span class="sxs-lookup"><span data-stu-id="4f4a2-293">Network</span></span>

* <span data-ttu-id="4f4a2-294">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-294">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="4f4a2-295">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-295">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="4f4a2-296">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-296">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="4f4a2-297">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-297">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="4f4a2-298">Профиль</span><span class="sxs-lookup"><span data-stu-id="4f4a2-298">Profile</span></span>

* <span data-ttu-id="4f4a2-299">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-299">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-300">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4f4a2-300">Storage</span></span>

* <span data-ttu-id="4f4a2-301">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-301">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-302">ВМ</span><span class="sxs-lookup"><span data-stu-id="4f4a2-302">VM</span></span>

* <span data-ttu-id="4f4a2-303">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-303">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="4f4a2-304">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-304">Exposed `list-skus` command</span></span>
* <span data-ttu-id="4f4a2-305">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-305">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="4f4a2-306">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-306">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="4f4a2-307">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-307">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="4f4a2-308">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-308">July 28, 2017</span></span>

<span data-ttu-id="4f4a2-309">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="4f4a2-309">Version 2.0.12</span></span>

* <span data-ttu-id="4f4a2-310">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-310">Added container commands</span></span>
* <span data-ttu-id="4f4a2-311">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-311">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="4f4a2-312">Core</span><span class="sxs-lookup"><span data-stu-id="4f4a2-312">Core</span></span>

* <span data-ttu-id="4f4a2-313">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-313">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="4f4a2-314">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-314">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="4f4a2-315">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-315">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="4f4a2-316">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-316">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="4f4a2-317">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-317">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="4f4a2-318">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-318">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="4f4a2-319">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-319">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4f4a2-320">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-320">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="4f4a2-321">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-321">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="4f4a2-322">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-322">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="4f4a2-323">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-323">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="4f4a2-324">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-324">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="4f4a2-325">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-325">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="4f4a2-326">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-326">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="4f4a2-327">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-327">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="4f4a2-328">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-328">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="4f4a2-329">ACR</span><span class="sxs-lookup"><span data-stu-id="4f4a2-329">ACR</span></span>

* <span data-ttu-id="4f4a2-330">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-330">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="4f4a2-331">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-331">Support SKU update for managed registries</span></span>
* <span data-ttu-id="4f4a2-332">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-332">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="4f4a2-333">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-333">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="4f4a2-334">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-334">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="4f4a2-335">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-335">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-336">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-336">ACS</span></span>

* <span data-ttu-id="4f4a2-337">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-337">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-338">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="4f4a2-338">Appservice</span></span>

* <span data-ttu-id="4f4a2-339">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-339">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="4f4a2-340">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-340">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="4f4a2-341">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-341">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="4f4a2-342">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-342">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="4f4a2-343">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-343">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="4f4a2-344">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-344">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="4f4a2-345">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-345">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="4f4a2-346">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-346">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="4f4a2-347">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-347">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="4f4a2-348">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-348">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="4f4a2-349">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="4f4a2-349">Batch</span></span>

* <span data-ttu-id="4f4a2-350">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-350">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="4f4a2-351">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-351">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="4f4a2-352">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-352">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="4f4a2-353">CDN</span><span class="sxs-lookup"><span data-stu-id="4f4a2-353">CDN</span></span>

* <span data-ttu-id="4f4a2-354">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-354">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="4f4a2-355">Облако</span><span class="sxs-lookup"><span data-stu-id="4f4a2-355">Cloud</span></span>

* <span data-ttu-id="4f4a2-356">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-356">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="4f4a2-357">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-357">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="4f4a2-358">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-358">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="4f4a2-359">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-359">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="4f4a2-360">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-360">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4f4a2-361">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4f4a2-361">CosmosDB</span></span>

* <span data-ttu-id="4f4a2-362">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-362">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="4f4a2-363">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-363">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4f4a2-364">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="4f4a2-364">Data Lake Analytics</span></span>

* <span data-ttu-id="4f4a2-365">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-365">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="4f4a2-366">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-366">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="4f4a2-367">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-367">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4f4a2-368">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="4f4a2-368">Data Lake Store</span></span>

* <span data-ttu-id="4f4a2-369">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-369">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="4f4a2-370">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-370">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="4f4a2-371">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-371">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="4f4a2-372">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-372">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="4f4a2-373">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="4f4a2-373">Interactive</span></span>

* <span data-ttu-id="4f4a2-374">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-374">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="4f4a2-375">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-375">Increased test coverage</span></span>
* <span data-ttu-id="4f4a2-376">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-376">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="4f4a2-377">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-377">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="4f4a2-378">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-378">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="4f4a2-379">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-379">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="4f4a2-380">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-380">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="4f4a2-381">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-381">Added `--progress` flag</span></span>
* <span data-ttu-id="4f4a2-382">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-382">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="4f4a2-383">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-383">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="4f4a2-384">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="4f4a2-384">IoT</span></span>

* <span data-ttu-id="4f4a2-385">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="4f4a2-385">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="4f4a2-386">(3934).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-386">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="4f4a2-387">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4f4a2-387">Key vault</span></span>

* <span data-ttu-id="4f4a2-388">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="4f4a2-388">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="4f4a2-389">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="4f4a2-389">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="4f4a2-390">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="4f4a2-390">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4f4a2-391">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="4f4a2-391">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="4f4a2-392">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-392">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="4f4a2-393">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-393">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="4f4a2-394">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="4f4a2-394">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="4f4a2-395">(3307).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-395">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="4f4a2-396">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4f4a2-396">Lab</span></span>

* <span data-ttu-id="4f4a2-397">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-397">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="4f4a2-398">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-398">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="4f4a2-399">Монитор</span><span class="sxs-lookup"><span data-stu-id="4f4a2-399">Monitor</span></span>

* <span data-ttu-id="4f4a2-400">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-400">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="4f4a2-401">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-401">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="4f4a2-402">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-402">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="4f4a2-403">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-403">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="4f4a2-404">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-404">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="4f4a2-405">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="4f4a2-405">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="4f4a2-406">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="4f4a2-406">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="4f4a2-407">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="4f4a2-407">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="4f4a2-408">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="4f4a2-408">`location` no longer required</span></span>
  * <span data-ttu-id="4f4a2-409">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="4f4a2-409">Add name and ID support for target</span></span>
  * <span data-ttu-id="4f4a2-410">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="4f4a2-410">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="4f4a2-411">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="4f4a2-411">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="4f4a2-412">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="4f4a2-412">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="4f4a2-413">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-413">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="4f4a2-414">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-414">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="4f4a2-415">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-415">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="4f4a2-416">Сеть</span><span class="sxs-lookup"><span data-stu-id="4f4a2-416">Network</span></span>

* <span data-ttu-id="4f4a2-417">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-417">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="4f4a2-418">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-418">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="4f4a2-419">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-419">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="4f4a2-420">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-420">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="4f4a2-421">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-421">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="4f4a2-422">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-422">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="4f4a2-423">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-423">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="4f4a2-424">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-424">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="4f4a2-425">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-425">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="4f4a2-426">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-426">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="4f4a2-427">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-427">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="4f4a2-428">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-428">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="4f4a2-429">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-429">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="4f4a2-430">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-430">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="4f4a2-431">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-431">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="4f4a2-432">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-432">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="4f4a2-433">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-433">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="4f4a2-434">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-434">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="4f4a2-435">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-435">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="4f4a2-436">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-436">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="4f4a2-437">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-437">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="4f4a2-438">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-438">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="4f4a2-439">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-439">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="4f4a2-440">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-440">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="4f4a2-441">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-441">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="4f4a2-442">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-442">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="4f4a2-443">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-443">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="4f4a2-444">Профиль</span><span class="sxs-lookup"><span data-stu-id="4f4a2-444">Profile</span></span>

* <span data-ttu-id="4f4a2-445">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-445">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="4f4a2-446">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-446">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="4f4a2-447">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-447">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="4f4a2-448">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-448">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="4f4a2-449">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-449">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="4f4a2-450">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="4f4a2-450">RDBMS</span></span>

* <span data-ttu-id="4f4a2-451">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-451">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="4f4a2-452">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-452">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="4f4a2-453">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-453">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="4f4a2-454">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-454">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="4f4a2-455">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4f4a2-455">Resource</span></span>

* <span data-ttu-id="4f4a2-456">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-456">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="4f4a2-457">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-457">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="4f4a2-458">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-458">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="4f4a2-459">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-459">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="4f4a2-460">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-460">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="4f4a2-461">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-461">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="4f4a2-462">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-462">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="4f4a2-463">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-463">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="4f4a2-464">Роль</span><span class="sxs-lookup"><span data-stu-id="4f4a2-464">Role</span></span>

* <span data-ttu-id="4f4a2-465">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-465">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="4f4a2-466">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-466">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="4f4a2-467">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-467">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="4f4a2-468">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-468">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="4f4a2-469">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-469">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="4f4a2-470">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="4f4a2-470">Service Fabric</span></span>
* <span data-ttu-id="4f4a2-471">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-471">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="4f4a2-472">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-472">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="4f4a2-473">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-473">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="4f4a2-474">SQL</span><span class="sxs-lookup"><span data-stu-id="4f4a2-474">SQL</span></span>

* <span data-ttu-id="4f4a2-475">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-475">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="4f4a2-476">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-476">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="4f4a2-477">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-477">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-478">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4f4a2-478">Storage</span></span>

* <span data-ttu-id="4f4a2-479">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-479">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="4f4a2-480">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-480">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="4f4a2-481">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-481">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="4f4a2-482">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="4f4a2-482">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="4f4a2-483">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-483">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="4f4a2-484">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-484">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-485">ВМ</span><span class="sxs-lookup"><span data-stu-id="4f4a2-485">VM</span></span>

* <span data-ttu-id="4f4a2-486">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-486">Support configuring nsg</span></span>
* <span data-ttu-id="4f4a2-487">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-487">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="4f4a2-488">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-488">Support managed service identities</span></span>
* <span data-ttu-id="4f4a2-489">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-489">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="4f4a2-490">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-490">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="4f4a2-491">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-491">May 10, 2017</span></span>

<span data-ttu-id="4f4a2-492">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="4f4a2-492">Version 2.0.6</span></span>

* <span data-ttu-id="4f4a2-493">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-493">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="4f4a2-494">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-494">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="4f4a2-495">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-495">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="4f4a2-496">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-496">Include Cognitive Services module.</span></span>
* <span data-ttu-id="4f4a2-497">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-497">Include Service Fabric module.</span></span>
* <span data-ttu-id="4f4a2-498">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-498">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="4f4a2-499">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-499">Add support for CDN commands.</span></span>
* <span data-ttu-id="4f4a2-500">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-500">Remove Container module.</span></span>
* <span data-ttu-id="4f4a2-501">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-501">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="4f4a2-502">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-502">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="4f4a2-503">Core</span><span class="sxs-lookup"><span data-stu-id="4f4a2-503">Core</span></span>

* <span data-ttu-id="4f4a2-504">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-504">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="4f4a2-505">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-505">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="4f4a2-506">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-506">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="4f4a2-507">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-507">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="4f4a2-508">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-508">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="4f4a2-509">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-509">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="4f4a2-510">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-510">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="4f4a2-511">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-511">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="4f4a2-512">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-512">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="4f4a2-513">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-513">core: Improved performance</span></span>
* <span data-ttu-id="4f4a2-514">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-514">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="4f4a2-515">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-515">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="4f4a2-516">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-516">ACS</span></span>

* <span data-ttu-id="4f4a2-517">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-517">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="4f4a2-518">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-518">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="4f4a2-519">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-519">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="4f4a2-520">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-520">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="4f4a2-521">AppService</span><span class="sxs-lookup"><span data-stu-id="4f4a2-521">AppService</span></span>

* <span data-ttu-id="4f4a2-522">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-522">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="4f4a2-523">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-523">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="4f4a2-524">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-524">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="4f4a2-525">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-525">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="4f4a2-526">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-526">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="4f4a2-527">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-527">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="4f4a2-528">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-528">support slot swap with preview</span></span>
* <span data-ttu-id="4f4a2-529">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-529">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="4f4a2-530">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-530">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="4f4a2-531">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="4f4a2-531">CosmosDB</span></span>

* <span data-ttu-id="4f4a2-532">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-532">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="4f4a2-533">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-533">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="4f4a2-534">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-534">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="4f4a2-535">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-535">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="4f4a2-536">Аналитика озера данных</span><span class="sxs-lookup"><span data-stu-id="4f4a2-536">Data Lake Analytics</span></span>

* <span data-ttu-id="4f4a2-537">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-537">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="4f4a2-538">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-538">Add support for new catalog item type: package.</span></span> <span data-ttu-id="4f4a2-539">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-539">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="4f4a2-540">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="4f4a2-540">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="4f4a2-541">Таблица</span><span class="sxs-lookup"><span data-stu-id="4f4a2-541">Table</span></span>
  * <span data-ttu-id="4f4a2-542">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="4f4a2-542">Table valued function</span></span>
  * <span data-ttu-id="4f4a2-543">Просмотр</span><span class="sxs-lookup"><span data-stu-id="4f4a2-543">View</span></span>
  * <span data-ttu-id="4f4a2-544">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-544">Table Statistics.</span></span> <span data-ttu-id="4f4a2-545">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-545">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="4f4a2-546">Хранилище озера данных</span><span class="sxs-lookup"><span data-stu-id="4f4a2-546">Data Lake Store</span></span>

* <span data-ttu-id="4f4a2-547">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-547">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="4f4a2-548">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-548">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="4f4a2-549">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-549">missed help for access show.</span></span> <span data-ttu-id="4f4a2-550">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-550">adding it.</span></span> <span data-ttu-id="4f4a2-551">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-551">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="4f4a2-552">Поиск</span><span class="sxs-lookup"><span data-stu-id="4f4a2-552">Find</span></span>

* <span data-ttu-id="4f4a2-553">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-553">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="4f4a2-554">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="4f4a2-554">KeyVault</span></span>

* <span data-ttu-id="4f4a2-555">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-555">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="4f4a2-556">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-556">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="4f4a2-557">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-557">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="4f4a2-558">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-558">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="4f4a2-559">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-559">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="4f4a2-560">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="4f4a2-560">Lab</span></span>

* <span data-ttu-id="4f4a2-561">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-561">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="4f4a2-562">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-562">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="4f4a2-563">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-563">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="4f4a2-564">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-564">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="4f4a2-565">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-565">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="4f4a2-566">Монитор</span><span class="sxs-lookup"><span data-stu-id="4f4a2-566">Monitor</span></span>

* <span data-ttu-id="4f4a2-567">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-567">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="4f4a2-568">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-568">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="4f4a2-569">Сеть</span><span class="sxs-lookup"><span data-stu-id="4f4a2-569">Network</span></span>

* <span data-ttu-id="4f4a2-570">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-570">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="4f4a2-571">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-571">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="4f4a2-572">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-572">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="4f4a2-573">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-573">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="4f4a2-574">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-574">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="4f4a2-575">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-575">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="4f4a2-576">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-576">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="4f4a2-577">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-577">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="4f4a2-578">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-578">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="4f4a2-579">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="4f4a2-579">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="4f4a2-580">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-580">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="4f4a2-581">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-581">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="4f4a2-582">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-582">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="4f4a2-583">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-583">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="4f4a2-584">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-584">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="4f4a2-585">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-585">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="4f4a2-586">Профиль</span><span class="sxs-lookup"><span data-stu-id="4f4a2-586">Profile</span></span>

* <span data-ttu-id="4f4a2-587">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-587">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="4f4a2-588">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-588">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="4f4a2-589">Redis</span><span class="sxs-lookup"><span data-stu-id="4f4a2-589">Redis</span></span>

* <span data-ttu-id="4f4a2-590">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-590">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="4f4a2-591">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-591">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="4f4a2-592">Ресурс</span><span class="sxs-lookup"><span data-stu-id="4f4a2-592">Resource</span></span>

* <span data-ttu-id="4f4a2-593">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-593">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="4f4a2-594">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-594">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="4f4a2-595">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-595">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="4f4a2-596">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-596">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="4f4a2-597">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-597">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="4f4a2-598">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-598">Add docs for az lock update.</span></span> <span data-ttu-id="4f4a2-599">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-599">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="4f4a2-600">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-600">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="4f4a2-601">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-601">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="4f4a2-602">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-602">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="4f4a2-603">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="4f4a2-603">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="4f4a2-604">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-604">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="4f4a2-605">Роль</span><span class="sxs-lookup"><span data-stu-id="4f4a2-605">Role</span></span>

* <span data-ttu-id="4f4a2-606">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-606">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="4f4a2-607">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-607">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="4f4a2-608">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-608">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="4f4a2-609">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-609">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="4f4a2-610">SQL</span><span class="sxs-lookup"><span data-stu-id="4f4a2-610">SQL</span></span>

* <span data-ttu-id="4f4a2-611">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-611">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="4f4a2-612">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-612">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="4f4a2-613">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4f4a2-613">Storage</span></span>

* <span data-ttu-id="4f4a2-614">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-614">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="4f4a2-615">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-615">Add support for incremental blob copy</span></span>
* <span data-ttu-id="4f4a2-616">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-616">Add support for large block blob upload</span></span>
* <span data-ttu-id="4f4a2-617">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-617">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-618">ВМ</span><span class="sxs-lookup"><span data-stu-id="4f4a2-618">VM</span></span>

* <span data-ttu-id="4f4a2-619">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-619">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="4f4a2-620">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="4f4a2-620">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="4f4a2-621">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="4f4a2-621">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="4f4a2-622">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="4f4a2-622">az vm/vmss disk</span></span>
  3. <span data-ttu-id="4f4a2-623">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-623">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="4f4a2-624">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-624">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="4f4a2-625">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-625">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="4f4a2-626">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-626">April 3, 2017</span></span>

<span data-ttu-id="4f4a2-627">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="4f4a2-627">Version 2.0.2</span></span>

<span data-ttu-id="4f4a2-628">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-628">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="4f4a2-629">Core</span><span class="sxs-lookup"><span data-stu-id="4f4a2-629">Core</span></span>

* <span data-ttu-id="4f4a2-630">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-630">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="4f4a2-631">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-631">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="4f4a2-632">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-632">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="4f4a2-633">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-633">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4f4a2-634">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-634">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="4f4a2-635">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="4f4a2-635">Add prompting for missing template parameters.</span></span> <span data-ttu-id="4f4a2-636">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-636">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="4f4a2-637">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-637">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="4f4a2-638">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-638">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="4f4a2-639">ACS</span><span class="sxs-lookup"><span data-stu-id="4f4a2-639">ACS</span></span>

* <span data-ttu-id="4f4a2-640">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-640">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="4f4a2-641">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="4f4a2-641">Add support for ssh key password prompting.</span></span> <span data-ttu-id="4f4a2-642">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-642">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="4f4a2-643">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="4f4a2-643">Add support for windows clusters.</span></span> <span data-ttu-id="4f4a2-644">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-644">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="4f4a2-645">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="4f4a2-645">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="4f4a2-646">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-646">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="4f4a2-647">AppService</span><span class="sxs-lookup"><span data-stu-id="4f4a2-647">AppService</span></span>

* <span data-ttu-id="4f4a2-648">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-648">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="4f4a2-649">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-649">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="4f4a2-650">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-650">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="4f4a2-651">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-651">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="4f4a2-652">DataLake</span><span class="sxs-lookup"><span data-stu-id="4f4a2-652">DataLake</span></span>

* <span data-ttu-id="4f4a2-653">Первоначальный выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-653">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="4f4a2-654">Первоначальный выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-654">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="4f4a2-655">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="4f4a2-655">DocuemntDB</span></span>

* <span data-ttu-id="4f4a2-656">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-656">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="4f4a2-657">ВМ</span><span class="sxs-lookup"><span data-stu-id="4f4a2-657">VM</span></span>

* <span data-ttu-id="4f4a2-658">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-658">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="4f4a2-659">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-659">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="4f4a2-660">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-660">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="4f4a2-661">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-661">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="4f4a2-662">Масштабируемый набор виртуальных машин: добавлена поддержка * для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-662">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="4f4a2-663">Добавлена команда --secrets для виртуальных машин и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-663">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="4f4a2-664">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-664">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="4f4a2-665">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-665">February 27, 2017</span></span>

<span data-ttu-id="4f4a2-666">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="4f4a2-666">Version 2.0.0</span></span>

<span data-ttu-id="4f4a2-667">Этот первый общедоступный выпуск Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-667">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="4f4a2-668">Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="4f4a2-668">General availability applies to these command modules:</span></span>
- <span data-ttu-id="4f4a2-669">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="4f4a2-669">Container Service (acs)</span></span>
- <span data-ttu-id="4f4a2-670">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="4f4a2-670">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="4f4a2-671">Сеть</span><span class="sxs-lookup"><span data-stu-id="4f4a2-671">Networking</span></span>
- <span data-ttu-id="4f4a2-672">Хранилище</span><span class="sxs-lookup"><span data-stu-id="4f4a2-672">Storage</span></span>

<span data-ttu-id="4f4a2-673">Эти командные модули могут использоваться в рабочих средах и поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-673">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="4f4a2-674">Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-674">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="4f4a2-675">Вы можете задавать вопросы на сайте [StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-675">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="4f4a2-676">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-676">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="4f4a2-677">Чтобы проверить версию интерфейса командной строки, используйте `az --version`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-677">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="4f4a2-678">В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-678">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="4f4a2-679">Некоторые командные модули имеют постфикс b*n* или rc*n*.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-679">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="4f4a2-680">Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-680">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="4f4a2-681">У нас также есть предварительные ежедневные сборки интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-681">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="4f4a2-682">Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="4f4a2-682">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="4f4a2-683">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="4f4a2-683">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="4f4a2-684">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="4f4a2-684">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="4f4a2-685">обратившись к специалистам группы разработчиков продукта по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com);</span><span class="sxs-lookup"><span data-stu-id="4f4a2-685">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="4f4a2-686">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="4f4a2-686">Provide feedback from the command line with the `az feedback` command.</span></span>

