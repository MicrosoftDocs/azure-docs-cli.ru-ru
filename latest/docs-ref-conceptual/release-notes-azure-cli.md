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
ms.openlocfilehash: ad30efeb7efafcc5816160ee130665d37adb62c6
ms.sourcegitcommit: e866977985ba0286fa05f41729dd7e7d9ce86f8e
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/13/2017
---
# <a name="azure-cli-20-release-notes"></a><span data-ttu-id="3e3d9-104">Заметки о выпуске Azure CLI 2.0</span><span class="sxs-lookup"><span data-stu-id="3e3d9-104">Azure CLI 2.0 release notes</span></span>

## <a name="september-11-2017"></a><span data-ttu-id="3e3d9-105">11 сентября 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-105">September 11, 2017</span></span>

<span data-ttu-id="3e3d9-106">Версия 2.0.17</span><span class="sxs-lookup"><span data-stu-id="3e3d9-106">Version 2.0.17</span></span>

### <a name="core"></a><span data-ttu-id="3e3d9-107">Core</span><span class="sxs-lookup"><span data-stu-id="3e3d9-107">Core</span></span>

* <span data-ttu-id="3e3d9-108">Включен командный модуль для настройки собственного идентификатора корреляции в телеметрии.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-108">Enabled command module to set its own correlation ID in telemetry</span></span>
* <span data-ttu-id="3e3d9-109">Исправлена проблема с дампом JSON, когда для телеметрии настроен режим диагностики.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-109">Fixed JSON dump issue when telemetry is set to diagnostics mode</span></span>

### <a name="acs"></a><span data-ttu-id="3e3d9-110">ACS</span><span class="sxs-lookup"><span data-stu-id="3e3d9-110">Acs</span></span>

* <span data-ttu-id="3e3d9-111">Добавлена команда `acs list-locations`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-111">Added `acs list-locations` command</span></span>
* <span data-ttu-id="3e3d9-112">Для `ssh-key-file` предоставляется ожидаемое значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-112">Made `ssh-key-file` come with expected default value</span></span>

### <a name="appservice"></a><span data-ttu-id="3e3d9-113">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3e3d9-113">Appservice</span></span>

* <span data-ttu-id="3e3d9-114">Добавлена возможность создавать веб-приложения в группе ресурсов в рамках плана службы, отличной от активной.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-114">Added ability to create a webapp in a resource group other than the active service plan's</span></span>

### <a name="cdn"></a><span data-ttu-id="3e3d9-115">CDN</span><span class="sxs-lookup"><span data-stu-id="3e3d9-115">CDN</span></span>

* <span data-ttu-id="3e3d9-116">Исправлена ошибка "CustomDomain не пригоден к итерации" для `cdn custom-domain create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-116">Fixed 'CustomDomain is not interable' bug for `cdn custom-domain create`.</span></span>

### <a name="extension"></a><span data-ttu-id="3e3d9-117">Добавочный номер</span><span class="sxs-lookup"><span data-stu-id="3e3d9-117">Extension</span></span>

* <span data-ttu-id="3e3d9-118">Первый выпуск.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-118">Initial Release.</span></span>

### <a name="keyvault"></a><span data-ttu-id="3e3d9-119">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="3e3d9-119">Keyvault</span></span>

* <span data-ttu-id="3e3d9-120">Исправлена проблема с зависимостью разрешений от регистра для `keyvault set-policy`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-120">Fixed issue where permissions were case sensitive for `keyvault set-policy`.</span></span>

### <a name="network"></a><span data-ttu-id="3e3d9-121">Сеть</span><span class="sxs-lookup"><span data-stu-id="3e3d9-121">Network</span></span>

* <span data-ttu-id="3e3d9-122">Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-122">Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="3e3d9-123">Аргумент `--private-access-services` переименован в `--service-endpoints` для команды `vnet subnet create/update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-123">Renamed `--private-access-services` argument to `--service-endpoints` for `vnet subnet create/update`</span></span>
* <span data-ttu-id="3e3d9-124">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule create/update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-124">Added support for multiple IP ranges and port ranges to `nsg rule create/update`</span></span>
* <span data-ttu-id="3e3d9-125">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-125">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="3e3d9-126">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-126">Added support for SKU to `public-ip create`</span></span>

### <a name="resource"></a><span data-ttu-id="3e3d9-127">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3e3d9-127">Resource</span></span>

* <span data-ttu-id="3e3d9-128">Разрешена передача в определениях параметров политики ресурсов в командах `policy definition create` и `policy definition update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-128">Allow passing in resource policy parameter definitions in `policy definition create`, and `policy definition update`</span></span>
* <span data-ttu-id="3e3d9-129">Разрешена передача значений параметров для команды `policy assignment create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-129">Allow passing in parameter values for `policy assignment create`</span></span>
* <span data-ttu-id="3e3d9-130">Разрешена передача JSON или файла для всех параметров.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-130">Allow for passing JSON or file for all params</span></span>
* <span data-ttu-id="3e3d9-131">Версия API изменена на более позднюю.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-131">Incremented API version</span></span>

### <a name="sql"></a><span data-ttu-id="3e3d9-132">SQL</span><span class="sxs-lookup"><span data-stu-id="3e3d9-132">SQL</span></span>

* <span data-ttu-id="3e3d9-133">Добавлены команды `sql server vnet-rule`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-133">Added `sql server vnet-rule` commands</span></span>

### <a name="vm"></a><span data-ttu-id="3e3d9-134">ВМ</span><span class="sxs-lookup"><span data-stu-id="3e3d9-134">VM</span></span>

* <span data-ttu-id="3e3d9-135">Исправлено: не назначать доступ, если `--scope` не предоставляется.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-135">Fixed: Don't assign access unless `--scope` is provided</span></span>
* <span data-ttu-id="3e3d9-136">Исправлено: использование тех же расширений имен, что и для портала.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-136">Fixed: Use the same extension naming as portal does</span></span>
* <span data-ttu-id="3e3d9-137">Удалено `subscription` из выходных данных `[vm|vmss] create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-137">Removed `subscription` from the `[vm|vmss] create` output</span></span>
* <span data-ttu-id="3e3d9-138">Исправлено: номер SKU хранилища `[vm|vmss] create` неприменим для дисков данных с образом.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-138">Fixed: `[vm|vmss] create` storage SKU is not applied on data disks with an image</span></span>
* <span data-ttu-id="3e3d9-139">Исправлено: `vm format-secret --secrets` не принимает идентификаторы, разделенные строками.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-139">Fixed: `vm format-secret --secrets` would not accept newline separated IDs</span></span>

## <a name="august-31-2017"></a><span data-ttu-id="3e3d9-140">31 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-140">August 31, 2017</span></span>

<span data-ttu-id="3e3d9-141">Версия 2.0.16</span><span class="sxs-lookup"><span data-stu-id="3e3d9-141">Version 2.0.16</span></span>

### <a name="keyvault"></a><span data-ttu-id="3e3d9-142">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="3e3d9-142">Keyvault</span></span>

* <span data-ttu-id="3e3d9-143">Исправлена ошибка при попытке автоматически разрешить шифрование секрета с помощью `secret download`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-143">Fixed bug when trying to automatically resolve secret encoding with `secret download`</span></span>

### <a name="sf"></a><span data-ttu-id="3e3d9-144">Sf</span><span class="sxs-lookup"><span data-stu-id="3e3d9-144">Sf</span></span>

* <span data-ttu-id="3e3d9-145">Объявлены неподдерживаемыми все команды; вместо них используется Service Fabric CLI (sfctl).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-145">Deprecating all commands in favor of Service Fabric CLI (sfctl)</span></span>

### <a name="storage"></a><span data-ttu-id="3e3d9-146">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3e3d9-146">Storage</span></span>

* <span data-ttu-id="3e3d9-147">Исправлена проблема, когда учетные записи хранения нельзя было создавать в регионах, которые не поддерживают функцию NetworkACLs.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-147">Fixed issue where storage accounts could not be created in regions that don't support the NetworkACLs feature</span></span>
* <span data-ttu-id="3e3d9-148">Определение типа и кодировки содержимого во время передачи больших двоичных объектов и файла, если оба свойства не указаны.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-148">Determine content type and content encoding during blob and file upload if neither content type and content encoding are specified</span></span>

## <a name="august-28-2017"></a><span data-ttu-id="3e3d9-149">28 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-149">August 28, 2017</span></span>

<span data-ttu-id="3e3d9-150">Версия 2.0.15</span><span class="sxs-lookup"><span data-stu-id="3e3d9-150">Version 2.0.15</span></span>

### <a name="cli"></a><span data-ttu-id="3e3d9-151">Интерфейс командной строки</span><span class="sxs-lookup"><span data-stu-id="3e3d9-151">CLI</span></span>

* <span data-ttu-id="3e3d9-152">К параметру `--version` добавлено юридическое примечание.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-152">Added legal note to `--version`.</span></span>

### <a name="acs"></a><span data-ttu-id="3e3d9-153">ACS</span><span class="sxs-lookup"><span data-stu-id="3e3d9-153">ACS</span></span>

* <span data-ttu-id="3e3d9-154">Исправлены регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-154">Corrected preview regions.</span></span>
* <span data-ttu-id="3e3d9-155">Правильно отформатирован параметр по умолчанию `dns_name_prefix`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-155">Formatted default `dns_name_prefix` properly.</span></span>
* <span data-ttu-id="3e3d9-156">Оптимизированы выходные данные команды ACS.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-156">Optimized acs command output.</span></span>

### <a name="appservice"></a><span data-ttu-id="3e3d9-157">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3e3d9-157">Appservice</span></span>

* <span data-ttu-id="3e3d9-158">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Исправлены несоответствия в выходных данных `az webapp config appsettings [delete|set]`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-158">[BREAKING CHANGE] Fixed inconsistencies in the output of `az webapp config appsettings [delete|set]`</span></span>
* <span data-ttu-id="3e3d9-159">Добавлен новый псевдоним `-i` в команду `az webapp config container set --docker-custom-image-name`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-159">Added a new alias of `-i` for `az webapp config container set --docker-custom-image-name`</span></span>
* <span data-ttu-id="3e3d9-160">Предоставлена команда `az webapp log show`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-160">Exposed `az webapp log show`</span></span>
* <span data-ttu-id="3e3d9-161">Предоставлены новые аргументы команды `az webapp delete`, которые позволяют сохранить план службы приложений, метрики и данные регистрации DNS.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-161">Exposed new arguments from `az webapp delete` to retain app service plan, metrics or dns registration</span></span>
* <span data-ttu-id="3e3d9-162">Исправление. Параметры слота определяются правильно.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-162">Fixed: Detect slot settings correctly</span></span>

### <a name="iot"></a><span data-ttu-id="3e3d9-163">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="3e3d9-163">IoT</span></span>

* <span data-ttu-id="3e3d9-164">Исправление 3934. При создании политики существующие политики больше не удаляются.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-164">Fixed #3934: Policy creation no longer clears existing policies</span></span>

### <a name="network"></a><span data-ttu-id="3e3d9-165">Сеть</span><span class="sxs-lookup"><span data-stu-id="3e3d9-165">Network</span></span>

* <span data-ttu-id="3e3d9-166">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Команда `vnet list-private-access-services` переименована в `vnet list-endpoint-services`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-166">[BREAKING CHANGE] Renamed `vnet list-private-access-services` to `vnet list-endpoint-services`</span></span>
* <span data-ttu-id="3e3d9-167">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--private-access-services` переименован в `--service-endpoints` в командах `vnet subnet [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-167">[BREAKING CHANGE] Renamed option `--private-access-services` to `--service-endpoints` for `vnet subnet [create|update]`</span></span>
* <span data-ttu-id="3e3d9-168">Добавлена поддержка нескольких диапазонов IP-адресов и портов в командах `nsg rule [create|update]`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-168">Added support for multiple IP and port ranges to `nsg rule [create|update]`</span></span>
* <span data-ttu-id="3e3d9-169">Добавлена поддержка номера SKU в команде `lb create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-169">Added support for SKU to `lb create`</span></span>
* <span data-ttu-id="3e3d9-170">Добавлена поддержка номера SKU в команде `public-ip create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-170">Added support for SKU to `public-ip create`</span></span>

### <a name="profile"></a><span data-ttu-id="3e3d9-171">Профиль</span><span class="sxs-lookup"><span data-stu-id="3e3d9-171">Profile</span></span>

* <span data-ttu-id="3e3d9-172">Предоставлены параметры `--msi` и `--msi-port` для входа с использованием удостоверения виртуальной машины.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-172">Exposed `--msi` and `--msi-port` to login using a virtual machine's identity</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3e3d9-173">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3e3d9-173">Service Fabric</span></span>

* <span data-ttu-id="3e3d9-174">Предварительный выпуск.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-174">Preview release</span></span>
* <span data-ttu-id="3e3d9-175">Упрощены правила реестра для паролей и имен пользователя для команды.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-175">Simplified registry user/password rules for command</span></span>
* <span data-ttu-id="3e3d9-176">Исправлена строка для ввода пароля пользователем даже после передачи параметра.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-176">Fixed password prompt for user even after passing in the param</span></span>
* <span data-ttu-id="3e3d9-177">Добавлена поддержка пустого значения `registry_cred`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-177">Added support for empty `registry_cred`</span></span>

### <a name="storage"></a><span data-ttu-id="3e3d9-178">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3e3d9-178">Storage</span></span>

* <span data-ttu-id="3e3d9-179">Появилась возможность задавать уровень большого двоичного объекта.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-179">Enabled setting blob tier</span></span>
* <span data-ttu-id="3e3d9-180">Добавлены аргументы `--bypass` и `--default-action` в командах `storage account [create|update]` для поддержки туннелирования службы.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-180">Added `--bypass` and `--default-action` arguments to `storage account [create|update]` to support service tunneling</span></span>
* <span data-ttu-id="3e3d9-181">Добавлены команды для добавления правил виртуальной сети и правил на основе IP-адресов в `storage account network-rule`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-181">Added commands to add VNET rules and IP based rules to `storage account network-rule`</span></span>  
* <span data-ttu-id="3e3d9-182">Разрешено шифрование службы с управляемым пользователем ключом.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-182">Enabled service encryption by customer managed key</span></span>
* <span data-ttu-id="3e3d9-183">[КРИТИЧЕСКИ ВАЖНОЕ ИЗМЕНЕНИЕ.] Параметр `--encryption` переименован в `--encryption-services` в команде `az storage account create and az storage account update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-183">[BREAKING CHANGE] Renamed `--encryption` option to `--encryption-services` for `az storage account create and az storage account update` command</span></span>
* <span data-ttu-id="3e3d9-184">Исправление 4220. Несоответствие синтаксиса `az storage account update encryption`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-184">Fixed #4220: `az storage account update encryption` - syntax mismatch</span></span>

### <a name="vm"></a><span data-ttu-id="3e3d9-185">ВМ</span><span class="sxs-lookup"><span data-stu-id="3e3d9-185">VM</span></span>

* <span data-ttu-id="3e3d9-186">Исправлена проблема, из-за которой для команды `vmss get-instance-view` отображались лишние и неправильные сведения при использовании параметра `--instance-id *`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-186">Fixed issue where extra, erroneous information was displayed for `vmss get-instance-view` when using `--instance-id *`</span></span>
* <span data-ttu-id="3e3d9-187">Добавлена поддержка параметра `--lb-sku` в команде `vmss create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-187">Added support for `--lb-sku` to `vmss create`:</span></span> 
* <span data-ttu-id="3e3d9-188">Из черного списка имен администраторов для команд `[vm|vmss] create` удалены имена людей.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-188">Removed human names from the admin name blacklist for `[vm|vmss] create`</span></span> 
* <span data-ttu-id="3e3d9-189">Исправлена проблема, из-за которой команда `[vm|vmss] create` выдавала ошибку, если из образа не удавалось извлечь сведения о плане.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-189">Fixed issue where `[vm|vmss] create` would throw an error if unable to extract plan information from an image</span></span>
* <span data-ttu-id="3e3d9-190">Исправлена проблема, которая приводила к сбою при создании масштабируемого набора виртуальных машин с внутренней подсистемой балансировки нагрузки.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-190">Fixed a crash when creating a vmms scaleset with an internal LB</span></span>
* <span data-ttu-id="3e3d9-191">Исправлена проблема, из-за которой аргумент `--no-wait` не работал с командой `vm availability-set create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-191">Fixed issue where `--no-wait` argument did not work wth `vm availability-set create`</span></span>


## <a name="august-15-2017"></a><span data-ttu-id="3e3d9-192">15 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-192">August 15, 2017</span></span>

<span data-ttu-id="3e3d9-193">Версия 2.0.14</span><span class="sxs-lookup"><span data-stu-id="3e3d9-193">Version 2.0.14</span></span>

### <a name="acs"></a><span data-ttu-id="3e3d9-194">ACS</span><span class="sxs-lookup"><span data-stu-id="3e3d9-194">ACS</span></span>

* <span data-ttu-id="3e3d9-195">Исправлен номер порта sshMaster0 для Kubernetes.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-195">Corrected sshMaster0 port number for kubernetes</span></span>

### <a name="appservice"></a><span data-ttu-id="3e3d9-196">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3e3d9-196">Appservice</span></span>

* <span data-ttu-id="3e3d9-197">Исправлено исключение при создании веб-приложения Linux на основе Git.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-197">Fixed an exception when creatng a new git based Linux webapp</span></span>

### <a name="event-grid"></a><span data-ttu-id="3e3d9-198">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="3e3d9-198">Event Grid</span></span>

* <span data-ttu-id="3e3d9-199">Добавлены зависимости пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-199">Added SDK dependencies</span></span>

## <a name="august-11-2017"></a><span data-ttu-id="3e3d9-200">11 августа 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-200">August 11, 2017</span></span>

<span data-ttu-id="3e3d9-201">Версия 2.0.13</span><span class="sxs-lookup"><span data-stu-id="3e3d9-201">Version 2.0.13</span></span>

### <a name="acs"></a><span data-ttu-id="3e3d9-202">ACS</span><span class="sxs-lookup"><span data-stu-id="3e3d9-202">ACS</span></span>

* <span data-ttu-id="3e3d9-203">Добавлены дополнительные регионы, в которых доступна предварительная версия.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-203">Added more preview regions</span></span>

### <a name="batch"></a><span data-ttu-id="3e3d9-204">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="3e3d9-204">Batch</span></span>

* <span data-ttu-id="3e3d9-205">Пакет SDK для пакетной службы обновлен до версии 3.1.0, а пакет SDK для управления пакетной службой — до версии 4.1.0.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-205">Updated to Batch SDK 3.1.0 and Batch Management SDK 4.1.0</span></span>
* <span data-ttu-id="3e3d9-206">Добавлена новая команда для отображения количества задач в задании.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-206">Added a new command show the task counts of a job</span></span>
* <span data-ttu-id="3e3d9-207">Исправлена ошибка при обработке URL-адреса SAS файла ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-207">Fixed bug in resource file SAS URL processing</span></span>
* <span data-ttu-id="3e3d9-208">Для конечной точки учетной записи пакетной службы теперь поддерживается дополнительный префикс https://.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-208">Batch account endpoint now supports optional 'https://' prefix</span></span>
* <span data-ttu-id="3e3d9-209">Поддерживается добавление к заданию списков, содержащих более 100 задач.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-209">Support for adding lists of more than 100 tasks to a job</span></span>
* <span data-ttu-id="3e3d9-210">Добавлено ведение журнала отладки при загрузке командного модуля расширений.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-210">Added debug logging for loading Extensions command module</span></span>

### <a name="component"></a><span data-ttu-id="3e3d9-211">Компонент</span><span class="sxs-lookup"><span data-stu-id="3e3d9-211">Component</span></span>

* <span data-ttu-id="3e3d9-212">Добавлено предупреждение о прекращении поддержки в команды az component.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-212">Added deprecation warning to 'az component' commands</span></span>

### <a name="container"></a><span data-ttu-id="3e3d9-213">Контейнер</span><span class="sxs-lookup"><span data-stu-id="3e3d9-213">Container</span></span>

* <span data-ttu-id="3e3d9-214">`create`. Исправлена проблема, из-за которой запрещалось использовать знак равенства в переменной среды.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-214">`create`: Fixed issue where equals sign was not allowed inside an environment variable</span></span>


### <a name="data-lake-store"></a><span data-ttu-id="3e3d9-215">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3e3d9-215">Data Lake Store</span></span>

* <span data-ttu-id="3e3d9-216">Включен индикатор хода выполнения.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-216">Enabled progress control</span></span>

### <a name="event-grid"></a><span data-ttu-id="3e3d9-217">Служба "Сетка событий Azure"</span><span class="sxs-lookup"><span data-stu-id="3e3d9-217">Event Grid</span></span>

* <span data-ttu-id="3e3d9-218">Первый выпуск</span><span class="sxs-lookup"><span data-stu-id="3e3d9-218">Initial release</span></span>

### <a name="network"></a><span data-ttu-id="3e3d9-219">Сеть</span><span class="sxs-lookup"><span data-stu-id="3e3d9-219">Network</span></span>

* <span data-ttu-id="3e3d9-220">`lb`. Исправлена проблема, из-за которой некоторые имена дочерних ресурсов не разрешались правильно, если не были указаны.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-220">`lb`: Fixed issue where the certain child resource names did not resolve correctly when omitted</span></span>
* <span data-ttu-id="3e3d9-221">`application-gateway {subresource} delete`. Исправлена проблема, из-за которой не учитывался параметр `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-221">`application-gateway {subresource} delete`: Fixed issue where `--no-wait` was not honored</span></span>
* <span data-ttu-id="3e3d9-222">`application-gateway http-settings update`. Исправлена проблема, из-за которой не удавалось отключить параметр `--connection-draining-timeout`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-222">`application-gateway http-settings update`: Fixed issue where `--connection-draining-timeout` could not be turned off</span></span>
* <span data-ttu-id="3e3d9-223">Исправлена проблема с непредвиденным аргументом ключевого слова `sa_data_size_kilobyes` при использовании с командой `az network vpn-connection ipsec-policy add`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-223">Fixed error unexpected keyword argument `sa_data_size_kilobyes` with `az network vpn-connection ipsec-policy add`</span></span>

### <a name="profile"></a><span data-ttu-id="3e3d9-224">Профиль</span><span class="sxs-lookup"><span data-stu-id="3e3d9-224">Profile</span></span>

* <span data-ttu-id="3e3d9-225">`account list`. Добавлен параметр `--refresh` для синхронизации последних подписок с сервером.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-225">`account list`: Added `--refresh` to sync up the latest subscriptions from server</span></span>

### <a name="storage"></a><span data-ttu-id="3e3d9-226">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3e3d9-226">Storage</span></span>

* <span data-ttu-id="3e3d9-227">Включено обновление учетной записи хранения с помощью удостоверения, назначенного системой.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-227">Enable update storage account with system assigned identity</span></span>

### <a name="vm"></a><span data-ttu-id="3e3d9-228">ВМ</span><span class="sxs-lookup"><span data-stu-id="3e3d9-228">VM</span></span>

* <span data-ttu-id="3e3d9-229">`availability-set`. Предоставлено число доменов сбоя при преобразовании.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-229">`availability-set`: Exposed fault domain count on convert</span></span>
* <span data-ttu-id="3e3d9-230">Предоставлена команда `list-skus`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-230">Exposed `list-skus` command</span></span>
* <span data-ttu-id="3e3d9-231">Поддерживается назначение удостоверений без создания назначений ролей.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-231">Support to assign identity w/o creating role assignments</span></span>
* <span data-ttu-id="3e3d9-232">При подключении дисков данных применяется номер SKU хранилища.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-232">Apply storage sku on attaching data disks</span></span>
* <span data-ttu-id="3e3d9-233">Удалено используемое по умолчанию имя диска ОС и номер SKU хранилища при использовании управляемых дисков.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-233">Removed default os-disk name and storage SKU when using managed disks</span></span>


## <a name="july-28-2017"></a><span data-ttu-id="3e3d9-234">28 июля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-234">July 28, 2017</span></span>

<span data-ttu-id="3e3d9-235">Версия 2.0.12</span><span class="sxs-lookup"><span data-stu-id="3e3d9-235">Version 2.0.12</span></span>

* <span data-ttu-id="3e3d9-236">Добавлены команды для контейнеров.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-236">Added container commands</span></span>
* <span data-ttu-id="3e3d9-237">Добавлены модули выставления счетов и потребления ресурсов.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-237">Added billing and consumption modules</span></span>

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

### <a name="core"></a><span data-ttu-id="3e3d9-238">Core</span><span class="sxs-lookup"><span data-stu-id="3e3d9-238">Core</span></span>

* <span data-ttu-id="3e3d9-239">Вывод сведений о пакетах SDK для проверки подлинности субъектов-служб с помощью сертификатов.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-239">Output sdk auth info for service principals with certificates</span></span>
* <span data-ttu-id="3e3d9-240">Исправлены исключения в ходе выполнения развертывания.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-240">Fixed deployment progress exceptions</span></span>
* <span data-ttu-id="3e3d9-241">Для создания клиента подписки используется конечная точка ARM текущего облака.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-241">Use arm endpoint from the current cloud to create subscription client</span></span>
* <span data-ttu-id="3e3d9-242">Улучшена параллельная обработка файла clouds.config (3636).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-242">Improved concurrent handling of clouds.config file (#3636)</span></span>
* <span data-ttu-id="3e3d9-243">Обновление идентификатора клиентского запроса при каждом выполнении команды.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-243">Refresh client request id for each command execution</span></span>
* <span data-ttu-id="3e3d9-244">Создание клиентов подписки с правильным профилем SDK (3635).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-244">Create subscription clients with right SDK profile (#3635)</span></span>
* <span data-ttu-id="3e3d9-245">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-245">Progress Reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="3e3d9-246">Добавлена поддержка выбора полей вывода в таблице с помощью запроса jmespath (3581).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-246">Added support for picking table output fields through jmespath query  (#3581)</span></span>
* <span data-ttu-id="3e3d9-247">Улучшено отключение аргументов анализа и добавлено ведение журналов с помощью жестов (3434).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-247">Improved the muting of parse args and append history with gestures (#3434)</span></span>
* <span data-ttu-id="3e3d9-248">Создание клиентов подписки с правильным профилем SDK.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-248">Create subscription clients with right SDK profile</span></span>
* <span data-ttu-id="3e3d9-249">Перемещение всех существующих файлов записи в последнюю папку.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-249">Move all existing recording files to latest folder</span></span>
* <span data-ttu-id="3e3d9-250">Исправлена идемпотентность при создании виртуальной машины или масштабируемого набора виртуальных машин (3586).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-250">Fixed idempotency for VM/VMSS create (#3586)</span></span>
* <span data-ttu-id="3e3d9-251">В путях команд больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-251">Command paths are no longer case sensitive</span></span>
* <span data-ttu-id="3e3d9-252">В определенных параметрах логического типа больше не учитывается регистр.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-252">Certain boolean-type parameters are no longer case sensitive</span></span>
* <span data-ttu-id="3e3d9-253">Поддержка входа на локальный сервер AD FS, например Azure Stack.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-253">Support login to ADFS on prem server like Azure Stack</span></span>
* <span data-ttu-id="3e3d9-254">Исправлена параллельная запись в файл clouds.config (3255).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-254">Fixed concurrent writes to clouds.config (#3255)</span></span>

### <a name="acr"></a><span data-ttu-id="3e3d9-255">ACR</span><span class="sxs-lookup"><span data-stu-id="3e3d9-255">ACR</span></span>

* <span data-ttu-id="3e3d9-256">Добавлена команда `show-usage` для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-256">Added `show-usage` command for managed registries</span></span>
* <span data-ttu-id="3e3d9-257">Поддержка обновления номера SKU для управляемых реестров.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-257">Support SKU update for managed registries</span></span>
* <span data-ttu-id="3e3d9-258">Добавлены управляемые реестры с управляемыми номерами SKU.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-258">Added managed registries with managed SKU</span></span>
* <span data-ttu-id="3e3d9-259">Добавлены веб-перехватчики для управляемых реестров с использованием модуля для команды acr webhook.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-259">Added webhooks for managed registries with acr webhook command module</span></span>
* <span data-ttu-id="3e3d9-260">Добавлена проверка подлинности с помощью AAD с использованием команды acr login.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-260">Added AAD authentication with acr login command</span></span>
* <span data-ttu-id="3e3d9-261">Добавлена команда delete для репозиториев, манифестов и тегов Docker.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-261">Added delete command for docker repositories, manifests, and tags</span></span>

### <a name="acs"></a><span data-ttu-id="3e3d9-262">ACS</span><span class="sxs-lookup"><span data-stu-id="3e3d9-262">ACS</span></span>

* <span data-ttu-id="3e3d9-263">Поддержка API версии 2017-07-01.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-263">Support for API version 2017-07-01</span></span>

### <a name="appservice"></a><span data-ttu-id="3e3d9-264">Служба приложений</span><span class="sxs-lookup"><span data-stu-id="3e3d9-264">Appservice</span></span>

* <span data-ttu-id="3e3d9-265">Исправлена ошибка, из-за которой команда вывода списка в веб-приложениях Linux не возвращала данные.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-265">Fixed bug where listing Linux webapp would return nothing</span></span>
* <span data-ttu-id="3e3d9-266">Поддержка извлечения учетных данных из ACR.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-266">Support to retrieve creds from acr</span></span>
* <span data-ttu-id="3e3d9-267">Удаление всех команд группы `appservice web`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-267">Remove all commands under `appservice web`</span></span>
* <span data-ttu-id="3e3d9-268">Создание масок паролей для реестров Docker из выходных данных команды (3656).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-268">Mask docker registry passwords from command output (#3656)</span></span>
* <span data-ttu-id="3e3d9-269">Обеспечено использование браузера по умолчанию в macOS без ошибок (3623).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-269">Ensure default browser is used on macOS without errors (#3623)</span></span>
* <span data-ttu-id="3e3d9-270">Улучшена справка по командам `webapp log tail` и `webapp log download` (3624).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-270">Improve the help of `webapp log tail` and `webapp log download` (#3624)</span></span>
* <span data-ttu-id="3e3d9-271">Предоставлена команда `traffic-routing` для настройки статической маршрутизации (3566).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-271">Exposed `traffic-routing` command to configure static routing (#3566)</span></span>
* <span data-ttu-id="3e3d9-272">Добавлены исправления, связанные с надежностью, при настройке системы управления версиями (3245).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-272">Added reliability fixes in configuring source control (#3245)</span></span>
* <span data-ttu-id="3e3d9-273">Удален неподдерживаемый аргумент `--node-version` из функции `webapp config update` для веб-приложений Windows.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-273">Removed unsupported `--node-version` argument from `webapp config update` for Windows webapps.</span></span> <span data-ttu-id="3e3d9-274">Вместо него используется `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-274">Instead use `webapp config appsettings set --settings WEBSITE_NODE_DEFAULT_VERSION=...`</span></span>

### <a name="batch"></a><span data-ttu-id="3e3d9-275">Пакетная служба</span><span class="sxs-lookup"><span data-stu-id="3e3d9-275">Batch</span></span>

* <span data-ttu-id="3e3d9-276">Пакеты SDK для пакетной службы обновлены до версии 3.0.0 с поддержкой низкоприоритетных виртуальных машин в пулах.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-276">Updated to Batch SDK 3.0.0 with support for low-priority VMs in pools</span></span>
* <span data-ttu-id="3e3d9-277">Параметр команды `pool create` переименован с `--target-dedicated` в `--target-dedicated-nodes`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-277">Renamed `pool create` option `--target-dedicated` to `--target-dedicated-nodes`</span></span>
* <span data-ttu-id="3e3d9-278">Для команды `pool create` добавлены параметры `--target-low-priority-nodes` и `--application-licenses`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-278">Added `pool create` options `--target-low-priority-nodes` and `--application-licenses`</span></span>

### <a name="cdn"></a><span data-ttu-id="3e3d9-279">CDN</span><span class="sxs-lookup"><span data-stu-id="3e3d9-279">CDN</span></span>

* <span data-ttu-id="3e3d9-280">Предоставлено улучшенное сообщение об ошибке для команды `cdn endpoint list`, которое отображается, если заданный параметром `--profile-name` профиль не существует.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-280">Provided a better error message for `cdn endpoint list` when the profile specified by `--profile-name` does not exist.</span></span>

### <a name="cloud"></a><span data-ttu-id="3e3d9-281">Облако</span><span class="sxs-lookup"><span data-stu-id="3e3d9-281">Cloud</span></span>

* <span data-ttu-id="3e3d9-282">Формат версии API конечной точки метаданных облака изменен на следующий: ГГГГ-ММ-ДД.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-282">Changed API version of cloud metadata endpoint to YYYY-MM-DD format</span></span>
* <span data-ttu-id="3e3d9-283">Конечная точка коллекции не является обязательной.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-283">Gallery endpoint isn't required</span></span>
* <span data-ttu-id="3e3d9-284">Поддерживается регистрация облака только с конечной точкой диспетчера ARM.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-284">Support for registering cloud just with ARM resource manager endpoint</span></span>
* <span data-ttu-id="3e3d9-285">Предоставлен параметр в команде `cloud set` для выбора профиля при выборе текущего облака.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-285">Provided an option for `cloud set` to choose the profile while selecting current cloud</span></span>
* <span data-ttu-id="3e3d9-286">Предоставлен параметр `endpoint_vm_image_alias_doc`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-286">Exposed `endpoint_vm_image_alias_doc`</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3e3d9-287">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3e3d9-287">CosmosDB</span></span>

* <span data-ttu-id="3e3d9-288">Внесены исправления, которые позволяют создавать коллекцию с пользовательским ключом секции.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-288">Fixed allowing creation of collection with custom partition key</span></span>
* <span data-ttu-id="3e3d9-289">Добавлена поддержка срока жизни по умолчанию для коллекции.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-289">Added support for collection default TTL.</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3e3d9-290">Data Lake Analytics</span><span class="sxs-lookup"><span data-stu-id="3e3d9-290">Data Lake Analytics</span></span>

* <span data-ttu-id="3e3d9-291">Добавлены команды для управления политикой вычислений в разделе `dla account compute-policy`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-291">Added commands for compute policy management under the `dla account compute-policy` heading</span></span>
* <span data-ttu-id="3e3d9-292">Добавлена команда `dla job pipeline show`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-292">Added `dla job pipeline show`</span></span>
* <span data-ttu-id="3e3d9-293">Добавлена команда `dla job recurrence list`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-293">Added `dla job recurrence list`</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3e3d9-294">Data Lake Store</span><span class="sxs-lookup"><span data-stu-id="3e3d9-294">Data Lake Store</span></span>

* <span data-ttu-id="3e3d9-295">Добавлена поддержка смены ключей пользовательского хранилища ключей в `dls account update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-295">Added support for user managed key vault key rotation in `dls account update`</span></span>
* <span data-ttu-id="3e3d9-296">Обновлена версия пакета SDK для базовой файловой системы Data Lake Store из-за проблем с производительностью.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-296">Updated underlying Data Lake Store filesystem SDK version, addressing a performance issue</span></span>
* <span data-ttu-id="3e3d9-297">Добавлена команда `dls enable-key-vault`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-297">Added command `dls enable-key-vault`.</span></span> <span data-ttu-id="3e3d9-298">Эта команда пытается активировать пользовательское хранилище ключей, предназначенное для шифрования данных в учетной записи Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-298">This command attempts to enable a user provided Key Vault for use encrypting the data ina Data Lake Store account</span></span>

### <a name="interactive"></a><span data-ttu-id="3e3d9-299">Интерактивный режим</span><span class="sxs-lookup"><span data-stu-id="3e3d9-299">Interactive</span></span>

* <span data-ttu-id="3e3d9-300">Улучшено время запуска с помощью кэшированных команд.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-300">Improved the start up time by using cached commands</span></span>
* <span data-ttu-id="3e3d9-301">Увеличено тестовое покрытие.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-301">Increased test coverage</span></span>
* <span data-ttu-id="3e3d9-302">Расширены возможности жеста "?", которые позволяют также вставить его в следующую команду.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-302">Enhanced the '?' gesture to also inject into the next command</span></span>
* <span data-ttu-id="3e3d9-303">Исправлены ошибки с интерактивными функциями в предварительной версии профиля 2017-03-09 (3587).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-303">Fixed interactive errors with the profile 2017-03-09-profile-preview (#3587)</span></span>
* <span data-ttu-id="3e3d9-304">Разрешено использовать `--version` в качестве параметра в интерактивном режиме (3645).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-304">Allowed `--version` as a parameter for interactive mode (#3645)</span></span>
* <span data-ttu-id="3e3d9-305">В интерактивном режиме больше не возникают ошибки при выполнении проверки (3570).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-305">Stop interactive mode throwing errors from validation completions (#3570)</span></span>
* <span data-ttu-id="3e3d9-306">Создание отчетов о ходе выполнения развертывания шаблонов (3510).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-306">Progress reporting for template deployments (#3510)</span></span>
* <span data-ttu-id="3e3d9-307">Добавлен флаг `--progress`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-307">Added `--progress` flag</span></span>
* <span data-ttu-id="3e3d9-308">Из вариантов завершения удалены `--debug` и `--verbose`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-308">Removed `--debug` and `--verbose` from completions</span></span>
* <span data-ttu-id="3e3d9-309">Из вариантов завершения удален `interactive` (3324).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-309">Removed `interactive` from completions (#3324)</span></span>

### <a name="iot"></a><span data-ttu-id="3e3d9-310">Интернет вещей</span><span class="sxs-lookup"><span data-stu-id="3e3d9-310">IoT</span></span>

* <span data-ttu-id="3e3d9-311">Исправлено. При создании политики больше не удаляются существующие политики</span><span class="sxs-lookup"><span data-stu-id="3e3d9-311">Fixed policy creation no longer clears existing policies.</span></span> <span data-ttu-id="3e3d9-312">(3934).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-312">(#3934)</span></span>

### <a name="key-vault"></a><span data-ttu-id="3e3d9-313">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="3e3d9-313">Key vault</span></span>

* <span data-ttu-id="3e3d9-314">Добавлены команды для функций восстановления хранилища ключей:</span><span class="sxs-lookup"><span data-stu-id="3e3d9-314">Added commands for key vault recovery features:</span></span>
  * <span data-ttu-id="3e3d9-315">`keyvault`, подкоманды `purge`, `recover` и `keyvault list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="3e3d9-315">`keyvault` subcommands `purge`, `recover`, `keyvault list-deleted`</span></span>
  * <span data-ttu-id="3e3d9-316">`keyvault secret`, подкоманды `backup`, `restore`, `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="3e3d9-316">`keyvault secret` subcommands `backup`, `restore`, `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="3e3d9-317">`keyvault certificate`, подкоманды `purge`, `recover` и `list-deleted`;</span><span class="sxs-lookup"><span data-stu-id="3e3d9-317">`keyvault certificate` subcommands `purge`, `recover`, `list-deleted`</span></span>
  * <span data-ttu-id="3e3d9-318">`keyvault key`, подкоманды `purge`, `recover` и `list-deleted`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-318">`keyvault key` subcommands `purge`, `recover`, `list-deleted`</span></span>
* <span data-ttu-id="3e3d9-319">Добавлена интеграция хранилища ключей с субъектом-службой (3133).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-319">Added service principal key vault integration (#3133)</span></span>
* <span data-ttu-id="3e3d9-320">Обновлена плоскость данных хранилища ключей до версии 0.3.2</span><span class="sxs-lookup"><span data-stu-id="3e3d9-320">Updated key vault dataplane to 0.3.2.</span></span> <span data-ttu-id="3e3d9-321">(3307).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-321">(#3307)</span></span>

### <a name="lab"></a><span data-ttu-id="3e3d9-322">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="3e3d9-322">Lab</span></span>

* <span data-ttu-id="3e3d9-323">Добавлена поддержка запросов ко всем виртуальным машинам в лаборатории с помощью `az lab vm claim`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-323">Added support for claiming any vm in the lab through `az lab vm claim`</span></span>
* <span data-ttu-id="3e3d9-324">Добавлен модуль форматирования табличных выходных данных команд `az lab vm list` и `az lab vm show`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-324">Added table output formatter for `az lab vm list` and `az lab vm show`</span></span>

### <a name="monitor"></a><span data-ttu-id="3e3d9-325">Монитор</span><span class="sxs-lookup"><span data-stu-id="3e3d9-325">Monitor</span></span>

* <span data-ttu-id="3e3d9-326">Исправлены ошибки с файлом шаблона с помощью команды `monitor autoscale-settings get-parameters-template` (3349).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-326">Fix for template file with `monitor autoscale-settings get-parameters-template` command (#3349)</span></span>
* <span data-ttu-id="3e3d9-327">Команда `monitor alert-rule-incidents list` переименована в `monitor alert list-incidents`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-327">Renamed `monitor alert-rule-incidents list` to `monitor alert list-incidents`</span></span>
* <span data-ttu-id="3e3d9-328">Команда `monitor alert-rule-incidents show` переименована в `monitor alert show-incident`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-328">Renamed `monitor alert-rule-incidents show` to `monitor alert show-incident`</span></span>
* <span data-ttu-id="3e3d9-329">Команда `monitor metric-defintions list` переименована в `monitor metrics list-definitions`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-329">Renamed `monitor metric-defintions list` to `monitor metrics list-definitions`</span></span>
* <span data-ttu-id="3e3d9-330">Команда `monitor alert-rules` переименована в `monitor alert`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-330">Renamed `monitor alert-rules` to `monitor alert`</span></span>
* <span data-ttu-id="3e3d9-331">В команду `monitor alert create` внесены следующие изменения:</span><span class="sxs-lookup"><span data-stu-id="3e3d9-331">Changed `monitor alert create`:</span></span>
  * <span data-ttu-id="3e3d9-332">подкоманды `condition` и `action` больше не принимают данные JSON;</span><span class="sxs-lookup"><span data-stu-id="3e3d9-332">`condition` and `action` subcommands no longer accept JSON</span></span>
  * <span data-ttu-id="3e3d9-333">добавлены различные параметры, которые упрощают процесс создания правила;</span><span class="sxs-lookup"><span data-stu-id="3e3d9-333">Add numerous parameters to simplify the rule creation process</span></span>
  * <span data-ttu-id="3e3d9-334">параметр `location` больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="3e3d9-334">`location` no longer required</span></span>
  * <span data-ttu-id="3e3d9-335">добавлена поддержка имени и идентификатора для целевого объекта;</span><span class="sxs-lookup"><span data-stu-id="3e3d9-335">Add name and ID support for target</span></span>
  * <span data-ttu-id="3e3d9-336">удален параметр `--alert-rule-resource-name`;</span><span class="sxs-lookup"><span data-stu-id="3e3d9-336">Remove `--alert-rule-resource-name`</span></span>
  * <span data-ttu-id="3e3d9-337">параметр `is-enabled` переименован в `enabled`, он больше не требуется;</span><span class="sxs-lookup"><span data-stu-id="3e3d9-337">Rename `is-enabled` to `enabled`, no longer required</span></span>
  * <span data-ttu-id="3e3d9-338">значения по умолчанию для `description` теперь основаны на указанном условии;</span><span class="sxs-lookup"><span data-stu-id="3e3d9-338">`description` defaults now based on the supplied condition</span></span>
  *  <span data-ttu-id="3e3d9-339">добавлены примеры, в которых подробно представлен новый формат.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-339">Add examples to help clarifiy the new format</span></span>
* <span data-ttu-id="3e3d9-340">Поддержка имен или идентификаторов для команд `monitor metric`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-340">Support names or IDs for `monitor metric` commands</span></span>
* <span data-ttu-id="3e3d9-341">Добавлены вспомогательные аргументы и примеры использования команды `monitor alert rule update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-341">Added convenience arguments and examples to `monitor alert rule update`</span></span>

### <a name="network"></a><span data-ttu-id="3e3d9-342">Сеть</span><span class="sxs-lookup"><span data-stu-id="3e3d9-342">Network</span></span>

* <span data-ttu-id="3e3d9-343">Добавлена команда `list-private-access-services`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-343">Added `list-private-access-services` command</span></span>
* <span data-ttu-id="3e3d9-344">Добавлен аргумент `--private-access-services` в команды `vnet subnet create` и `vnet subnet update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-344">Added `--private-access-services` argument to `vnet subnet create` and `vnet subnet update`</span></span>
* <span data-ttu-id="3e3d9-345">Исправлена проблема, из-за которой команда `application-gateway redirect-config create` завершалась ошибкой.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-345">Fixed issue where `application-gateway redirect-config create` would fail</span></span>
* <span data-ttu-id="3e3d9-346">Исправлена проблема, из-за которой команда `application-gateway redirect-config update` не работала с параметром `--no-wait`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-346">Fixed issue where `application-gateway redirect-config update` with `--no-wait` would not work</span></span>
* <span data-ttu-id="3e3d9-347">Исправлена ошибка при использовании аргумента `--servers` с командами `application-gateway address-pool create` и `application-gateway address-pool update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-347">Fixed bug when using `--servers` argument with `application-gateway address-pool create` and `application-gateway address-pool update`</span></span>
* <span data-ttu-id="3e3d9-348">Добавлены команды `application-gateway redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-348">Added `application-gateway redirect-config` commands</span></span>
* <span data-ttu-id="3e3d9-349">В команду `application-gateway ssl-policy` добавлены подкоманды `list-options`, `predefined list` и `predefined show`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-349">Added commands to `application-gateway ssl-policy`: `list-options`, `predefined list`, `predefined show`</span></span>
* <span data-ttu-id="3e3d9-350">В команду `application-gateway ssl-policy set` добавлены аргументы `--name`, `--cipher-suites` и `--min-protocol-version`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-350">Added arguments to `application-gateway ssl-policy set`: `--name`, `--cipher-suites`, `--min-protocol-version`</span></span>
* <span data-ttu-id="3e3d9-351">В команды `application-gateway http-settings create` и `application-gateway http-settings update` добавлены аргументы `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe` и `--path`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-351">Added arguments to `application-gateway http-settings create` and `application-gateway http-settings update`: `--host-name-from-backend-pool`, `--affinity-cookie-name`, `--enable-probe`, `--path`</span></span>
* <span data-ttu-id="3e3d9-352">В команды `application-gateway url-path-map create` и `application-gateway url-path-map update` добавлены аргументы `--default-redirect-config` и `--redirect-config`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-352">Added arguments to `application-gateway url-path-map create` and `application-gateway url-path-map update`: `--default-redirect-config`, `--redirect-config`</span></span>
* <span data-ttu-id="3e3d9-353">Добавлен аргумент `--redirect-config` в команду `application-gateway url-path-map rule create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-353">Added argument `--redirect-config` to `application-gateway url-path-map rule create`</span></span>
* <span data-ttu-id="3e3d9-354">Добавлена поддержка параметра `--no-wait` в команде `application-gateway url-path-map rule delete`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-354">Added support for `--no-wait` to `application-gateway url-path-map rule delete`</span></span>
* <span data-ttu-id="3e3d9-355">В команды `application-gateway probe create` и `application-gateway probe update` добавлены аргументы `--host-name-from-http-settings`, `--min-servers`, `--match-body` и `--match-status-codes`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-355">Added arguments to `application-gateway probe create` and `application-gateway probe update`: `--host-name-from-http-settings`, `--min-servers`, `--match-body`, `--match-status-codes`</span></span>
* <span data-ttu-id="3e3d9-356">Добавлен аргумент `--redirect-config` в команды `application-gateway rule create` и `application-gateway rule update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-356">Added argument `--redirect-config` to `application-gateway rule create` and `application-gateway rule update`</span></span>
* <span data-ttu-id="3e3d9-357">Добавлена поддержка аргумента `--accelerated-networking` в командах `nic create` и `nic update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-357">Added support for `--accelerated-networking` to `nic create` and `nic update`</span></span>
* <span data-ttu-id="3e3d9-358">Удален аргумент `--internal-dns-name-suffix` из команды `nic create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-358">Removed `--internal-dns-name-suffix` argument from `nic create`</span></span>
* <span data-ttu-id="3e3d9-359">Добавлена поддержка параметра `--dns-servers` в командах `nic update` и `nic create`. Добавлена поддержка параметра --dns-servers.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-359">Added support for `--dns-servers` to `nic update` and `nic create`: Add support for --dns-servers</span></span>
* <span data-ttu-id="3e3d9-360">Исправлена ошибка, из-за которой команда `local-gateway create` игнорировала параметр `--local-address-prefixes`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-360">Fixed bug where `local-gateway create` ignored `--local-address-prefixes`</span></span>
* <span data-ttu-id="3e3d9-361">Добавлена поддержка параметра `--dns-servers` в команде `vnet update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-361">Added support for `--dns-servers` to `vnet update`</span></span>
* <span data-ttu-id="3e3d9-362">Исправлена ошибка при создании пиринга без фильтрации маршрутов с помощью команды `express-route peering create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-362">Fixed bug when creating a peering without route filtering with `express-route peering create`</span></span>
* <span data-ttu-id="3e3d9-363">Исправлена ошибка, из-за которой аргументы `--provider` и `--bandwidth` не работали с командой `express-route update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-363">Fixed bug where `--provider` and `--bandwidth` arguments did not work with `express-route update`</span></span>
* <span data-ttu-id="3e3d9-364">Исправлена ошибка с логикой установки значений по умолчанию в команде `network watcher show-topology`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-364">Fixed bug with `network watcher show-topology` defaulting logic</span></span>
* <span data-ttu-id="3e3d9-365">Улучшено форматирование выходных данных команды `network list-usages`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-365">Improved output formatting for `network list-usages`</span></span>
* <span data-ttu-id="3e3d9-366">В команде `application-gateway http-listener create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-366">Use default frontend IP for `application-gateway http-listener create` if only one exists</span></span>
* <span data-ttu-id="3e3d9-367">В команде `application-gateway rule create` используются пул адресов, параметры HTTP и прослушиватель HTTP по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-367">Use default address pool, HTTP settings, and HTTP listener for `application-gateway rule create` if only one exists</span></span>
* <span data-ttu-id="3e3d9-368">В команде `lb rule create` используются интерфейсный IP-адрес и серверный пул по умолчанию, если они существуют.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-368">Use default frontend IP and backend pool for `lb rule create` if only one exists</span></span>
* <span data-ttu-id="3e3d9-369">В команде `lb inbound-nat-rule create` используется интерфейсный IP-адрес по умолчанию, если он существует.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-369">Use default frontend IP for `lb inbound-nat-rule create` if only one exists</span></span>

### <a name="profile"></a><span data-ttu-id="3e3d9-370">Профиль</span><span class="sxs-lookup"><span data-stu-id="3e3d9-370">Profile</span></span>

* <span data-ttu-id="3e3d9-371">Поддержка входа на виртуальную машину с использованием управляемого удостоверения.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-371">Support login inside a VM with a managed identity</span></span>
* <span data-ttu-id="3e3d9-372">Поддержка вывода данных команды `account show` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-372">Support output for `account show` in SDK auth file format</span></span>
* <span data-ttu-id="3e3d9-373">При использовании параметра --expanded-view отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-373">Show deprecation warnings when using '--expanded-view'</span></span>
* <span data-ttu-id="3e3d9-374">Добавлена команда `get-access-token` для предоставления необработанного токена AAD.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-374">Added `get-access-token` command to provide raw AAD token</span></span>
* <span data-ttu-id="3e3d9-375">Поддержка входа с учетной записью пользователя без связанных подписок.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-375">Support login with a user account with no associated subscriptions</span></span>

### <a name="rdbms"></a><span data-ttu-id="3e3d9-376">Реляционная СУБД</span><span class="sxs-lookup"><span data-stu-id="3e3d9-376">RDBMS</span></span>

* <span data-ttu-id="3e3d9-377">Поддержка вывода списка серверов в подписке (3417).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-377">Support listing servers across a subscription (#3417)</span></span>
* <span data-ttu-id="3e3d9-378">Исправлена проблема, когда объект `%s` не обрабатывался из-за отсутствия `% server_type` (3393).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-378">Fixed `%s` not processed becasue of missing `% server_type` (#3393)</span></span>
* <span data-ttu-id="3e3d9-379">Исправлено сопоставление источника документа и добавлена задача непрерывной интеграции для проверки (3361).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-379">Fixed doc source map and added CI task to verify (#3361)</span></span>
* <span data-ttu-id="3e3d9-380">Исправлена справка по MySQL и PostgreSQL (3369).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-380">Fixed MySQL and PostgreSQL help (#3369)</span></span>

### <a name="resource"></a><span data-ttu-id="3e3d9-381">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3e3d9-381">Resource</span></span>

* <span data-ttu-id="3e3d9-382">Улучшены запросы на ввод отсутствующих параметров для команды `group deployment create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-382">Improved prompts for missing parameters for `group deployment create`</span></span>
* <span data-ttu-id="3e3d9-383">Улучшен анализ синтаксиса `--parameters KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-383">Improved parsing of `--parameters KEY=VALUE` syntax</span></span>
* <span data-ttu-id="3e3d9-384">Исправлены проблемы, из-за которых файлы параметров `group deployment create` не распознавались с использованием синтаксиса `@<file>`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-384">Fixed issues where `group deployment create` parameter files were no longer recognized using `@<file>` syntax</span></span>
* <span data-ttu-id="3e3d9-385">Поддержка аргумента `--ids` в командах `resource` и `managedapp`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-385">Support `--ids` argument for `resource` and `managedapp` commands</span></span>
* <span data-ttu-id="3e3d9-386">Исправлены некоторые сообщения об ошибках и анализе (3584).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-386">Fixed up some parsing and error messages (#3584)</span></span>
* <span data-ttu-id="3e3d9-387">Исправлены ошибки анализа параметра `--resource-type` в команде `lock`. Теперь принимаются `<resource-namespace>` и `<resource-type>`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-387">Fixed `--resource-type` parsing for the `lock` command to accept `<resource-namespace>` and `<resource-type>`</span></span>
* <span data-ttu-id="3e3d9-388">Добавлена проверка параметров для шаблонов для ссылок на шаблоны (3629).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-388">Added parameter checking for template link templates (#3629)</span></span>
* <span data-ttu-id="3e3d9-389">Добавлена поддержка указания параметров развертывания с использованием синтаксиса `KEY=VALUE`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-389">Added support for specifying deployment parameters using `KEY=VALUE` syntax</span></span>

### <a name="role"></a><span data-ttu-id="3e3d9-390">Роль</span><span class="sxs-lookup"><span data-stu-id="3e3d9-390">Role</span></span>

* <span data-ttu-id="3e3d9-391">Поддержка вывода данных команды `create-for-rbac` в формате файла проверки подлинности с помощью пакета SDK.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-391">Support output in SDK auth file format for `create-for-rbac`</span></span>
* <span data-ttu-id="3e3d9-392">Добавлена очистка назначений ролей и связанного приложения AAD при удалении субъекта-службы (3610).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-392">Cleaned up role assignments and related AAD application when deleting a service principal (#3610)</span></span>
* <span data-ttu-id="3e3d9-393">В описания аргументов `--start-date` и `--end-date` команды `app create` добавлен формат времени.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-393">Include time format in `app create` args `--start-date` and `--end-date` descriptions</span></span>
* <span data-ttu-id="3e3d9-394">При использовании параметра `--expanded-view` отображаются предупреждения о прекращении поддержки.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-394">Show deprecation warnings when using `--expanded-view`</span></span>
* <span data-ttu-id="3e3d9-395">Добавлена интеграция хранилища ключей для команд `create-for-rbac` и `reset-credentials`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-395">Added key vault integration to the `create-for-rbac` and `reset-credentials` commands</span></span>

### <a name="service-fabric"></a><span data-ttu-id="3e3d9-396">Service Fabric</span><span class="sxs-lookup"><span data-stu-id="3e3d9-396">Service Fabric</span></span>
* <span data-ttu-id="3e3d9-397">Исправлена ошибка, из-за которой большие файлы в приложениях усекались при отправке (3666).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-397">Fixed an issue with large files in applications being truncated on upload (#3666)</span></span>
* <span data-ttu-id="3e3d9-398">Добавлены тесты для команд Service Fabric (3424).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-398">Added tests for Service Fabric commands (#3424)</span></span>
* <span data-ttu-id="3e3d9-399">Исправлены многие команды Service Fabric (3234).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-399">Fixed numerous Service Fabric commands (#3234)</span></span>

### <a name="sql"></a><span data-ttu-id="3e3d9-400">SQL</span><span class="sxs-lookup"><span data-stu-id="3e3d9-400">SQL</span></span>

* <span data-ttu-id="3e3d9-401">Удален недействительный параметр `--identity` команды `sql server create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-401">Removed broken `sql server create` `--identity` parameter</span></span>
* <span data-ttu-id="3e3d9-402">Удалены значения паролей из выходных данных команд `sql server create` и `sql server update`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-402">Removed password values from `sql server create` and `sql server update` command output</span></span>
* <span data-ttu-id="3e3d9-403">Добавлены команды `sql db list-editions` и `sql elastic-pool list-editions`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-403">Added commands `sql db list-editions` and `sql elastic-pool list-editions`</span></span>

### <a name="storage"></a><span data-ttu-id="3e3d9-404">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3e3d9-404">Storage</span></span>

* <span data-ttu-id="3e3d9-405">Удален параметр `--marker` из команд `storage blob list`, `storage container list` и `storage share list` (3745).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-405">Removed `--marker` option from `storage blob list`, `storage container list`, and `storage share list` commands (#3745)</span></span>
* <span data-ttu-id="3e3d9-406">Включено создание учетных записей хранения с поддержкой только HTTPS.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-406">Enabled creating an https-only storage account</span></span>
* <span data-ttu-id="3e3d9-407">Обновлены метрики хранилища, команды входа и CORS (3495).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-407">Updated storage metrics, logging and cors commands (#3495)</span></span>
* <span data-ttu-id="3e3d9-408">Перефразировано сообщение об исключении, которое выводит команда добавления CORS (3638) (3362)</span><span class="sxs-lookup"><span data-stu-id="3e3d9-408">Rephrased exception message from CORS add (#3638) (#3362)</span></span>  
* <span data-ttu-id="3e3d9-409">Генератор преобразован в список в режиме пробного выполнения команды пакетной загрузки (3592).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-409">Converted generator to a list in download batch command dry run mode (#3592)</span></span> 
* <span data-ttu-id="3e3d9-410">Исправлена проблема при пробном выполнении команды пакетной загрузки больших двоичных объектов (3640) (3592).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-410">Fixed blob download batch dryrun issue (#3640) (#3592)</span></span>

### <a name="vm"></a><span data-ttu-id="3e3d9-411">ВМ</span><span class="sxs-lookup"><span data-stu-id="3e3d9-411">VM</span></span>

* <span data-ttu-id="3e3d9-412">Поддержка настройки NSG.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-412">Support configuring nsg</span></span>
* <span data-ttu-id="3e3d9-413">Исправлена ошибка, из-за которой не удавалось правильно настроить DNS-сервер.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-413">Fixed a bug where the DNS server would not be configured correctly</span></span>
* <span data-ttu-id="3e3d9-414">Поддержка удостоверений управляемой службы.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-414">Support managed service identities</span></span>
* <span data-ttu-id="3e3d9-415">Исправлена проблема, из-за которой для команды `cmss create` с существующей подсистемой балансировки нагрузки требовался параметр `--backend-pool-name`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-415">Fixed issue where `cmss create` with an existing load balancer required `--backend-pool-name`.</span></span>
* <span data-ttu-id="3e3d9-416">Теперь нумерация LUN дисков данных, создаваемых с помощью команды `vm image create`, начинается с 0.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-416">Make datadisks created with `vm image create` lun start with 0</span></span>


## <a name="may-10-2017"></a><span data-ttu-id="3e3d9-417">10 мая 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-417">May 10, 2017</span></span>

<span data-ttu-id="3e3d9-418">Версия 2.0.6</span><span class="sxs-lookup"><span data-stu-id="3e3d9-418">Version 2.0.6</span></span>

* <span data-ttu-id="3e3d9-419">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-419">documentdb renamed to cosmosdb</span></span>
* <span data-ttu-id="3e3d9-420">Добавлена реляционная СУБД (MySQL, Postgres).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-420">Add rdbms (mysql, postgres)</span></span>
* <span data-ttu-id="3e3d9-421">Добавлены модули Data Lake Store и Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-421">Include Data Lake Analytics and Data Lake Store modules.</span></span>
* <span data-ttu-id="3e3d9-422">Добавлен модуль Cognitive Services.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-422">Include Cognitive Services module.</span></span>
* <span data-ttu-id="3e3d9-423">Добавлен модуль Service Fabric.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-423">Include Service Fabric module.</span></span>
* <span data-ttu-id="3e3d9-424">Добавлен модуль Interactive (az-shell переименован).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-424">Include Interactive module (rename of az-shell).</span></span>
* <span data-ttu-id="3e3d9-425">Добавлена поддержка команд CDN.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-425">Add support for CDN commands.</span></span>
* <span data-ttu-id="3e3d9-426">Удален модуль Container.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-426">Remove Container module.</span></span>
* <span data-ttu-id="3e3d9-427">Добавлена команда az -v для az --version ([№ 2926](https://github.com/Azure/azure-cli/issues/2926)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-427">Add 'az -v' as shortcut for 'az --version' ([#2926](https://github.com/Azure/azure-cli/issues/2926))</span></span>
* <span data-ttu-id="3e3d9-428">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-428">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>

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

### <a name="core"></a><span data-ttu-id="3e3d9-429">Core</span><span class="sxs-lookup"><span data-stu-id="3e3d9-429">Core</span></span>

* <span data-ttu-id="3e3d9-430">Ядро: запись исключений, порожденных незарегистрированным поставщиком, и его автоматическая регистрация.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-430">core: capture exceptions caused by unregistered provider and auto-register it</span></span>   
* <span data-ttu-id="3e3d9-431">Производительность: сохранение кэша маркеров библиотеки ADAL в памяти до завершения работы процесса ([№ 2603](https://github.com/Azure/azure-cli/issues/2603)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-431">perf: persist adal token cache in memory till process exits ([#2603](https://github.com/Azure/azure-cli/issues/2603))</span></span>
* <span data-ttu-id="3e3d9-432">Исправление байтов, возвращаемых из шестнадцатеричных отпечатков -o tsv ([№ 3053](https://github.com/Azure/azure-cli/issues/3053)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-432">Fix bytes returned from hex fingerprint -o tsv ([#3053](https://github.com/Azure/azure-cli/issues/3053))</span></span>
* <span data-ttu-id="3e3d9-433">Улучшенное скачивание сертификатов Key Vault и интеграция субъектов-служб AAD ([№ 3003](https://github.com/Azure/azure-cli/issues/3003)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-433">Enhanced Key Vault Certificate Download and AAD SP Integration ([#3003](https://github.com/Azure/azure-cli/issues/3003))</span></span>
* <span data-ttu-id="3e3d9-434">Добавление расположения Python в az -version ([№ 2986](https://github.com/Azure/azure-cli/issues/2986)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-434">Add Python location to ‘az —version’ ([#2986](https://github.com/Azure/azure-cli/issues/2986))</span></span>
* <span data-ttu-id="3e3d9-435">Вход: поддержка входа при отсутствии подписок ([№ 2929](https://github.com/Azure/azure-cli/issues/2929)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-435">login: support login when there are no subscriptions ([#2929](https://github.com/Azure/azure-cli/issues/2929))</span></span>
* <span data-ttu-id="3e3d9-436">Ядро: устранен сбой при двукратном входе с помощью субъекта-службы ([№ 2800](https://github.com/Azure/azure-cli/issues/2800)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-436">core: fix a failure when login using a service principal twice ([#2800](https://github.com/Azure/azure-cli/issues/2800))</span></span>
* <span data-ttu-id="3e3d9-437">Ядро: возможность настроить путь к файлу accessTokens.json с помощью env var ([№ 2605](https://github.com/Azure/azure-cli/issues/2605)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-437">core: Allow file path of accessTokens.json to be configurable through an env var ([#2605](https://github.com/Azure/azure-cli/issues/2605))</span></span>
* <span data-ttu-id="3e3d9-438">Ядро: возможность применять настроенные параметры по умолчанию к необязательным аргументам ([№ 2703](https://github.com/Azure/azure-cli/issues/2703)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-438">core: Allow configured defaults to apply on optional args ([#2703](https://github.com/Azure/azure-cli/issues/2703))</span></span>
* <span data-ttu-id="3e3d9-439">Ядро: повышение производительности.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-439">core: Improved performance</span></span>
* <span data-ttu-id="3e3d9-440">Ядро: настаиваемые сертификаты ЦС — поддержка настройки переменной среды REQUESTS_CA_BUNDLE.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-440">core: Custom CA Certs - Support setting REQUESTS_CA_BUNDLE environment variable</span></span>
* <span data-ttu-id="3e3d9-441">Ядро: облачная конфигурация — использование конечной точки Resource Manager, если не задана конечная точка управления.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-441">core: Cloud configuration - use 'resource manager' endpoint if 'management' endpoint not set</span></span>

### <a name="acs"></a><span data-ttu-id="3e3d9-442">ACS</span><span class="sxs-lookup"><span data-stu-id="3e3d9-442">ACS</span></span>

* <span data-ttu-id="3e3d9-443">Исправление: теперь значение счетчика баз данных master и агентов — целое число, а не строка.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-443">fix the master and agent count to be integer instead of string</span></span>
* <span data-ttu-id="3e3d9-444">Предоставлены команды az acs create --no-wait и az acs wait для асинхронного создания.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-444">expose 'az acs create --no-wait' and 'az acs wait' for async creation</span></span>
* <span data-ttu-id="3e3d9-445">Предоставлена команда az acs create --validate для пробного создания.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-445">expose 'az acs create --validate' for dry-run validations</span></span>
* <span data-ttu-id="3e3d9-446">Удален профиль Windows перед вызовом метода PUT для команды scale ([№ 2755](https://github.com/Azure/azure-cli/issues/2755)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-446">remove windows profile before PUT call for scale command ([#2755](https://github.com/Azure/azure-cli/issues/2755))</span></span>

### <a name="appservice"></a><span data-ttu-id="3e3d9-447">AppService</span><span class="sxs-lookup"><span data-stu-id="3e3d9-447">AppService</span></span>

* <span data-ttu-id="3e3d9-448">Приложение-функция: добавлена полная поддержка приложений-функций, включая создание, отображение, вывод списка, удаление, настройку имени узла, настройку протокола SSL и т. д.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-448">functionapp: add full functionapp supports, including create, show, list, delete, hostname, ssl, etc</span></span>
* <span data-ttu-id="3e3d9-449">Добавлены службы Team Services (VSTS) в качестве параметра непрерывной доставки в конфигурации веб-системы управления версиями службы приложений.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-449">Adding Team Services (vsts) as a continuous delivery option to "appservice web source-control config"</span></span>
* <span data-ttu-id="3e3d9-450">Создана команда az webapp, заменяющая команду az appservice web (для обеспечения обратной совместимости команда az appservice web будет оставлена еще в двух выпусках).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-450">Create "az webapp" to replace "az appservice web" (for backward compat, "az appservice web" will stay for 2 releases)</span></span>
* <span data-ttu-id="3e3d9-451">Предоставлены аргументы для настройки развертывания и стеков времени выполнения при создании веб-приложения.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-451">Expose arguments to configure deployment and "runtime stacks" on webapp create</span></span>
* <span data-ttu-id="3e3d9-452">Предоставлена команда webapp list-runtimes.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-452">Expose "webapp list-runtimes"</span></span>
* <span data-ttu-id="3e3d9-453">Поддержка настройки строк подключения ([№ 2647](https://github.com/Azure/azure-cli/issues/2647)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-453">support configure connection strings ([#2647](https://github.com/Azure/azure-cli/issues/2647))</span></span>
* <span data-ttu-id="3e3d9-454">Поддержка переключения слотов с предварительным просмотром.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-454">support slot swap with preview</span></span>
* <span data-ttu-id="3e3d9-455">Устранены ошибки из команд службы приложений ([№ 2948](https://github.com/Azure/azure-cli/issues/2948)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-455">Polish errors from appservice commands ([#2948](https://github.com/Azure/azure-cli/issues/2948))</span></span>
* <span data-ttu-id="3e3d9-456">Использование группы ресурсов в плане служб приложений для операций с сертификатами ([№ 2750](https://github.com/Azure/azure-cli/issues/2750)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-456">Use the app service plan's resource group for cert operations ([#2750](https://github.com/Azure/azure-cli/issues/2750))</span></span>

### <a name="cosmosdb"></a><span data-ttu-id="3e3d9-457">Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="3e3d9-457">CosmosDB</span></span>

* <span data-ttu-id="3e3d9-458">Модуль documentdb переименован в cosmosdb.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-458">Rename documentdb module to cosmosdb.</span></span>
* <span data-ttu-id="3e3d9-459">Добавлена поддержка интерфейсов API уровня данных DocumentDB: управление базами данных и коллекциями.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-459">Added support for documentdb data-plane APIs: database and collection management</span></span>
* <span data-ttu-id="3e3d9-460">Добавлена поддержка включения автоматической отработки отказа для учетных записей базы данных.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-460">Added support for enabling automatic failover on database accounts</span></span>
* <span data-ttu-id="3e3d9-461">Добавлена поддержка нового параметра ConsistentPrefix политики согласованности.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-461">Added support for new consistency policy ConsistentPrefix</span></span>

### <a name="data-lake-analytics"></a><span data-ttu-id="3e3d9-462">Аналитика озера данных</span><span class="sxs-lookup"><span data-stu-id="3e3d9-462">Data Lake Analytics</span></span>

* <span data-ttu-id="3e3d9-463">Исправлена ошибка, из-за которой фильтрация списков заданий по результату и состоянию вызывала сбой.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-463">Fix a bug where filtering on result and state for job lists would throw an error.</span></span>
* <span data-ttu-id="3e3d9-464">Добавлена поддержка нового типа элемента каталога — пакета.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-464">Add support for new catalog item type: package.</span></span> <span data-ttu-id="3e3d9-465">Для доступа к нему используется `az dla catalog package`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-465">accessed through: `az dla catalog package`</span></span>
* <span data-ttu-id="3e3d9-466">Появилась возможность вывести список следующих элементов каталога из базы данных (указание схемы не требуется):</span><span class="sxs-lookup"><span data-stu-id="3e3d9-466">Made it possible to list the following catalog items from within a database (no schema specification required):</span></span>

  * <span data-ttu-id="3e3d9-467">Таблица</span><span class="sxs-lookup"><span data-stu-id="3e3d9-467">Table</span></span>
  * <span data-ttu-id="3e3d9-468">функция с табличным значением;</span><span class="sxs-lookup"><span data-stu-id="3e3d9-468">Table valued function</span></span>
  * <span data-ttu-id="3e3d9-469">Просмотр</span><span class="sxs-lookup"><span data-stu-id="3e3d9-469">View</span></span>
  * <span data-ttu-id="3e3d9-470">статистика таблицы.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-470">Table Statistics.</span></span> <span data-ttu-id="3e3d9-471">Их можно также вывести с помощью схемы, но без указания имени таблицы.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-471">This can also be listed with a schema, but without specifying a table name.</span></span>

### <a name="data-lake-store"></a><span data-ttu-id="3e3d9-472">Хранилище озера данных</span><span class="sxs-lookup"><span data-stu-id="3e3d9-472">Data Lake Store</span></span>

* <span data-ttu-id="3e3d9-473">Обновлена версия пакета SDK базовой файловой системы, что обеспечивает лучшую поддержку сценариев регулирования на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-473">Update the version of the underlying filesystem SDK, which gives better support for handling server side throttling scenarios.</span></span>
* <span data-ttu-id="3e3d9-474">Повышена производительность загрузки пакетов и выполнения команд ([№ 2819](https://github.com/Azure/azure-cli/issues/2819)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-474">Improve performance of package load and command execution ([#2819](https://github.com/Azure/azure-cli/issues/2819))</span></span>
* <span data-ttu-id="3e3d9-475">Отсутствовала справка для команды access show.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-475">missed help for access show.</span></span> <span data-ttu-id="3e3d9-476">Теперь она добавлена.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-476">adding it.</span></span> <span data-ttu-id="3e3d9-477">([№ 2743](https://github.com/Azure/azure-cli/issues/2743))</span><span class="sxs-lookup"><span data-stu-id="3e3d9-477">([#2743](https://github.com/Azure/azure-cli/issues/2743))</span></span>

### <a name="find"></a><span data-ttu-id="3e3d9-478">Поиск</span><span class="sxs-lookup"><span data-stu-id="3e3d9-478">Find</span></span>

* <span data-ttu-id="3e3d9-479">Улучшены результаты поиска и разрешено управление версиями индекса поиска.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-479">improve search results and allow for versioning of the search index</span></span>

### <a name="keyvault"></a><span data-ttu-id="3e3d9-480">Хранилище ключей</span><span class="sxs-lookup"><span data-stu-id="3e3d9-480">KeyVault</span></span>

* <span data-ttu-id="3e3d9-481">BC: в команде `az keyvault certificate download` параметр -e со строкового или двоичного значения изменен на PEM или DER, чтобы лучше представить параметры.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-481">BC:`az keyvault certificate download` change -e from string or binary to PEM or DER to better represent the options</span></span>
* <span data-ttu-id="3e3d9-482">BC: из команды `keyvault certificate create` удалены параметры --expires и --not-before, так как они не поддерживаются службой.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-482">BC: Remove --expires and --not-before from `keyvault certificate create` as these parameters are not supported by the service.</span></span>
* <span data-ttu-id="3e3d9-483">В команду `keyvault certificate create` добавлен параметр --validity для выборочного переопределения значение в параметре --policy.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-483">Adds the --validity parameter to `keyvault certificate create` to selectively override the value in --policy</span></span>
* <span data-ttu-id="3e3d9-484">Исправлена ошибка в команде `keyvault certificate get-default-policy`, в которой были доступны параметры expires и not_before, а параметр validity_in_months — нет.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-484">Fixes issue in `keyvault certificate get-default-policy` where 'expires' and 'not_before' were exposed but 'validity_in_months' was not.</span></span>
* <span data-ttu-id="3e3d9-485">Добавлено исправление для модуля keyvault для импорта PEM- и PFX-файлов ([№ 2754](https://github.com/Azure/azure-cli/issues/2754)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-485">keyvault fix for import of pem and pfx ([#2754](https://github.com/Azure/azure-cli/issues/2754))</span></span>

### <a name="lab"></a><span data-ttu-id="3e3d9-486">Лаборатория</span><span class="sxs-lookup"><span data-stu-id="3e3d9-486">Lab</span></span>

* <span data-ttu-id="3e3d9-487">Добавлены команды создания, отображения, удаления и вывода списка для среды в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-487">Adding create, show, delete & list commands for environment in the lab.</span></span>
* <span data-ttu-id="3e3d9-488">Добавлены команды отображения и вывода списка для просмотра шаблонов ARM в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-488">Adding show & list commands to view ARM templates in the lab.</span></span>
* <span data-ttu-id="3e3d9-489">В команду `az lab vm list` добавлен флаг --environment для фильтрации виртуальных машин по среде в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-489">Adding --environment flag in `az lab vm list` to filter VMs by environment in the lab.</span></span>
* <span data-ttu-id="3e3d9-490">Добавлена вспомогательная команда `az lab formula export-artifacts` для экспорта шаблона артефакта в формуле лаборатории.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-490">Add convenience command `az lab formula export-artifacts` to export artifact scaffold within a Lab's formula.</span></span>
* <span data-ttu-id="3e3d9-491">Добавлены команды для управления секретами в лаборатории.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-491">Add commands to manage secrets within a Lab.</span></span>

### <a name="monitor"></a><span data-ttu-id="3e3d9-492">Монитор</span><span class="sxs-lookup"><span data-stu-id="3e3d9-492">Monitor</span></span>

* <span data-ttu-id="3e3d9-493">Исправление ошибки: моделирование `--actions` в `az alert-rules create` для использования строки в формате JSON ([№ 3009](https://github.com/Azure/azure-cli/issues/3009)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-493">Bug Fix: Modeling `--actions` of `az alert-rules create` to consume JSON string ([#3009](https://github.com/Azure/azure-cli/issues/3009))</span></span>
* <span data-ttu-id="3e3d9-494">Исправление ошибки: при создании параметров диагностики не принимались журналы и метрики из команды show ([№ 2913](https://github.com/Azure/azure-cli/issues/2913)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-494">Bug fix - diagnostic settings create does not accept logs/metrics from show commands ([#2913](https://github.com/Azure/azure-cli/issues/2913))</span></span>

### <a name="network"></a><span data-ttu-id="3e3d9-495">Сеть</span><span class="sxs-lookup"><span data-stu-id="3e3d9-495">Network</span></span>

* <span data-ttu-id="3e3d9-496">Добавлена команда `network watcher test-connectivity`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-496">Add `network watcher test-connectivity` command.</span></span>
* <span data-ttu-id="3e3d9-497">Добавлена поддержка параметра `--filters` в команде `network watcher packet-capture create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-497">Add support for `--filters` parameter for `network watcher packet-capture create`.</span></span>
* <span data-ttu-id="3e3d9-498">Добавлена поддержка фильтрации подключений шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-498">Add support for Application Gateway connection draining.</span></span>
* <span data-ttu-id="3e3d9-499">Добавлена поддержка конфигурации набора правил WAF шлюза приложений.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-499">Add support for Application Gateway WAF rule set configuration.</span></span>
* <span data-ttu-id="3e3d9-500">Добавлена поддержка правил и фильтров маршрутов ExpressRoute.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-500">Add support for ExpressRoute route filters and rules.</span></span>
* <span data-ttu-id="3e3d9-501">Добавлена поддержка географической маршрутизации диспетчера трафика.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-501">Add support for TrafficManager geographic routing.</span></span>
* <span data-ttu-id="3e3d9-502">Добавлена поддержка селекторов трафика на основе политик для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-502">Add support for VPN connection policy-based traffic selectors.</span></span>
* <span data-ttu-id="3e3d9-503">Добавлена поддержка политик IPSec для VPN-подключений.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-503">Add support for VPN connection IPSec policies.</span></span>
* <span data-ttu-id="3e3d9-504">Исправлена ошибка `vpn-connection create`, возникавшая при использовании параметра `--no-wait` или `--validate`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-504">Fix bug with `vpn-connection create` when using the `--no-wait` or `--validate` parameters.</span></span>
* <span data-ttu-id="3e3d9-505">Добавлена поддержка шлюзов виртуальной сети "активный-активный".</span><span class="sxs-lookup"><span data-stu-id="3e3d9-505">Add support for active-active VNet gateways</span></span>
* <span data-ttu-id="3e3d9-506">Удалены значения NULL из выходных данных команды `network vpn-connection list/show`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-506">Remove nulls values from output of `network vpn-connection list/show` commands.</span></span>
* <span data-ttu-id="3e3d9-507">BC: исправлена ошибка в выходных данных `vpn-connection create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-507">BC: Fix bug in the output of `vpn-connection create`</span></span> 
* <span data-ttu-id="3e3d9-508">Исправлена ошибка, приводившая к неправильному анализу аргумента --key-length команды vpn-connection create.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-508">Fix bug where '--key-length' argument of 'vpn-connection create' was not parsed correctly.</span></span>
* <span data-ttu-id="3e3d9-509">Исправлена ошибка в `dns zone import`, из-за которой записи не импортировались правильно.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-509">Fix bug in `dns zone import` where records were not imported correctly.</span></span>
* <span data-ttu-id="3e3d9-510">Исправлена ошибка, из-за которой команда `traffic-manager endpoint update` не работала.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-510">Fix bug where `traffic-manager endpoint update` did not work.</span></span>
* <span data-ttu-id="3e3d9-511">Добавлены команды предварительного просмотра для Наблюдателя за сетями.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-511">Add 'network watcher' preview commands.</span></span>

### <a name="profile"></a><span data-ttu-id="3e3d9-512">Профиль</span><span class="sxs-lookup"><span data-stu-id="3e3d9-512">Profile</span></span>

* <span data-ttu-id="3e3d9-513">Поддержка входа при отсутствии подписок ([№ 2560](https://github.com/Azure/azure-cli/issues/2560)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-513">Support login when there are no subscriptions found ([#2560](https://github.com/Azure/azure-cli/issues/2560))</span></span>
* <span data-ttu-id="3e3d9-514">Поддержка сокращенных имен параметров в команде az account set --subscription ([№ 2980](https://github.com/Azure/azure-cli/issues/2980)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-514">Support short param name in az account set --subscription ([#2980](https://github.com/Azure/azure-cli/issues/2980))</span></span>

### <a name="redis"></a><span data-ttu-id="3e3d9-515">Redis</span><span class="sxs-lookup"><span data-stu-id="3e3d9-515">Redis</span></span>

* <span data-ttu-id="3e3d9-516">Добавлена команда update, которая также добавляет возможность масштабирования для кэша Redis.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-516">Adding update command which also adds the ability to scale for redis cache</span></span>
* <span data-ttu-id="3e3d9-517">Команда update-settings объявляется нерекомендуемой.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-517">Deprecates the 'update-settings' command.</span></span>

### <a name="resource"></a><span data-ttu-id="3e3d9-518">Ресурс</span><span class="sxs-lookup"><span data-stu-id="3e3d9-518">Resource</span></span>

* <span data-ttu-id="3e3d9-519">Добавлены команды определения managedapp и managedapp ([№ 2985](https://github.com/Azure/azure-cli/issues/2985)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-519">Add managedapp and managedapp definition commands ([#2985](https://github.com/Azure/azure-cli/issues/2985))</span></span>
* <span data-ttu-id="3e3d9-520">Поддержка команд provider operation ([№ 2908](https://github.com/Azure/azure-cli/issues/2908)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-520">Support 'provider operation' commands ([#2908](https://github.com/Azure/azure-cli/issues/2908))</span></span>
* <span data-ttu-id="3e3d9-521">Поддержка создания универсального ресурса ([№ 2606](https://github.com/Azure/azure-cli/issues/2606)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-521">Support generic resource create ([#2606](https://github.com/Azure/azure-cli/issues/2606))</span></span>
* <span data-ttu-id="3e3d9-522">Исправлен анализ ресурсов и поиск версии API.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-522">Fix resource parsing and api version lookup.</span></span> <span data-ttu-id="3e3d9-523">([№ 2781](https://github.com/Azure/azure-cli/issues/2781))</span><span class="sxs-lookup"><span data-stu-id="3e3d9-523">([#2781](https://github.com/Azure/azure-cli/issues/2781))</span></span>
* <span data-ttu-id="3e3d9-524">Добавлены документы для команды az lock update.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-524">Add docs for az lock update.</span></span> <span data-ttu-id="3e3d9-525">([№ 2702](https://github.com/Azure/azure-cli/issues/2702))</span><span class="sxs-lookup"><span data-stu-id="3e3d9-525">([#2702](https://github.com/Azure/azure-cli/issues/2702))</span></span>
* <span data-ttu-id="3e3d9-526">Исправлена ошибка, возникавшая при попытке вывести список ресурсов группы, которая не существует.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-526">Error out if you try to list resources for a group that doesn't exist.</span></span> <span data-ttu-id="3e3d9-527">([№ 2769](https://github.com/Azure/azure-cli/issues/2769))</span><span class="sxs-lookup"><span data-stu-id="3e3d9-527">([#2769](https://github.com/Azure/azure-cli/issues/2769))</span></span>
* <span data-ttu-id="3e3d9-528">[Вычисления.] Устранены проблемы с масштабируемым набором виртуальных машин и обновлением группы доступности виртуальных машин.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-528">[Compute] Fix issues with VMSS and VM availability set update.</span></span> <span data-ttu-id="3e3d9-529">([№ 2773](https://github.com/Azure/azure-cli/issues/2773))</span><span class="sxs-lookup"><span data-stu-id="3e3d9-529">([#2773](https://github.com/Azure/azure-cli/issues/2773))</span></span>
* <span data-ttu-id="3e3d9-530">Исправлена блокировка создания и удаления, возникающая, если параметр parent-resource-path не указан ([№ 2742](https://github.com/Azure/azure-cli/issues/2742)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-530">Fix lock create and delete if parent-resource-path is None ([#2742](https://github.com/Azure/azure-cli/issues/2742))</span></span>

### <a name="role"></a><span data-ttu-id="3e3d9-531">Роль</span><span class="sxs-lookup"><span data-stu-id="3e3d9-531">Role</span></span>

* <span data-ttu-id="3e3d9-532">create-for-rbac: гарантируется, что дата завершения работы поставщика служб не может превышать срок действия сертификата ([№ 2989](https://github.com/Azure/azure-cli/issues/2989)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-532">create-for-rbac: ensure SP's end date will not exceed certificate's expiration date ([#2989](https://github.com/Azure/azure-cli/issues/2989))</span></span>
* <span data-ttu-id="3e3d9-533">RBAC: добавлена полная поддержка команды ad group ([№ 2016](https://github.com/Azure/azure-cli/issues/2016)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-533">RBAC: add full support for 'ad group' ([#2016](https://github.com/Azure/azure-cli/issues/2016))</span></span>
* <span data-ttu-id="3e3d9-534">Роль: устранены проблемы при обновлении определения роли ([№ 2745](https://github.com/Azure/azure-cli/issues/2745)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-534">role: fix issues on role definition update ([#2745](https://github.com/Azure/azure-cli/issues/2745))</span></span>
* <span data-ttu-id="3e3d9-535">create-for-rbac: обеспечен выбор введенного пользователем пароля.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-535">create-for-rbac: ensure user provided password is picked up</span></span>

### <a name="sql"></a><span data-ttu-id="3e3d9-536">SQL</span><span class="sxs-lookup"><span data-stu-id="3e3d9-536">SQL</span></span>

* <span data-ttu-id="3e3d9-537">Добавлены команды az sql server list-usages и az sql db list-usages.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-537">Added az sql server list-usages and az sql db list-usages commands.</span></span>
* <span data-ttu-id="3e3d9-538">SQL: возможность прямого подключения к поставщику ресурса ([№ 2832](https://github.com/Azure/azure-cli/issues/2832)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-538">SQL - ability to connect directly to resource provider ([#2832](https://github.com/Azure/azure-cli/issues/2832))</span></span>

### <a name="storage"></a><span data-ttu-id="3e3d9-539">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3e3d9-539">Storage</span></span>

* <span data-ttu-id="3e3d9-540">Добавлено расположение по умолчанию группы ресурсов для `storage account create`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-540">Default location to resource group location for `storage account create`.</span></span>
* <span data-ttu-id="3e3d9-541">Добавлена поддержка добавочного копирования больших двоичных объектов.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-541">Add support for incremental blob copy</span></span>
* <span data-ttu-id="3e3d9-542">Добавлена поддержка передачи больших блочных BLOB-объектов.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-542">Add support for large block blob upload</span></span>
* <span data-ttu-id="3e3d9-543">Размер блока изменяется и составляет 100 МБ, если передается файл, чей размер превышает 200 ГБ.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-543">Change block size to 100MB when file to upload is larger than 200GB</span></span>

### <a name="vm"></a><span data-ttu-id="3e3d9-544">ВМ</span><span class="sxs-lookup"><span data-stu-id="3e3d9-544">VM</span></span>

* <span data-ttu-id="3e3d9-545">avail-set: число доменов обновления и доменов сбоя сделано необязательным.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-545">avail-set: make UD&FD domain counts optional</span></span>

  <span data-ttu-id="3e3d9-546">Примечание. Команды виртуальной машины в независимых облаках: избегайте использовать функции, связанные с Управляемыми дисками, включая следующие:</span><span class="sxs-lookup"><span data-stu-id="3e3d9-546">note: VM commands in sovereign clouds Please avoid managed disk related features, including the following:</span></span>
  1. <span data-ttu-id="3e3d9-547">az disk/snapshot/image</span><span class="sxs-lookup"><span data-stu-id="3e3d9-547">az disk/snapshot/image</span></span>
  2. <span data-ttu-id="3e3d9-548">az vm/vmss disk</span><span class="sxs-lookup"><span data-stu-id="3e3d9-548">az vm/vmss disk</span></span>
  3. <span data-ttu-id="3e3d9-549">В команде az vm/vmss create используйте параметр --use-unmanaged-disk, чтобы избежать использования Управляемых дисков. Другие команды должны работать.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-549">Inside "az vm/vmss create", use "—use-unmanaged-disk" to avoid managed disk Other commands should work</span></span>
* <span data-ttu-id="3e3d9-550">vm/vmss: улучшен текст предупреждения при создании пары ключей SSH.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-550">vm/vmss: improve the warning text when generates ssh key pairs</span></span>
* <span data-ttu-id="3e3d9-551">vm/vmss: поддержка создания из образа Marketplace, для которого требуются сведения о плане ([№ 1209](https://github.com/Azure/azure-cli/issues/1209)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-551">vm/vmss: support create from a market place image which requires plan info ([#1209](https://github.com/Azure/azure-cli/issues/1209))</span></span>


## <a name="april-3-2017"></a><span data-ttu-id="3e3d9-552">3 апреля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-552">April 3, 2017</span></span>

<span data-ttu-id="3e3d9-553">Версия 2.0.2</span><span class="sxs-lookup"><span data-stu-id="3e3d9-553">Version 2.0.2</span></span>

<span data-ttu-id="3e3d9-554">В этом выпуске мы добавили компоненты ACR, Batch, KeyVault и SQL.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-554">We released the ACR, Batch, KeyVault, and SQL components in this release.</span></span>

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

### <a name="core"></a><span data-ttu-id="3e3d9-555">Core</span><span class="sxs-lookup"><span data-stu-id="3e3d9-555">Core</span></span>

* <span data-ttu-id="3e3d9-556">Модули Acr, Lab, Monitor и Find добавлены в список по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-556">Add acr, lab, monitor, and find modules to default list.</span></span>
* <span data-ttu-id="3e3d9-557">Вход: пропуск неправильного клиента ([#2634](https://github.com/Azure/azure-cli/pull/2634)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-557">Login: skip erroneous tenant ([#2634](https://github.com/Azure/azure-cli/pull/2634))</span></span>
* <span data-ttu-id="3e3d9-558">Вход: для подписки по умолчанию задано значение 1 с состоянием "Включено" ([#2575](https://github.com/Azure/azure-cli/pull/2575)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-558">login: set default subscription to one with the state of "Enabled" ([#2575](https://github.com/Azure/azure-cli/pull/2575))</span></span>
* <span data-ttu-id="3e3d9-559">Добавлена поддержка команд wait и --no-wait для дополнительных команд ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-559">Add wait commands and --no-wait support to more commands ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="3e3d9-560">Core: поддержка входа при помощи субъекта-службы с использованием сертификата ([#2457](https://github.com/Azure/azure-cli/pull/2457)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-560">core: support login using service principal with a cert ([#2457](https://github.com/Azure/azure-cli/pull/2457))</span></span>
* <span data-ttu-id="3e3d9-561">Добавлен запрос для отсутствующих параметров шаблона</span><span class="sxs-lookup"><span data-stu-id="3e3d9-561">Add prompting for missing template parameters.</span></span> <span data-ttu-id="3e3d9-562">([#2364](https://github.com/Azure/azure-cli/pull/2364)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-562">([#2364](https://github.com/Azure/azure-cli/pull/2364))</span></span>
* <span data-ttu-id="3e3d9-563">Добавлена поддержка установки параметров по умолчанию для таких распространенных аргументов, как группа ресурсов по умолчанию, веб-страница по умолчанию, виртуальная машина по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-563">Support setting default values for common arguments like default resource group, default web, default vm</span></span>
* <span data-ttu-id="3e3d9-564">Добавлена поддержка входа на конкретный клиент.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-564">Support login to specific tenant</span></span>
 
### <a name="acs"></a><span data-ttu-id="3e3d9-565">ACS</span><span class="sxs-lookup"><span data-stu-id="3e3d9-565">ACS</span></span>

* <span data-ttu-id="3e3d9-566">[ACS] Добавлена поддержка настройки кластера ACS по умолчанию ([#2554](https://github.com/Azure/azure-cli/pull/2554)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-566">[ACS] Adding support for configuring a default ACS cluster ([#2554](https://github.com/Azure/azure-cli/pull/2554))</span></span>
* <span data-ttu-id="3e3d9-567">Добавлена поддержка запроса пароля для ключа SSH</span><span class="sxs-lookup"><span data-stu-id="3e3d9-567">Add support for ssh key password prompting.</span></span> <span data-ttu-id="3e3d9-568">([#2044](https://github.com/Azure/azure-cli/pull/2044)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-568">([#2044](https://github.com/Azure/azure-cli/pull/2044))</span></span>
* <span data-ttu-id="3e3d9-569">Добавлена поддержка кластеров Windows</span><span class="sxs-lookup"><span data-stu-id="3e3d9-569">Add support for windows clusters.</span></span> <span data-ttu-id="3e3d9-570">([#2211](https://github.com/Azure/azure-cli/pull/2211)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-570">([#2211](https://github.com/Azure/azure-cli/pull/2211))</span></span>
* <span data-ttu-id="3e3d9-571">Добавлена возможность изменения роли "Владелец" на роль "Участник"</span><span class="sxs-lookup"><span data-stu-id="3e3d9-571">Switch from Owner to Contributor role.</span></span> <span data-ttu-id="3e3d9-572">([#2321](https://github.com/Azure/azure-cli/pull/2321)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-572">([#2321](https://github.com/Azure/azure-cli/pull/2321))</span></span>
 
### <a name="appservice"></a><span data-ttu-id="3e3d9-573">AppService</span><span class="sxs-lookup"><span data-stu-id="3e3d9-573">AppService</span></span>

* <span data-ttu-id="3e3d9-574">AppService: добавлена поддержка получения внешнего IP-адреса, используемого для записей DNS типа A ([#2627](https://github.com/Azure/azure-cli/pull/2627)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-574">appservice: support to get external ip address used for DNS A records ([#2627](https://github.com/Azure/azure-cli/pull/2627))</span></span>
* <span data-ttu-id="3e3d9-575">AppService: добавлена поддержка привязки групповых сертификатов ([#2625](https://github.com/Azure/azure-cli/pull/2625)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-575">appservice: support binding wildcard certificates ([#2625](https://github.com/Azure/azure-cli/pull/2625))</span></span>
* <span data-ttu-id="3e3d9-576">AppService: добавлена поддержка профилей для публикации списком ([#2504](https://github.com/Azure/azure-cli/pull/2504)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-576">appservice: support list publishing profiles ([#2504](https://github.com/Azure/azure-cli/pull/2504))</span></span>
* <span data-ttu-id="3e3d9-577">AppService: добавлен триггер синхронизации с системой управления версиями после настройки ([#2326](https://github.com/Azure/azure-cli/pull/2326)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-577">AppService - Trigger source control sync after config ([#2326](https://github.com/Azure/azure-cli/pull/2326))</span></span>
 
### <a name="datalake"></a><span data-ttu-id="3e3d9-578">DataLake</span><span class="sxs-lookup"><span data-stu-id="3e3d9-578">DataLake</span></span>

* <span data-ttu-id="3e3d9-579">Первоначальный выпуск модуля Data Lake Analytics.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-579">Initial release of Data Lake Analytics module.</span></span>
* <span data-ttu-id="3e3d9-580">Первоначальный выпуск модуля Data Lake Store.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-580">Initial release of Data Lake Store module.</span></span>
 
### <a name="docuemntdb"></a><span data-ttu-id="3e3d9-581">DocumentDB</span><span class="sxs-lookup"><span data-stu-id="3e3d9-581">DocuemntDB</span></span>

* <span data-ttu-id="3e3d9-582">DocumentDB: добавлена поддержка для получения списка строк подключения ([#2580](https://github.com/Azure/azure-cli/pull/2580)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-582">DocumentDB: Adding support for listing connection strings ([#2580](https://github.com/Azure/azure-cli/pull/2580))</span></span>

### <a name="vm"></a><span data-ttu-id="3e3d9-583">ВМ</span><span class="sxs-lookup"><span data-stu-id="3e3d9-583">VM</span></span>

* <span data-ttu-id="3e3d9-584">[Вычисления] Добавлена поддержка AppGateway для создания масштабируемого набора виртуальных машин ([#2570](https://github.com/Azure/azure-cli/pull/2570)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-584">[Compute] Add AppGateway support to virtual machine scale set create ([#2570](https://github.com/Azure/azure-cli/pull/2570))</span></span>
* <span data-ttu-id="3e3d9-585">[ВМ и VMSS] Улучшена поддержка кэширования диска ([#2522](https://github.com/Azure/azure-cli/pull/2522)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-585">[VM/VMSS] Improved disk caching support ([#2522](https://github.com/Azure/azure-cli/pull/2522))</span></span>
* <span data-ttu-id="3e3d9-586">ВМ и VMSS: внедрена логика проверки учетных данных, используемая на портале ([#2537](https://github.com/Azure/azure-cli/pull/2537)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-586">VM/VMSS: incorporate credentials validation logic used by portal ([#2537](https://github.com/Azure/azure-cli/pull/2537))</span></span>
* <span data-ttu-id="3e3d9-587">Добавлена поддержка команд wait и --no-wait ([#2524](https://github.com/Azure/azure-cli/pull/2524)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-587">Add wait commands and --no-wait support ([#2524](https://github.com/Azure/azure-cli/pull/2524))</span></span>
* <span data-ttu-id="3e3d9-588">Масштабируемый набор виртуальных машин: добавлена поддержка * для представления экземпляров на виртуальных машинах в виде списка ([#2467](https://github.com/Azure/azure-cli/pull/2467)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-588">Virtual machine scale set: support * to list instance view across vms ([#2467](https://github.com/Azure/azure-cli/pull/2467))</span></span>
* <span data-ttu-id="3e3d9-589">Добавлена команда --secrets для виртуальных машин и масштабируемого набора виртуальных машин ([#2212}(https://github.com/Azure/azure-cli/pull/2212)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-589">Add --secrets for VM and virtual machine scale set ([#2212}(https://github.com/Azure/azure-cli/pull/2212))</span></span>
* <span data-ttu-id="3e3d9-590">Добавлено разрешение на создание виртуальных машин на основе специализированного образа VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256)).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-590">Allow VM creation with specialized VHD ([#2256](https://github.com/Azure/azure-cli/pull/2256))</span></span>

## <a name="february-27-2017"></a><span data-ttu-id="3e3d9-591">27 февраля 2017 г.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-591">February 27, 2017</span></span>

<span data-ttu-id="3e3d9-592">Версия 2.0.0</span><span class="sxs-lookup"><span data-stu-id="3e3d9-592">Version 2.0.0</span></span>

<span data-ttu-id="3e3d9-593">Этот первый общедоступный выпуск Azure CLI 2.0.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-593">This release of Azure CLI 2.0 is the first "Generally Available" release.</span></span>
<span data-ttu-id="3e3d9-594">Общедоступными являются такие командные модули:</span><span class="sxs-lookup"><span data-stu-id="3e3d9-594">General availability applies to these command modules:</span></span>
- <span data-ttu-id="3e3d9-595">служба контейнеров (ACS);</span><span class="sxs-lookup"><span data-stu-id="3e3d9-595">Container Service (acs)</span></span>
- <span data-ttu-id="3e3d9-596">вычисления (в том числе Resource Manager, виртуальная машина, масштабируемые наборы виртуальных машин, управляемые диски);</span><span class="sxs-lookup"><span data-stu-id="3e3d9-596">Compute (including Resource Manager, VM, virtual machine scale sets, Managed Disks)</span></span>
- <span data-ttu-id="3e3d9-597">Сеть</span><span class="sxs-lookup"><span data-stu-id="3e3d9-597">Networking</span></span>
- <span data-ttu-id="3e3d9-598">Хранилище</span><span class="sxs-lookup"><span data-stu-id="3e3d9-598">Storage</span></span>

<span data-ttu-id="3e3d9-599">Эти командные модули могут использоваться в рабочих средах и поддерживаются стандартными соглашениями Майкрософт об уровне обслуживания.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-599">These command modules can be used in production and are supported by standard Microsoft SLA.</span></span>
<span data-ttu-id="3e3d9-600">Вы можете отправлять запросы непосредственно в службу технической поддержки Майкрософт или добавлять описание проблем в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-600">You can open issues directly with Microsoft support or on our [github issues list](https://github.com/azure/azure-cli/issues/).</span></span>
<span data-ttu-id="3e3d9-601">Вы можете задавать вопросы на сайте [StackOverflow, используя тег azure-cli](http://stackoverflow.com/questions/tagged/azure-cli), или обращаться к группе разработчиков по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). Можно отправлять отзывы из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-601">You can ask questions on [StackOverflow using the azure-cli tag](http://stackoverflow.com/questions/tagged/azure-cli), or contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com). You can provide feedback from the command line with the `az feedback` command.</span></span>

<span data-ttu-id="3e3d9-602">Команды в этих модулях стабильны, и предполагается, что в следующих выпусках этой версии Azure CLI их синтаксис не будет меняться.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-602">The commands in these modules are stable and the syntax is not expected to change in upcoming releases of this version of Azure CLI.</span></span>

<span data-ttu-id="3e3d9-603">Чтобы проверить версию интерфейса командной строки, используйте `az --version`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-603">To verify the version of the CLI, use `az --version`.</span></span>
<span data-ttu-id="3e3d9-604">В выходных данных указана версия самого интерфейса командной строки (2.0.0 в этом выпуске), версии отдельных командных модулей и используемые вами версии Python и GCC.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-604">The output lists the version of the CLI itself (2.0.0 in this release), the individual command modules, and the versions of Python and GCC that you're using.</span></span>

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
> <span data-ttu-id="3e3d9-605">Некоторые командные модули имеют постфикс b*n* или rc*n*.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-605">Some of the command modules have a "b*n*" or "rc*n*" postfix.</span></span>
> <span data-ttu-id="3e3d9-606">Эти командные модули все еще находятся на стадии предварительной версии и станут общедоступными в будущем.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-606">These command modules are still in preview and will become generally available in the future.</span></span>

<span data-ttu-id="3e3d9-607">У нас также есть предварительные ежедневные сборки интерфейса командной строки.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-607">We also have nightly preview builds of the CLI.</span></span>
<span data-ttu-id="3e3d9-608">Дополнительные сведения см. в инструкциях по [получению ежедневных сборок](https://github.com/Azure/azure-cli#nightly-builds), а также в инструкциях по [настройке среды разработки и участии в написании кода](https://github.com/Azure/azure-cli#developer-setup).</span><span class="sxs-lookup"><span data-stu-id="3e3d9-608">For information, see these instructions on [getting the nightly builds](https://github.com/Azure/azure-cli#nightly-builds), and these instructions on [developer setup and contributing code](https://github.com/Azure/azure-cli#developer-setup).</span></span>

<span data-ttu-id="3e3d9-609">О проблемах с предварительными ежедневными сборками можно сообщить несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="3e3d9-609">You can report issues with nightly preview builds in the following ways:</span></span>
- <span data-ttu-id="3e3d9-610">добавив информацию о проблемах в наш [список на сайте GitHub](https://github.com/azure/azure-cli/issues/);</span><span class="sxs-lookup"><span data-stu-id="3e3d9-610">Report issues in our [github issues list](https://github.com/azure/azure-cli/issues/)</span></span>
- <span data-ttu-id="3e3d9-611">обратившись к специалистам группы разработчиков продукта по адресу электронной почты [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com);</span><span class="sxs-lookup"><span data-stu-id="3e3d9-611">Contact the product team at [azfeedback@microsoft.com](mailto:azfeedback@microsoft.com).</span></span>
- <span data-ttu-id="3e3d9-612">отправив отзыв из командной строки с помощью команды `az feedback`.</span><span class="sxs-lookup"><span data-stu-id="3e3d9-612">Provide feedback from the command line with the `az feedback` command.</span></span>

